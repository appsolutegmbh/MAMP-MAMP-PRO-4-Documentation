---
title: MAMP PRO (Mac) Documentation > How Tos > General
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### How Do I Send Email Using Postfix?

The way we to transport emails over the internet is by using a Mail Transfer Agent (MTA) with its Simple Mail Transfer Protocol (SMTP). MAMP PRO uses Postfix as its MTA. Most of the email providers have a strong filter in their systems, which allows to pass only emails with some default headers. The following will help you send email using postfix. You will need to create 3 files, and one new subdirectory.

1. Add a new host in MAMP PRO, call it  "hostmailer".
2. Create an "email" subdirectory. Add an empty "InvatationEmail.php", "invatationMessage.html" and "script.php" to your "email" subdirectory. 
3. In the Postfix tab, check the box "Include Postfix service in GroupStart".
4. Set "domain of outgoing emails" to: hostmailer.com .
5. Save and restart the servers.
6. Open the hostmailer page and add to the browser path input: hostmailer/email/script.php .
7. After a few minutes you should receive your email (check if it didn’t go to spam).

---

Copy and paste the following. This will be your "InvatationEmail.php" file.

{% highlight php %}

  <?php
    class InvitationEmail {
		
		function sendEmailMessage($messageDetails){
			$message_subject = $messageDetails["message_subject"];
			$to_email = $messageDetails["to_email"];
			$from_name = $messageDetails["from_name"];
			$from_email = $messageDetails["from_email"];
			$message_body = $messageDetails["message_body"];
			
			$headers = 'MIME-Version: 1.0' . "\r\n";
			$headers .= 'Content-type: text/html; charset=iso-8859-1' . "\r\n";
			$headers .= "From: ".$from_name."<".$from_email.">"."\r\n";
			
			mail($to_email, $message_subject,$message_body,$headers);
		}
		
		function generateMessageBody(){
			$myfile = fopen("invitationMessage.html", "r");
			$returnValue = fread($myfile, filesize("invitationMessage.html"));
			fclose($myfile);
			
			return $returnValue;
		}
	}
?>

 {% endhighlight %}
 
---
 
 Copy and paste the following. This will be your "invatationMessage.html" file.

{% highlight php %}

  <!DOCTYPE html>
<html>
<head>
<title>MAMP PRO Invitation</title>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
</head>

<body>
	Hi there, <br><br>
	
    Your friend {name} has invited you to test MAMP PRO.<br><br>
    
	You can test MAMP PRO by downloading it from https://www.mamp.info/en/downloads/ .<br><br>
    
    MAMP PRO team.
</body>
</html>

{% endhighlight %}

---

Copy and paste the following. This will be your "script.php" file. Add the correct email address. 

{% highlight php %}

 <?php

/*__________________INPUT_DATA______________________*/

    $to_email = "john@gmaill.com"; // you are sending email to .. change the email recipient
    $your_name = "john";

/*____________________SCRIPT________________________*/
    
    require("InvitationEmail.php");
    
    $messageDetails = array();
	$messageDetails["message_subject"] = "Invitation to MAMP PRO";
	$messageDetails["to_email"] = $to_email; 
	$messageDetails["from_name"] = "MAMP PRO";
	$messageDetails["from_email"] = "donotreply";
		
	$invitationEmail = new InvitationEmail();
		
	$messageBody = $invitationEmail->generateMessageBody();
	$emailMessage = str_replace("{name}", $your_name, $messageBody);
		
	$messageDetails["message_body"] = $emailMessage;
		
	$invitationEmail->sendEmailMessage($messageDetails);
	
	$returnValue["status"] = "200";
	$returnValue["message"] = "Email sent to ".$to_email.". Check it in your Inbox or Spam Folder";
	echo json_encode($returnValue);
?>
  
{% endhighlight %}

---

More detailed information about postfix can be found [here](http://www.postfix.org/BASIC_CONFIGURATION_README.html){:target="_blank"}. 











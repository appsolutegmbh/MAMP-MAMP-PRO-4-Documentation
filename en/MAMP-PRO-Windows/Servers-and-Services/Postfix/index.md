---
title: MAMP PRO (Windows) Documentation > Servers and Services > SMTP
description: 
layout: default-2
product: MAMP PRO Windows
language: en
---

## Servers and Services > SMTP

Sometimes you may need to send an email using PHP, to do so you have to configure and start SMTP. An easy way getting SMTP to run is using the configuration tool built into MAMP PRO. 

![MAMP](/en/MAMP-PRO-Windows/Servers-and-Services/Postfix/smtp.png)

*  **Include SMPT service in GroupStart**  

   Check to include SMTP in the GroupStart. When activated SMTP will automatically start/stop when the Servers button is   pressed.

---

*  **Set domain of outgoing e-mails to**

   If you want to use the PHP function `mail()` for sending emails to your own email address (like mail@johndoe.com) you
   just need to add the value "johndoe.com" (without quotes and the according domain name) into this field. 
   
   <div class="alert" role="alert">
   Note: Only if you want to send e-mail to others you will need to fill
   in the other fields. In this case make sure that your e-mail provider allows the use of a Smart host.
   </div>
---

*  **Use a smart host for routing**  

    *  **Outgoing server:**  
       Fill in your server name for outgoing emails. This could be for instance "smtp.johndoe.com" (without quotes).
       Ask your provider if you are unsure about the server name.  

    *  **Use authentication**  
       Unencrypted: Your username and password will be sent unencrypted.
       
       MD5 Challenge-Response: MD5 Challenge Response Authentication will be used.

    *  **User name**  
       Add the user name of your mail account.  

    *  **Password**  
       Add the password for your email user account.  

    *  **Authentication**  
       What type of authentication to be used.  
  
   <div class="alert" role="alert">
   Note: Some providers do not allow Smart-Hosts, like Google Mail.
   </div>

---

*  **Path to SMTP log file**  

The path to your SMTP log file.

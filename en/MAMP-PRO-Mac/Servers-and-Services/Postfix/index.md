---
title: MAMP PRO (Mac) Documentation > Servers and Services > Postfix
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

## Servers and Services > Postfix

You may need to send an email using PHP. To do so you have to configure and start Postfix. An easy way getting Postfix to run is using the configuration tool built into MAMP PRO. A How-To with example code on sending email with Postfix can be found [here](../../How-Tos/General/SendMailPostfix).

![MAMP](/en/MAMP-PRO-Mac/Servers-and-Services/Postfix/Postfix.png)

*  **Include Postfix service in GroupStart**  

   Check to include Postfix in the GroupStart. When activated Postfix will automatically start/stop when the Servers button is pressed.

---

*  **Set domain of outgoing e-mails to**

   Use the PHP function `mail()` for sending emails to your own email address (like mail@johndoe.com). This field to set the outgoing email domain. After starting your servers with this set, you will see your changes reflected in  `/private/etc/postfix/main.cf`.
   
   {% highlight php %}

   ### MAMP Postfix Configuration - Start ###

   myorigin = johndoe.com
   myhostname = mailer.$myorigin
   smtpd_sender_restrictions = permit_inet_interfaces
   
   {% endhighlight %}

---

*  **Use a smart host for routing**  

    *  **Server name**  
       Fill in your server name for outgoing emails. This could be for instance "smtp.johndoe.com" (without quotes).
       Ask your provider if you are unsure about the server name.  

    *  **Authentication**  
       Unencrypted: Your username and password will be sent unencrypted.
       
       MD5 Challenge-Response: MD5 Challenge Response Authentication will be used.

    *  **User name**  
       Add the user name of your mail account.  

    *  **Password**  
       Add the password for your email user account.  

  
  MAMP PRO will move your existing main.cf and master.cf files to `/private/etc/postfix/MAMP_backup` when you include Postfix using the Groupstart in MAMP PRO. When you stop uncheck Groupstart your original postfix files will be moved back to `/private/etc/postfix`.
  
  <div class="alert" role="alert">
   Note: Some providers do not allow Smart-Hosts, like Google Mail.
   </div>

---

*  **Path to Postfix log file**  

   The path to your postfix log.
   
---

   

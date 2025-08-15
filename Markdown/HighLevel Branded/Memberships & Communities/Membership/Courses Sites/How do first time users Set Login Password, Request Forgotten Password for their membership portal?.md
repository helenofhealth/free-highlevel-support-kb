**Date Updated:** 2025-04-07T11:03:30.000Z

This article explains how users can set their password for the first time or reset it if forgotten using the magic link system. Whether access is granted through checkout or automation, this guide ensures your members know exactly how to securely log in and manage their credentials. It applies to both course and client portal access, creating a consistent experience across the platform.

---

**TABLE OF CONTENTS**

* [What is the Password Setup Process?](#What-is-the-Password-Setup-Process?)  
   * [Configuring: How Users Set or Reset Password](#Configuring%3A-How-Users-Set-or-Reset-Password)  
         * [Checkout (after purchasing an offer) :](#Checkout-%28after-purchasing-an-offer%29-%3A)  
         * [Manual enrollment by the admin](#Manual-enrollment-by-the-admin)  
         * [Automated workflows or smart list actions](#Automated-workflows-or-smart-list-actions)  
         * [Thank you Page](#Thank-you-Page)  
         * [Set Password](#Set-Password)  
         * [Password Reset](#Password-Reset)  
   * [Frequently Asked Questions](#Frequently-Asked-Questions)

---
  
  
---

# **What is the Password Setup Process?**

  
When a user gains access to a course or membership area, they no longer receive system-generated passwords. Instead, they receive an email with a secure magic link prompting them to create their own password. This modern approach improves security, enhances the user experience, and eliminates the need for admins to manually manage credentials. The same flow applies whether it’s a first-time login or a password reset request.

---

## **Configuring: How Users Set or Reset Password**

  
 Learn different ways users receive access to your courses and how they create or reset their passwords.

  
### **Checkout (after purchasing an offer) :**

  
New users are granted access to a course or membership after completing the checkout process, as shown in the screenshot. Once they enter their email and full name, clicking **“Proceed to checkout”** enrolls them in the offer. This action also triggers an automated email with a magic login link, prompting them to set their own password and access the course.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155044610969/original/LS1lS3ZpmrhnyklrnjDPQyU2w76p64Ugog.png?1743991978)
  
  
### **Manual enrollment by the admin**

  
Admins can manually enroll a user into a course by navigating to the contact’s profile and selecting an offer from the dropdown menu. This action triggers the same magic link email, allowing the user to set their password and access the course.

  
### **Automated workflows or smart list actions**

  
Users can be automatically enrolled into a course through workflows or smart list actions using triggers like “Offer Access Granted” or “Membership New Signup.” These automations send a system email containing a magic link. When users click it, they’re prompted to set their password and gain instant access.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155044612928/original/4eZko-NSaJjo3mwadVL8xHDY9L0e9TIosw.png?1743998486)
  
  
### **Thank you Page**

  
After completing the signup, users will see a confirmation message with a **“View Dashboard”** button. Clicking this takes them to a page where they’ll be prompted to set a new password before accessing the course.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155044611001/original/jFqID9jOzIA6xusuFatf-pRXPGcd6cCbCw.png?1743992158)
  
  
### **Set Password**

  
When they click it, they are prompted to set a new password. After setting the password, they are redirected to the course or membership dashboard

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155044612758/original/oBR8RMEtAb1yJfxinKsaPPMKAW5izf2pjA.png?1743998098)
  
  
### **Password Reset**

  
If a user forgets their password, they can go to the login page and click **“Forgot Password”** Enter their email and receive a password reset link. This link redirects them to set a new password and Automatically logs them into the course or portal once reset. Below is the example of the email a user receives when they request for a password reset link through Forgot Password option. 

  
The password reset link Expires in 2 hours. Be sure to reset the password within the given time.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155044613562/original/74YDK23_UOpCXiG4ntAYbfK7pABJzrOsEA.png?1744000459)

  
---

## **Frequently Asked Questions**

  
**Q:** **How can I ensure new users receive the email to set their password?**

Ensure that the email associated with the user is accurate and that the system-generated "Courses Login URL" email is enabled. You can check email delivery logs to confirm whether the email was sent successfully.
  
  
**Q: What should I do if a user reports not receiving the password reset email?**

Verify the user’s email address in the system and check the email delivery logs. Ensure that your email domain is properly authenticated (e.g., via SPF, DKIM) to prevent emails from being marked as spam. If needed, you can manually resend the email.
  
  
**Q: Can I reset a user’s password for them?**

No, admins cannot directly reset a user’s password for security reasons. However, you can guide the user to use the "Forgot Password" option or resend the password setup email from the system.
  
  
**Q: How do I monitor or troubleshoot password setup issues for users?**

Check the user's account status in the CRM to ensure they are properly added to the membership portal. Review email deliverability logs for issues like bounces or spam filtering. If issues persist, contact support for assistance.
**Date Updated:** 2024-08-13T21:49:02.000Z

Nearly everything you need to know about connecting your domain

---

**TABLE OF CONTENTS**

* [What is a Domain?](#What-is-a-Domain?)  
   * [What are Root & Sub-Domains](#What-are-Root-&-Sub-Domains)  
   * [Seamlessly Connect Domains with Domain Connect](#Seamlessly-Connect-Domains-with-Domain-Connect)  
         * [Manual Option](#Manual-Option)
* [Places to Add Domains](#Places-to-Add-Domains-to-in-HighLevel)  
   * [Whitelabel Domain](#Whitelabel-Domain)  
   * [API or Branded Domain](#API-or-Branded-Domain)  
   * [Sites (Settings > Domains)](#Sites-%28Settings-%3E-Domains%29)  
   * [Email Sending Domain](#Email-Sending-Domain)  
   * [Client Portal Domain (Communities, Courses)](#Client-Portal-Domain-%28Communities,-Courses%29)  
   * [WordPress](#WordPress)
* [Domain Glossary - Key Words to Know](#Domain-Glossary---Key-Words-to-Know)
* [Troubleshooting](#Troubleshooting)  
   * [1\. Check for Duplicate A Records:](#1.-Check-for-Duplicate-A-Records%3A)  
   * [2\. Confirm DNS Propagation](#2.-Confirm-DNS-Propagation)  
   * [3\. Review DNS Settings for Accuracy:](#3.-Review-DNS-Settings-for-Accuracy%3A)  
   * [4\. Verify Domain DNS Integration:](#4.-Verify-Domain-DNS-Integration%3A)  
   * [5\. Consider Other Potential Causes:](#5.-Consider-Other-Potential-Causes%3A)  
   * [6\. Seek Additional Assistance:](#6.-Seek-Additional-Assistance%3A)
* [FAQ](#FAQ)  
   * [What If I do not have a domain?](#What-If-I-do-not-have-a-domain?)  
   * [Can I use an existing domain for my email?](#Can-I-use-an-existing-domain-for-my-email?)  
   * [Can I use WIX for my Dedicated Domain?](#Can-I-use-WIX-for-my-Dedicated-Domain?)  
   * [My Cname record is not being recognized in Cloudflare.](#My-Cname-record-is-not-being-recognized-in-Cloudflare.)  
   * [What if I have an existing domain?](#What-if-I-have-an-existing-domain?)

---

# What is a Domain?

A domain serves as the digital address for online services like websites, email hosting, and more, by mapping them to IP addresses through DNS. Domain names are essential for your online presence, enhancing website accessibility and enabling email communication.

  
Domains are crucial for website hosting, white-label branding, configuring branded/API domains, email setup, and the Client portal. They form the foundation upon which HighLevel users build their digital presence.

  
## What are Root & Sub-Domains

When working with domains, it's important to distinguish between a root domain and a subdomain. 

* **Root Domain** (Example: “mywebsite.com”)  
   * The root domain is the primary address of your website, appearing after "www." in a URL (e.g., in "www.mywebsite.com," the root domain is "mywebsite.com"). It serves as the main entry point to your website.
* **Subdomain** (Example: "help.domain.com")  
   * Subdomains are extensions of your root domain, directing users to specific sections or areas within your online infrastructure (e.g., "help.domain.com" for support). This allows for separate content, landing pages, and marketing campaigns without affecting the primary site. This setup is useful for ads, promotions, and utilizing different SEO strategies.

**IMPORTANT NOTE:** Be careful when adding root domains. Many users accidentally break their existing mailbox or site by adding a root domain already in use. We recommend adding a sub-domain if your root domain is used somewhere else.

  
---

## Seamlessly Connect Domains with Domain Connect

**If your domain provider is Google, Cloudflare, or GoDaddy**, The system offers automatic DNS configuration for connecting your domain to the platform. This feature eliminates the need to manually manage DNS records for branded domains, websites, dedicated domains, and the client portal. Auto-configuration streamlines domain integration, saving time and reducing the risk of errors.

To see more information about seamlessly connecting domains, please visit [](https://help.gohighlevel.com/support/solutions/articles/155000000734-how-to-use-the-domain-connect-feature-)[How to Use the Domain Connect Feature](https://help.gohighlevel.com/support/solutions/articles/155000000734-how-to-use-the-domain-connect-feature-)

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095806/original/hrpCoz1Kx3xl9cE9J2HRAABgfYYjIdiccA.png?1717515282)

  
### Manual Option

**If your domain provider is not Google, Cloudflare, or GoDaddy**, manual DNS configuration is required. The system simplifies this process by generating the necessary record values for you to input into your domain provider's system. This ensures seamless integration of your domain with HighLevel, supporting branded domains, websites/funnels, dedicated domains, and the client portal.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095809/original/82lhQooK-BZRhn3IMxjM7GcSDZbSWjjPNg.png?1717515282)

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095807/original/a8TzYf-3dnw-VbAwcvB557Klucd9jSYIRA.png?1717515282)

  
1) Now you open your DNS provider of choice and add the records in. Adding records are much the same, with some variation based on the provider. Go to your DNS manager and click add record.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095808/original/NeCo_2dJkC96cNq4SD_gjAtSvrk-e1PSEg.png?1717515282)

  
2) Select the record type provided by HighLevel

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095819/original/Mf13PeAVBfyHw2UVIcqy9npH7W7b2VFhmA.png?1717515282)

3) Input the Hostname into the “Name” field and Value/Target into the “target field”

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095817/original/c1IMDbugE355g-RMxp50EGWBTEHgDNHCuQ.png?1717515282)

4) Save the record. If utilizing Cloudflare the Proxy Status will need to be toggled off.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095821/original/4M9zVsq-xWiE6yTlyTBccTJRD7V3pRHMwQ.png?1717515282)

To learn more about this manual process, go [here](https://help.gohighlevel.com/support/solutions/articles/48001153720-how-to-set-up-root-domain-subdomain-for-your-funnels-websites-).

---

# Places to Add Domains to in HighLevel

Within HighLevel, there are many places to add a domain, let’s briefly explore each one. We will provide resources to learn more.
  
  
## Whitelabel Domain

Whitelabeling your desktop web app ensures that your customers interact with your domain instead of the default one. Simply follow four steps: create a CNAME in your DNS records, configure it in your HighLevel Agency account, upload your agency logo, and update your agency Terms & Conditions. Once your DNS record propagates, your customers 

can access the app using your domain, seeing your branding elements like logo and terms & conditions.

  
A sub-domain is Recommended for whitelabeling. Most Commonly agencies will use "app" as the sub-domain for their whitelabel desktop app.
  
  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095824/original/RYqwtTH5ELlsyMXglUGtprsoLu3EhJsF3A.png?1717515282)

_Navigate to the Agency View > Settings > Company Settings > Whitelabel Domain_

  
For more information on setting up your Whitelabel Domain please visit [How to Set Up a Whitelabel Domain](https://help.gohighlevel.com/support/solutions/articles/48000982207-how-to-set-up-a-whitelabel-domain-for-the-desktop-web-app)

---

## API or Branded Domain

Enhance your brand visibility and link deliverability by customizing system-generated links with our API/Branded Domains. By doing so, you can personalize links for forms, surveys, calendars, and more.

Custom API domains allow for branding of system-generated links, improving brand recognition and link deliverability. Configure API domains at the agency level company settings to establish a default branded domain for all sub-accounts.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095823/original/Ft7JzHK2yiJeQfqbYizWpfp41evuZq2edQ.png?1717515282)

_Navigate to the Agency View > Settings > Company Settings > API Domain_

  
At the sub-account level to customize domains for individual clients a branded domain can be set up. This will be done under the sub-account settings, within the business profile.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095816/original/4VyHIMkwNpESs9yMBEBVy-jAHxNIO0EG6A.png?1717515282)

_Navigate to the Sub-Account > Settings > Business Profile > API Domain_

  
For more information on the API/Branded Domain setup please view [How to Configure Brand System Generated Links](https://help.gohighlevel.com/support/solutions/articles/48001143244-how-to-configure-brand-system-generated-links-api-domain-)

For both the API and Branded Domains, utilize a sub-domain as utilizing a root domain here will cause your domain to point away from your website.

  
---

## Sites (Settings > Domains)

Integrating a domain into your account unlocks the potential for website and funnel functionalities. This guide will offer a thorough walkthrough for manually configuring domains, covering essential steps like DNS setup, domain association with sub-accounts, and troubleshooting common issues like SSL errors and 404 errors. 

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095830/original/eSAldtQTlORLqsoMGuuptYJI9sCEsD6evg.png?1717515282)

_Navigate to the Sub-Account > Settings > Domains_

  
For more information on how to add a domain to a website please visit [How to Set Up a Root/Subdomain for Your Funnels/Websites](https://help.gohighlevel.com/support/solutions/articles/48001153720-how-to-set-up-root-domain-subdomain-for-your-funnels-websites-)

---

## Email Sending Domain

To maximize email marketing impact, prioritize sender reputation and deliverability. A dedicated sending domain in the LC Email system gives you control over email communications, enhancing brand credibility and reducing spam filter risks. This setup is ideal for customized notification emails and targeting specific categories, ensuring efficient delivery. To avoid conflicts with existing email services, configure your dedicated domain using a subdomain. Dedicated sending domains are key to maintaining a positive sender reputation and achieving effective email marketing with LC Email.

* Add additional MX Record

Some Domain Host Such as Google Domains require can only have one MX record pointing towards a domain. In cases such as this there may be an option within the domain registry to add an additional record where you will need to include the second value.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095829/original/hcq0UeChnG-9hDKlXxqS5zYyMdjHmZ4xNA.png?1717515282)

_For agency level email services navigate to the Agency View > Settings > Email Services > Dedicated domain_

  
_For sub-account level email services navigate to the Sub-Account > Settings > Email Services > Dedicated Domain_

  
For more information the Dedicated Email Sending Domain setup process please visit [How to Set Up a Dedicated Sending Domain](https://help.gohighlevel.com/support/solutions/articles/48001226115-how-to-set-up-a-dedicated-sending-domain-lc-email-)

  
---

## Client Portal Domain (Communities, Courses)

  
The client portal transforms client-business interactions by providing a secure, centralized platform in HighLevel for your Affiliates, Membership and Community management. The portal functions as a dynamic interface, centralizing affiliate manager commissions, community interactions, and membership course activity. It simplifies client engagement with custom domains and branding options, reinforcing brand-client relationships. Enhanced communication and client autonomy lead to greater satisfaction and loyalty.

  
This document guides you through setting up and customizing the portal to meet specific business needs, enabling clients to take autonomous actions.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095828/original/pE8FkmSirGnzByVygxv8KkZ-ogkjwzVFcw.png?1717515282)

_Navigate to the Sub-Account > Sites > ClientPortal > API Domain_

  
For more information on the Client Portal Setup please visit [How to Set Up the Client Portal](https://help.gohighlevel.com/support/solutions/articles/155000000193-how-to-set-up-the-client-portal-)

---

## WordPress

WordPress Hosting allows for the migration of an existing WordPress site, or for a new site to be created. After connecting the domain, users gain access to essential features like the WordPress Dashboard, User Management, Backup & Restore, and Advanced Settings. 

  
Whether users are starting a new website or managing existing ones, this guide provides valuable instructions and insights to streamline the WordPress setup process effectively for your clients.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095831/original/xBtwh9LbbbyeTDtR7LOC2Tjixy-NKbmPwg.png?1717515282)

_Navigate to Sub-Account > Sites > Wordpress > Add Domain_

  
For more information on Wordpress Domain setup please visit [Getting Started With Wordpress Client Side Setup Guide](https://help.gohighlevel.com/support/solutions/articles/48001199648-getting-started-with-wordpress-client-side-setup-guide)

---

# Domain Glossary - Key Words to Know

  
| | Example                    | Description                                                                                                                                                  |                                                                                                                                                                                                 |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Domain                       | www.gohighlevel.com                                                                                                                                          | The digital address for online services like websites, email hosting, and more                                                                                                                  |
| Root Domain                  | gohighlevel.com                                                                                                                                              | The primary address of your website, appearing after "www." in a URL (e.g., in "www.gohighlevel.com," the root domain is "gohighlevel.com"). It serves as the main entry point to your website. |
| Subdomain                    | help.gohighlevel.com                                                                                                                                         | Subdomains are extensions of your root domain, directing users to specific sections or areas within your online infrastructure (e.g., "help.domain.com" for support).                           |
| Hostname                     | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095813/original/_yK4XozIWht9RuVCgkZPZLj2RS-PgXlVxA.png?1717515282) | The name/value utilized in the record, typically the subdomain utilized. This is what allows subdomains such as “help.gohighlevel.com” to act independently from “www.highlevel.com”            |
| Data/Target/Value            | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095812/original/vLgs8iDxu5UEvVPjhHmwDc0COPb0G20twQ.png?1717515282) | The value which tells the URL to display intended website data.                                                                                                                                 |
| Nameservers                  | GoDaddy, Cloudflare, Google, etc.                                                                                                                            | The directory which organizes and controls the DNS records. This is what tells the internet which Domain Provider, e.g. Godaddy, Cloudflare, etc, is controlling the Domain                     |
| DNS (Dedicated Name Servers) | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095815/original/OK0coxwyfKCwvT4GTuhBhFWJm35KSh-OuA.png?1717515282) | The records that tell the internet when a certain URL is visited to populate a website, and allows email providers to send emails from the domain name.                                         |
| TXT                          | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095810/original/XgKktnkym29TrLhZdbDE9ZUxHWtMd3m0OQ.png?1717515282) | TXT records are used for sending emails to prevent spam, and for protecting the domain by creating a domain verification.                                                                       |
| MX                           | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095814/original/3rDvCDQP1_qG-XwtVojf_EOOmjQXYj39bA.png?1717515282) | The Mail Exchange (MX) records tell emails where to be routed to. This is utilized to send and receive emails within HighLevel.                                                                 |
| CNAME                        | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095811/original/8cdtZ17kqkLPdZnKQMkBwVtW08YLYykVPg.png?1717515282) | A Cname record points to another domain. These records are commonly utilized when creating sub-domains                                                                                          |
| A Record                     | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095818/original/Euay6ddSoczuJvgIyaQABt4wvVqK5JNtKA.png?1717515282) | An A record points to an IP address that is hosting your website. These records are commonly utilized for your root domain to point to your primary website.                                    |
| DMARC                        | ![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095820/original/vBdK9jdlUVOa9fmp-DSBENEfTwdHxgN5zQ.png?1717515282) | A DMARC record is a TXT record that prevents email spoofing protecting your email sending from scammers and unauthorized use of the domain.                                                     |

---

# Troubleshooting

If you've added DNS records to your domain provider but are encountering issues like web pages returning 404 errors, there are a few key troubleshooting steps to consider. 

  
[1\. Check for Duplicate A Records:](#1.-Check-for-Duplicate-A-Records%3A)

[2\. Confirm DNS Propagation](#2.-Confirm-DNS-Propagation)

[3\. Review DNS Settings for Accuracy:](#3.-Review-DNS-Settings-for-Accuracy%3A)

[4\. Verify Domain DNS Integration:](#4.-Verify-Domain-DNS-Integration%3A)

[5\. Consider Other Potential Causes:](#5.-Consider-Other-Potential-Causes%3A)

[6\. Seek Additional Assistance:](#6.-Seek-Additional-Assistance%3A)

  
## 1\. Check for Duplicate A Records:

* Ensure there are no duplicate A records pointing to the root domain in your domain provider's configuration.
* Look for records with "@" as the hostname, indicating a root domain A record.
* If duplicate A records are found, correct them to avoid conflicts that might cause 404 errors.
* Ensure each A record points to the correct data specified by HighLevel. “162.159.140.166”

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095822/original/fzteelSehDWQRuQRBoCJ8NShRCo_CzBZSg.png?1717515282)![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095825/original/6QbDBMiyo7tIMu965swGM7lF5NWrSK2eYg.png?1717515282)

## 2\. Confirm DNS Propagation

* Verify whether the DNS changes have fully propagated across the internet.
* DNS changes typically take between 24 to 48 hours to propagate, depending on factors like TTL, ISP, and domain provider systems.
* Utilize a DNS checker tool (https://dnschecker.org/) to monitor propagation status and identify any incomplete updates.

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095833/original/ptDUfOA6xIaBLBSFylW7K-V22mYLCb05YA.png?1717515283)

  
## 3\. Review DNS Settings for Accuracy:

* Double-check all DNS settings to ensure accuracy.
* Confirm that each DNS record points to the appropriate HighLevel value.

| **Domain Being Added**                                                                                                                                             | **Type**                                   | **Hostname**                                                                                                      | **Value**                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Funnels/Website Root Domain ](https://help.gohighlevel.com/support/solutions/articles/48001153720-how-to-set-up-root-domain-subdomain-for-your-funnels-websites-) | A                                          | **@**                                                                                                             | 162.159.140.166                                                                                                                                           |
| [Funnels/Website Subdomain ](https://help.gohighlevel.com/support/solutions/articles/48001153720-how-to-set-up-root-domain-subdomain-for-your-funnels-websites-)   | Cname                                      | Varies - “www.” & subdomain - “example”                                                                           | sites.ludicrous.cloud                                                                                                                                     |
| [Wordpress ](https://help.gohighlevel.com/support/solutions/articles/48001199648-getting-started-with-wordpress-client-side-setup-guide)                           | A - Root DomainCname - Subdomain           | Varies                                                                                                            | Varies                                                                                                                                                    |
| [Client Portal ](https://help.gohighlevel.com/support/solutions/articles/155000000193-how-to-set-up-the-client-portal-)                                            | Cname                                      | Subdomain - “memberships”                                                                                         | clientportal.ludicrous.cloud                                                                                                                              |
| [WhiteLabel](https://help.gohighlevel.com/support/solutions/articles/48000982207-how-to-set-up-a-whitelabel-domain-for-the-desktop-web-app)                        | Cname                                      | Subdomain - “App.”                                                                                                | whitelabel.ludicrous.cloud                                                                                                                                |
| [API Domain/Branded Domain ](https://help.gohighlevel.com/support/solutions/articles/48001143244-how-to-configure-brand-system-generated-links-api-domain-)        | Cname                                      | Sub-domain - “link”                                                                                               | brand.ludicrous.cloud                                                                                                                                     |
| [Dedicated Email ](https://help.gohighlevel.com/support/solutions/articles/48001226115-how-to-set-up-a-dedicated-sending-domain-lc-email-)                         | 1st TXT2nd TXTCname1st MX2nd MXTXT - DMARC | VariesSubdomain used“example”Uses Subdomain - “email.example”Subdomain used“example”Subdomain used“example”Varies | 1st TXT - Varies2nd TXT - v=spf1 include:mailgun.org \~allCname - mailgun.org1st MX - mxa.mailgun.org2nd MX - mxa.mailgun.orgDmarc TXT - v=DMARC1;p=none; |

## 4\. Verify Domain DNS Integration:

* Ensure that the domain DNS records were correctly added to the provider where the domain Nameservers are pointing.
* If the Nameservers are managed by a different provider, integrate the HighLevel records into the DNS of that provider.
* Utilize a MX checker (https://mxtoolbox.com/) to verify the Hosting provider and that the records are propagating the correct data.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095832/original/XUOU0QHgW-hgcx7vZ--VGvfw0m0NCmfhig.png?1717515282)

  
## 5\. Consider Other Potential Causes:

* If the issue persists, explore other potential causes such as server downtime or incorrect domain configurations.
* Investigate any recent changes or updates that might have impacted the DNS settings.

  
## 6\. Seek Additional Assistance:

* If troubleshooting steps do not resolve the issue, consider reaching out to your domain provider's support team for further assistance.
* Alternatively, contact HighLevel support for specialized help in resolving DNS-related issues.

---

# FAQ

## What If I do not have a domain?

You can purchase a domain from a domain registrar such as Godaddy, Cloudflare, Namecheap, Google Domains if you do not currently own a domain. Once purchased this will allow you to proceed to set up the domain within HighLevel

  
## Can I use an existing domain for my email?

You can set up a dedicated domain for an existing domain. It is advised to utilize a sub-domain when setting up your domain for email sending within HighLevel to prevent it from affecting your current email services. 

  
## Can I use WIX for my Dedicated Domain?

Wix does not allow for multiple MX records to be added of the same priority. In order to use a domain that is connected to Wix the nameservers will need to be changed to point to another domain host. For more information please see: [LC Email / Mailgun replies not working when using WIX as the domain provider](https://help.gohighlevel.com/support/solutions/articles/48001188738-lc-email-mailgun-replies-not-working-when-using-wix-as-the-domain-provider)

  
## My Cname record is not being recognized in Cloudflare.

Make sure the Cname record that is added into Cloudflare has the proxy toggled off in order to allow the record to propagate. 

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155027095826/original/MFQYCch3__QKBwKhSpCrSniblWBKnpgYCA.png?1717515282)

  
## What if I have an existing domain?

If you have an existing domain, Great! If you currently have an existing website connected to that domain and are not wanting to replace it with a HighLevel website/funnel we can utilize a sub-domain to connect your domain to our funnels so that we could get this to act independently
  
  
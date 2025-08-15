**Date Updated:** 2023-07-27T23:04:43.000Z

Where did you get the domain for WIX?

  
You will need to follow this article in order to set up your nameservers so they are not managed by WIX.

<https://support.wix.com/en/article/dns-records-needed-to-connect-your-domain-to-wix>

  
**Change** the nameservers here:

  
[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619872/original/B8A4v0q6PZ5YHsAp2mzk6_scZOWKWvgpuA.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048676561/original/YR0RErgqA3H6yrlCTXhhZbT3%5Fwiy8RMiLg.png?1594407818)

  
And then choose **I will use GoDaddy Nameservers**

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619871/original/leZXxFFitGVUL_wyqnukiQY8HewiiuhhkA.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048676558/original/c5-qSORu7yueJm6AQ9njZkWqb2793iw4NQ.png?1594407817)

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619867/original/xZMIopePhJIuQfvyI2d-FSmtfCGhaDamag.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048676749/original/O1cQxm9xOIXkrWlOOMVa6XthQtecaZmlSQ.png?1594407903)

  
Go to this article and copy the record here to add to your DNS records:

<https://support.wix.com/en/article/dns-records-needed-to-connect-your-domain-to-wix>

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619870/original/waEl3ZyYXtpTn3z8M1YI4SxEItlWK1-Z_g.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048677097/original/Nz7A2Pc9r7o6ifdDElkaDFxYb5GenehFlg.png?1594408059)

  
Hit Edit pencil button on the right

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619863/original/FcRU58EGiZKcns2K8ALxLueEHPfjdvaznA.png?1594935582)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048677230/original/sF5umzyoh6KeB%5FH7wBc055xK-5bx8F0Fdg.png?1594408105)

  
Paste the A record here:

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619868/original/f7c1M2IS1BJN60UZqO2J7yUctTOAlVNHcg.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048677378/original/7eVDwzLLsaC8fNs38La35DMKjtRtaGIzjQ.png?1594408151)
  
  
Edit the original CNAME record and Paste the wwwXX.wixdns.net record here:

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619869/original/MouLyh5lo5A1OLCtk6GsLHRX5O-8vMfaBg.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048678085/original/NgYbOPlEF2uAanqP9y07bHcteCHXA4buxQ.png?1594408436)

  
Go to <https://dnschecker.org/>

  
Put yourdomain.com (A record) and search to see if it's working:

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619864/original/mb1xaCvUJdDXFgow1RF-WpnHcGJYh2aTog.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048678312/original/RgvRn40F2j%5FhC6LaTJrhvhm9QtA0S4cN1w.png?1594408555)

  
Put [www.yourdomain.com](http://www.yourdomain.com/) (CNAME record) and search to see if it's working:

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619866/original/DrKok7JojxLYA6I4l4FBw6YDBT_Qt24NhA.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048678393/original/8LRWkWllhraLK1fb3e91NFVM3JV72ywzZg.png?1594408597)
  
  
Put yourdomain.com (NS record) and search to see if it's working:

[![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48049619865/original/R1d1SOWBIMaa6Rb2WNTr1ifPPeHnZjxj4g.png?1594935583)](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48048678590/original/vTmfShLRzSvkdM4pmRiTAIzWEU%5Flxcf0wg.png?1594408694)
  
  
Go to your website yourdomain.com and see if your website is working.

  
Now you can set up Mailgun in your domain provider's DNS records following these articles!

[Step-by-step guide to set up Mailgun](https://help.gohighlevel.com/en/support/solutions/articles/48001219824)

[How to Set Up a Dedicated Sending Domain (LC Email)](https://help.gohighlevel.com/en/support/solutions/articles/48001226115)
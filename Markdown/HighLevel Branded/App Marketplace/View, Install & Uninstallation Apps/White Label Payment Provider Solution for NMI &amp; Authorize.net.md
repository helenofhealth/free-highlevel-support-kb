**Date Updated:** 2024-10-07T17:35:54.000Z

We're thrilled to unveil our latest update, introducing support for White Label Payment (WLP) provider solution for both NMI and AuthorizeNet. This addition significantly enhances our platform's capabilities, allowing seamless integration with new payment providers built on top of native solutions like NMI and AuthorizeNet.

Enhanced User Experience with Integrated Marketplace Listings

To elevate the user experience to new heights, we've directly integrated marketplace app listings within the payment integration page. This means users can effortlessly discover and install any integration provider available through the marketplace. The page features a convenient search function, enabling users to quickly locate desired providers. Moreover, users can now install apps directly from the listing page, streamlining the process further.

How Does it Work?

Developers simply need to create a marketplace app categorised under White Label Payment Provider. Upon installation, the app automatically generates a provider configuration specific to the installing location. Once installed, users can manage connection properties just like any other native provider. Following configuration, users can designate the WLP provider as their default payment option and seamlessly utilize it, mirroring the functionality of NMI or AuthorizeNet.

Expanded Support

We're delighted to announce that the new WLP provider is supported across all platforms where NMI and AuthorizeNet have been available since day one. This includes order forms (both one-step and two-step), E-commerce stores, invoices, and payment links. :tada::tada:

Public API Support

In addition to the marketplace integration, we've also added support for two public APIs to the payment app list. This enables seamless integration with WLP solutions for NMI and AuthorizeNet, empowering developers to create even more robust payment experiences.

POST - payments/integrations/provider/whitelabel [here](https://highlevel.stoplight.io/docs/integrations/38fc7b49d107d-create-white-label-integration-provider)

GET - payments/integrations/provider/whitelabel [here](https://highlevel.stoplight.io/docs/integrations/cbdced5c59dfd-list-white-label-integration-providers)  
  
Refer for a detailed loom video for building and submitting the integration [here](https://www.loom.com/share/ca47b2b4a4e4441797482d07a1ce9232)

![Screenshot 2024-04-16 at 11](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155028671910/original/5b7NeJ12EHXLFRvS_UieNjqf4cM5vKrQ_Q.jpeg?1720041556)

![Screenshot 2024-04-17 at 10](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155028671909/original/NoFtjMQINWRiBJt6SnpNGCDDFXvPyRgTsw.jpeg?1720041556)

![Screenshot 2024-04-16 at 11](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155028671911/original/tiX0EP-N602vjB5NjFrQsjn3HnbaS0RIsw.jpeg?1720041556)

![Screenshot 2024-04-16 at 11](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155028671908/original/xxAsSytNVl_aDJZR5PFNbOJV-YwKFa5iFQ.jpeg?1720041556)
**Date Updated:** 2021-09-16T22:10:11.000Z

Chat widget offers many configurations through chat-widget builder but there are few configurations which we are not providing through chat-widget builder to keep it simple for most users and avoid complexity for most of the use cases, in this section we talk about configurations you can make in chat-widget code after copying from builder.

  
Let's assume the code below is the code you copied from builder. We can add new attributes to this code for advanced configuration.

  
```html
  <chat-widget
            style="--chat-widget-primary-color: #97C8A2; --chat-widget-active-color:#97C8A2"        
            location-id="hgHI41V5EbRCG*****">
    </chat-widget>
       <script src="https://widgets.leadconnectorhq.com/loader.js"
          data-resources-url="https://widgets.leadconnectorhq.com/chat-widget/loader.js" >
      </script>
```

HTML

  
### **Open-Icon-url**

This enables you to change the default message icon on chat-widget open button.

  
```html
 <chat-widget
            style="--chat-widget-primary-color: #97C8A2; --chat-widget-active-color:#97C8A2"        
            location-id="hgHI41V5EbRCG*****"
            open-icon-url="https://img.icons8.com/cotton/2x/blood-sample.png">
    </chat-widget>
       <script src="https://widgets.leadconnectorhq.com/loader.js"
          data-resources-url="https://widgets.leadconnectorhq.com/chat-widget/loader.js" >
      </script>
```

HTML

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48127183686/original/gwvRAPgzp_jm8-w5U7UhFz4kkpefUycwmw.png?1628085770)

### **Close-icon-url**

This enables you to change the default close icon on chat-widget close button.

  
```html
<chat-widget
            style="--chat-widget-primary-color: #97C8A2; --chat-widget-active-color:#97C8A2"        
            location-id="hgHI41V5EbRCG*****"
            close-icon-url="https://img.icons8.com/cotton/2x/blood-sample.png">
    </chat-widget>
       <script src="https://widgets.leadconnectorhq.com/loader.js"
          data-resources-url="https://widgets.leadconnectorhq.com/chat-widget/loader.js" >
      </script>
```

HTML

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48127184178/original/GsAwrDp0M-MLRTze103FditzRyzXXlkhFQ.png?1628085828)

  
### **Next-prompt-timer**

The next-prompt-timer determines the number of seconds the webchat widget will wait before showing the chat-bubble to a user when they revisit. The default value is 86400 sec (24 hours), meaning the prompt bubble will not be visible for 24 hours if a user closes the widget. To make chat-bubble visible upon every page visit, you would set its value to 0.

  
```html
  <chat-widget
            style="--chat-widget-primary-color: #97C8A2; --chat-widget-active-color:#97C8A2"        
            location-id="hgHI41V5EbRCG*****"
            next-prompt-timer="0">
    </chat-widget>
       <script src="https://widgets.leadconnectorhq.com/loader.js"
          data-resources-url="https://widgets.leadconnectorhq.com/chat-widget/loader.js" >
      </script>
```

HTML

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48127187894/original/UzMWDpr4xEnmapRsucaNV8pNABJikjDDKA.png?1628086231)

  
### **Server-u-r-l**

By default chat-widget will communicate (submit lead, etc.) with the server through this ([https://msgsndr.com](https://msgsndr.com/)) base URL, but you can use this attribute to communicate with different server. You would use this attribute for testing/debugging purposes.

  
```html
    <chat-widget
            style="--chat-widget-primary-color: #97C8A2; --chat-widget-active-color:#97C8A2"        
            location-id="hgHI41V5EbRCG*****"
            server-u-r-l="https://test-staging.com">
    </chat-widget>
       <script src="https://widgets.leadconnectorhq.com/loader.js"
          data-resources-url="https://widgets.leadconnectorhq.com/chat-widget/loader.js" >
      </script>
```

HTML

# Public API / Events

##   
APIs

1\. **openWidget**: This method will helps you to open widget programmatically from any other action items eg on button click

window.leadConnector.chatWidget.openWidget();

  
```html
var button = document.getElementById("myButton");
button.addEventListener("click",function(e){
    window.leadConnector.chatWidget.openWidget()
},false);

//HTML 
<button id='myButton'>Hello</button>
```

HTML

2\. **closeWidget**: This method will helps you to close widget programmatically from any other action items eg on button click

  
window.leadConnector.chatWidget.closeWidget()

  
```html
var button = document.getElementById("myButton");
button.addEventListener("click",function(e){
    window.leadConnector.chatWidget.closeWidget()
},false);

//HTML 
<button id='myButton'>Hello</button>
```

HTML

  
3\. **isActive()**: This api will return true if the widget is open(expanded) else return false if widget is closed(collapsed).

window.leadConnector.chatWidget.isActive()

  
```html
if(window.leadConnector.chatWidget.isActive()) {
  //do something CRAZY
}
else {
//stay silent
}

//HTML 
<button id='myButton'>Hello</button>
```

HTML

4\. **localizeWidget via API**: This code allows you to change widget labels after the widget gets loaded

  
```html
window.leadConnector.chatWidget.localizeWidget({"name": "Nombre"})
//this will change `Name` label to `Nombre`
//for complete list of supported labels refer to localization section
//ideally you should use the `i-1-8n-labels` attribute
```

HTML

![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/48128186151/original/jBqdi6nPz5ehvH768GIB07K31a76R86Krg.png?1628278617)

  
5\. **i18n: Internationalization** \- The chat widget does not have automatic i18n support based on i18n lang code but you can change any of the labels within the widget (refer below table for all labels) using attribute names.

  
```html
<chat-widget
      location-id="hgHI41V5EbRCGv*****"
      i-1-8n-labels='"{\"name\": \"nombre\", \"phone\": \"teléfono\"}"'>
</chat-widget>
```

HTML

| key            | default value(en-US) | Description                                           |
| -------------- | -------------------- | ----------------------------------------------------- |
| name           | Name                 | Name field label                                      |
| phone          | Mobile Phone         | Mobile input field label                              |
| email          | E-mail               | email input label                                     |
| message        | Message              | Message input field label                             |
| required       | Required             | error message for required fields                     |
| received       | Received             | acknowledgement label below your acknowledgement text |
| sending        | Sending              | visible when lead submission is in progress           |
| invalid\_value | Invalid value        | error message for invalid values in input fields      |
| send           | Send                 | Title of submit button                                |
| powered\_by    | Powered by           | Powered by text for agency branding                   |

##   

**Changing Widget Labels on Wordpress** \- Currently, there is not a way to change the chat widget labels in the WP LeadConnector plugin settings; however, you can add the following code to the footer of the Wordpress website that will change the labels after the widget loads.

```html
     <script>
window.addEventListener(
        'LC_chatWidgetLoaded',
        function (e) {
          window.leadConnector.chatWidget.localizeWidget({ 
              name: 'Nombre', 
              phone:'teléfono'
              //refer above table for more labels 
            });
        },
        false,
      );
</script>
```

HTML

  
If you're not comfortable adding the code into the footer, you can use a plugin like [Insert Headers And Footers](https://wordpress.org/plugins/insert-headers-and-footers/), which makes the process easy.

  
## Events

  
1\. **LC\_chatWidgetLoaded**: chat-widget will fire this event after it gets loaded completely on windows

  
```html
      window.addEventListener(
        'LC_chatWidgetLoaded',
        function (e) {
          console.log(e);
        },
        false,
      );
```

HTML

  
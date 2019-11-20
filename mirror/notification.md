# Describes how to use notifications

## For sending 
Call this when needed:
> ```self.sendNotification("MMM_MODULE_NAME", <payload (AnyObject)>);```

<b>Example</b>, send notification after 3sec (3000 milli):
> ```setTimeout(function(){self.sendNotification("MMM_TESTERONI_NOTIFICATION", "Joe Mama");}, 3000);```

## Receiving
```
Module.register("MMM_MODULE_NAME",{

    //...

    notificationReceived: function(notification, payload, sender) {
        var self = this
        if (sender) {
            if (notification=="MMM_MODULE_NAME") {
                self.config.text = "Notification was received: " + payload
                //self.updateDom() //if you want to update the UI
            }
        }     
    },

    //...
}
```

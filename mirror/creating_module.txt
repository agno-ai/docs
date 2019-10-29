#
# Creating a basic module 
#

1. Create folder in ~/MagicMirror/modules/ , e.g. "MMM-Testproject"
2. cd into "MMM-Testproject"
3. create MMM-Testproject.js
4. File should at least contain:
```
Module.register("MMM-Testproject",{

    // Default module config.
    defaults: {
        text: "Write some text here!"
    },

    // Override dom generator.
    getDom: function() {
        var wrapper = document.createElement("h1");
        wrapper.innerHTML = this.config.text;
        return wrapper;
    },

});
```
5. Add following code into ~/MagicMirror/config/config.js
```
{   
    module: 'MMM-Testproject',
    position: 'top_left',
    config: {}
}, 
```


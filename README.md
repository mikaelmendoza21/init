# init
A simple starter web app theme using vanilla CSS and OO Javascript. 
Mobile-first.
Made up of decoupled modules *init-CSS* (styling) and *init-js* (components) .


### Animated Classes
**Fade In classes**

* fadeIn

* delayedFade

### Javascript Components

* **Modal**

    A modal or "pop up" shown within the browser window.

    *Arguments*:  
    
    * title

    * content

    * modalContainerClasses

    * headerClasses

    * titleClasses

    * closeButtonClasses

    * closeButtonContainerClasses

    * contentClasses

    * onOpenCallback

    * onCloseCallback



    *Sample Initialization:*


    ```javascript
    
    var modal = new Modal({
                    
        // Modal Content

        title: 'Hello',

        content: 'This is a modal!', 
        

        // Styles classes (optional)

        modalContainerClasses: ['modal'],   

        headerClasses : ['modal-header'],

        titleClasses: ['modal-title'],

        closeButtonClasses: ['button close-modal-btn'],

        closeButtonContainerClasses: ['modal-close'],

        contentClasses: ['modal-content'],


        // Callback Functions

        onOpenCallback: openModalCallback,

        onCloseCallback: closeModalCallback
    });
    ```
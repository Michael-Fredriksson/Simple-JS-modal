# Simple JS modal
 A simple JS modal writen to get used to get more hands on and write more JS code as well as using Git rather than standalone coding.

 A basic modal made in JS 
 Sample code feel free to use it as you like.

 Modual is started by calling the open_mPop class.
 ```new open_mPop(args)```
 
 In order for the modal to show the first argument (modal body message) must be set.

### Modal arguments
 > message, header, type, url  

 ```open_mPop(message, head, type, url)```

 Message: -> str, any  
 Head: -> str, any  
 Type: -> arg, alert | info
 * alert change "confirm" button background color to the --modal_alert_bg color (Default RED)
 * info makes changes the modal to have a scrollable field and the close/confirm button(s) at the bottom is replaced by a close button at top right corner.  
 !-- note: If a url is passes the info parameter won't activate. --!  

 Url: -> str, any

### Modal colors
#### css/modal.css
 The modal uses @media (prefers-color-scheme: dark) | @media (prefers-color-scheme: light) to set the current color-scheme based on browser settings. If only one color-scheme should be used both must be changed to have the same values.  
 Alternative move/copy the preferred root: {} scheme to top hierarchy and comment out/remove @media (prefers-color-scheme: dark) | @media (prefers-color-scheme: light).

        --modal_bg: Modal background color
        --modal_color: Modal Text color
        --modal_button_bg: Default button background color
        --modal_button_color: Default button text color
        --modal_button_tshadow: Default button text shadow
        --modal_alert_bg: Alert button background color
        --modal_alert_color: Alert button text color
        --modal_alert_tshadow: Alert button text shadow
        --modal_confirm_bg: Confirm button background color
        --modal_confirm_color: Confirm button text color
        --modal_confirm_tshadow: Confirm button text shadow
        --mPop_close_bg: Info view close button background color;
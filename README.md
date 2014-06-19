ScrollToTOP
========

This simple project is used to create a button to the Scroll Top Page. 
This project was created with the languages ​​HTML5, CSS3 and JQuery. 
It is compatible with IE 6+, Google Chrome 1+, Firefox 1+, Safari 5.1+, Opera 12.1+ (http://jquery.com/browser-support/).
I am tested with JQuery 1.11.1.

## Installation

### Step 1 in ```<head></head>```

Include last [jQuery](http://ajax.googleapis.com/ajax/libs/jquery/1/jquery.min.js) 1.x and "stylesheet" scripts:
```html
<link rel="stylesheet" href="css/ScrollToTOP.css">
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1/jquery.min.js"></script>
```

### Step 2 in ```<head></head>``` or ```<body></body>```
```html
<!--Back to top-->
        <script type="text/javascript">
            // scroll-to-top button show and hide
            jQuery(document).ready(function () {
                jQuery(window).scroll(function () {
                    if (jQuery(this).scrollTop() > 100) {
                        jQuery('.scrollup').fadeIn();
                    } else {
                        jQuery('.scrollup').fadeOut();
                    }
                });
                // scroll-to-top animate
                jQuery('.scrollup').click(function () {
                    jQuery("html, body").animate({
                        scrollTop: 0
                    }, 600);
                    return false;
                });
            });
        </script>
```
### Step 3 in ```<body></body>```
```html
<a class="scrollup" href="#"></a>
```



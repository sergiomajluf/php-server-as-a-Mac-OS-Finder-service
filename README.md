# PHP Server as a Mac OS Finderservice

This Apple Script launches a PHP webserver by right clicking on a folder in Mac Finder.

You can install it using Automator as a service into Finder, then run it with a right click. It will launch a terminal window, and run:
` php -S localhost:8080`

If the port is taken, it increments it by one until the next available one.

The original script was developed by [Scott Garner](http://www.scottmadethis.net/interactive/simpleserver/) to use python SimpleHTTPServer. I just modded it to run PHP.

# Download
To use, just [download this file](https://github.com/sergiomajluf/php-server-as-a-Mac-OS-Finder-service/raw/master/My%20PHP%20Server.workflow.zip), then double click and let Automator install it in the appropiate folder (~Library/Services)

Next, go to the folder you want to serve, rigth click, and select PHP Server, like in the following image

![alt tag](https://github.com/sergiomajluf/php-server-as-a-Mac-OS-Finder-service/blob/master/simple-php-server.png)

This will start the server and open your default browser to the proper local URL and port.

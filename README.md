# PHP Server as a Mac OS Finderservice

This is an Apple Script that you install using Automator as a service into Finder.
Just navigate to the folder of your choice, right click and select the Server. 

It will launch a terminal window, and run:
` php -S localhost:8080
`
If the port is taken, it increments by one until the next available one.

The original script was developed by [Scott Garner](http://www.scottmadethis.net/interactive/simpleserver/) to use python SimpleHTTPServer. I just modded it to run PHP

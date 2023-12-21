# GoPhish-Microsoft-Login
A fake Microsoft login page optimized for GoPhish campaigns

This is a copy of the Microsoft login page created by [@Octagon-simon](https://github.com/Octagon-simon).

My version uses an updated index.html and app.jss.

The username and password are copied to a new form which then lets the final button submit the data to your GoPhish instance.
Regex is added for checking if an email address is valid.
You can use the Enter key after writting your username or password.

To use this with GoPhish simply copy the html to a new landing page template.
All of the other files need to be located on your server running GoPhish.

Under the directory where your GoPhish instance is located you'll find the directory \static\endpoint\ in there you need to create a new directory called "microsoftAssets":
...\<YOUR-GOPHISH-INSTANCE-DIRECTORY>\static\endpoint\microsoftAssets

In there copy all the files except the index.html.

These files are referenced in the index.html file using for example: href="http://localhost/static/microsoftAssets/app.css".

So you need to change "localhost" to the domain or IP on which your GoPhish server is hosted!

![alt text](https://github.com/jole583/GoPhish-Microsoft-Login/blob/main/previewGIF.gif)

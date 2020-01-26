# Creating your first site with HTML and CSS and how to open it in the browser
Type out all of the commands I give you below and follow the steps. **Do not get used to copying and pasting!**


### 1. Open Command Prompt(PC) or Terminal(Mac)

### 2. Run this command to see what folders/files you already have 
Get in the habit of doing this often.

```ls```

### 3. Create a "dev" folder
This is where you will keep everyting you create from now on.

```mkdir dev```

### 4. Run this command again.
You can see that the folder "dev" that you just created is visible and created.

```ls```

### 5. Now lets go into your "dev" folder.

```cd dev```

### 6. Create a new folder for this project.
You can name this whatever you want, just make sure it follows these naming rules:
1. The name always has to start with a lower case letter and **never** a number.
2. If the name is more than one word the words can be seperated by a a dash(-) or following the (n)ew(F)older naming style(example: helloWorld, newSite, firstSite, myFirstWebsite, hello-world, new-site, my-first-website).
__The most common is probably the newFolder naming style.__

```mkdir yourFolderName```

### 7. You can see this created now!

```ls```

### 8. Go into your new folder

```cd yourFolderName```

### 9. Create two files (HTML & CSS)
Side Note: You can always run commands in the same line seperated by a space, or you can run them seperately.

```touch index.html```
```touch style.css```

or

```touch index.html style.css```

### 10. You can see these created now!

```ls```

### 11. Now that the files are created you can open them in the IDE and in your folders
Running this command will open them in your folders.

```open .```

Running this command will open them in your IDE(text editor).

```code .```

__You don't really need the folder and files open in your computer's main folder organizer so you can go ahead and close that, I just wanted you to see that you can open it through Command Prompt or Terminal.__

### 12. Now that your files are opened in VS Code, create your HTML boilerplate in your HTML file.

```
<!DOCTYPE html>
<html>
<!--the 'head' of an HTML file will never be seen when you open the browser. Note that this is different than a 'header' which will be seen! The 'header' will live inside the body.-->
  <head>
    <meta charset="UTF-8">
    <title>title</title>
    <!--This is a comment tag. You can add comments anywhere in your code by using the these symbols on each end. -->
  </head>
  <body>
    <!--this is where your header will go.-->
    <!--this is where your photo will go.-->
    <!--this is where your paragraph will go.-->
    <!--this is where your link will go.-->
  </body>
</html>
```

### 13. Add a Title, Header, Photo, Paragraph (using lorem), and a Link in your HTML file.

```
<!DOCTYPE html>
<html>
<!--the 'head' of an HTML file will never be seen when you open the browser. Note that this is different than a 'header' which will be seen! The 'header' will live inside the body-->
<head>
  <meta charset="UTF-8">
  <title>title</title>
  <!--This is a comment tag. You can add comments anywhere in your code by using the these symbols on each end. -->
  <!--The title can be named whatever you want. Go ahead and change that! It will usually be titled whatever you titled your folder for this site. It doesn't have to follow the naming style so feel free to type it out normally (example: My First Site).-->
  <link rel="stylesheet" href="style.css">
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
</head>
<body>
  <div>
    <div class='navigation'>
      <h1>My First Site</h1>
      <!--Feel free to edit the text of the header inside of the header tags.-->
      <h4>Created by firstName lastName</h4>
    </div>
    <div class="card d-flex align-items-center justify-content-center" style="width: 45rem;">
      <img class="card-img-top" src="https://scontent-ort2-1.xx.fbcdn.net/v/t1.0-9/83268935_10212714463014695_726989335869521920_n.jpg?_nc_cat=101&_nc_oc=AQnPegnf1FElhMoaybjLfaV5ymTMkf16FzMuICyM1DplEYU1qAv4SRLjzsu7U4yzotqpfnrwRYgQSgL8Eoz0ZeNP&_nc_ht=scontent-ort2-1.xx&oh=eb91e289e1fb452907e7196ac52bfada&oe=5ED2B8AA" alt="">
      <!--the 'alt' attribute is used for when the image doesn't load and still allows the user to know what the photo would have been. This is also used for if the user is blind and is using a website reader to read to them. You always have to include an 'alt' attribute but you can leave it blank. The image tag <img> won't work without the 'alt' attribute. -->
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
      <!--'Lorem' is example text to fill in paragraphs. It is used a lot in coding so that you can fill and style a paragraph without having to spend the time writing your own paragraphs. There are lorem generators like this https://loremipsum.io/ -->
      <!--example hyperlink tag<a href="url">link text</a>-->
      <!--hyperlink tags will redirect the current tab. If you want the link to open in a seperate tag add target="_blank" inside of your <a> tag.-->
      <a href="https://www.facebook.com/reid.kennison" class="btn btn-primary" target="_blank">My Facebook Profile</a>
    </div>
  </div>
</body>
</html>
```
### 14. Open your new site in your browser through Command Prompt or Terminal.
Make sure your default broswer is set to Chrome.

```open index.html```

### 15. Link your CSS file in your HTML.
Add this code on the line right before your closing </head> tag. This will link your CSS file to your HTML file.

```<link rel="stylesheet" href="style.css">```

### 16. In your CSS file, add this styling. 

```
.navigation {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: 20px;
}

body > div > .card {
    display: flex;
    margin: 0 auto;
    margin-bottom: 100px;
}

.card > p {
    padding: 20px;
}
```

### 17. Refresh your website in Chrome.
You should see the styling changes made to your website!

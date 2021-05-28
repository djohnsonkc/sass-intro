# Sass Intro

Sample project for learning the basics of Sass

This video was the inspiration for this sample project.
https://www.youtube.com/watch?v=Zz6eOVaaelI


## These are the VS Code Extensions you will want to add

- Live Server - This allows you to right-click on your index.html file and run it in your browser
- Live Sass Compiler - This will watch for changes in your Sass .scss file and compile it to a .css file

## These are the concepts covered in the tutorial

- Variables
- Imports
- Nesting
- Mixins
- Inheritance
  
## These are the steps used in creating this sample project that I documented from his very helpful Youtube video

- Create a new empty project folder and add a new index.html file to the root
- In Terminal, run 'npm init' to create a package.json file
- Create a /styles folder with a styles.ccss (not .css) file and beging writing some CSS
- Click the 'Watch CSS' option in the lower-right corner of VS Code to watch for live changes, which will generate the styles.css file
- Link the styles.css file in your index.html page
- Right-click on index.html and select 'Live Server' to see you changes in real time


## Change the output directory

To help organize your styles, this will generate a ./dist folder in the root of your project.

Go to VScode menu- File > Preferences > Settings > Extensions > Live Sass Compile... > Edit in settings.json

Paste this into settings.json to dictate the output directory and minify the final css file:

"liveSassCompile.settings.formats": [
    {
      "format": "compressed",
      "extensionName": ".min.css",
      "savePath": "~/../dist/css/"
    }
]

Make sure and change your index.html file's link to your output style sheet
<link rel="stylesheet" href="./dist/css/styles.min.css">



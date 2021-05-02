![](https://cdn.glitch.com/5b29fefa-b38c-4c05-8f15-47cd7f21fd6a%2FScreenshot%202021-01-28%20at%204.06.26%20PM.png?v=1611930143656)


An open-source Android VM inside your browser that is made with Browserling scripts. 

This was originally meant for only Android Nougat (7.1), but I decided to expand it to many Android versions.

# Dependencies included in Nougat script
- jQuery
- socket.io

# How do I use Nougat?
To use Nougat, simply use this line of code:


`nougat.launch('#AnElementId, .AnElementClass, AnElement', 'android.version.here', 'url here (if none wanted simply put none)' center canvas: true/false, clear dom before load: true/false);`

To get the canvas element, use this:

```
nougat.getCanvas()
```

You can take screenshots too with:

```
nougat.generateScreenshotURL();
```

It will return a DataURL, and you can use it to make images like this:

```
var im=new Image();

nougat.launch('#mydisplay', '7.1', 'https://google.com', false, true);

setTimeout(function(){
im.src=nougat.generateScreenshotURL();
document.appendChild(im)
}, 5000);
```

The entire HTML code would be this:
```
<!DOCTYPE HTML>
<html>
  <head>
  </head>
  <body>
   <h1> Android in your browser! </h1>
  <p>This is a JavaScript library that embeds Android in your browser. (Nougat) </p>
    <button onclick="nougat.launch('#display', '7.1', 'https://google.com', true, true);">Launch Nougat!</button>
    <div id="display"></div>
        <script src="nougat.js"></script>
 </body>
</html>
```
# Demos of Nougat
Here is a screenshot of Nougat:
![](https://cdn.glitch.com/5b29fefa-b38c-4c05-8f15-47cd7f21fd6a%2FScreenshot%202021-01-26%20at%206.49.03%20PM.png?v=1611708575415)
And if you want to try Nougat yourself, here's the link to the project.

### [Demo Link](https://unzor.github.io/Nougat)

# All existing versions in Nougat:
7.1 - Android Nougat

7.0 - Android Nougat

6.0 - Android Marshmallow

5.1 - Android Lollipop

5.0 - Android Lollipop

4.4 - Android KitKat



## Code for all existing versions in Nougat:

`nougat.launch('#elementid', '7.1', url, true/false, true/false);` - Android Nougat

`nougat.launch('#elementid', '7.0', url, true/false, true/false);` - Android Nougat

`nougat.launch('#elementid', '6.0', url, true/false, true/false);` - Android Marshmallow

`nougat.launch('#elementid', '5.1', url, true/false, true/false);` - Android Lollipop

`nougat.launch('#elementid', '5.0', url, true/false, true/false);` - Android Lollipop

`nougat.launch('#elementid', '4.4', url, true/false, true/false);` - Android KitKat


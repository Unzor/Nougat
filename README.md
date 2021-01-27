# Nougat
An open-source Android VM inside your browser that is made with Browserling scripts. 

This was originally meant for only Android Nougat (7.1), but I decided to expand it to many Android versions.

# How do I use Nougat?
To use Nougat, simply use this line of code:


`nougat.launch('#AnElementId, .AnElementClass, AnElement', 'android.version.here');`



The entire HTML code would be this:
```
<!DOCTYPE HTML>
<html>
  <head>
  </head>
  <body>
   <h1> Android in your browser! </h1>
  <p>This is a JavaScript library that embeds Android in your browser. (Nougat) </p>
    <button onclick="nougat.launch('#display', '7.1');">Launch Nougat!</button>
    <div id="display"></div>
        <script src="nougat.js"></script>
 </body>
</html>
```
# Demos of Nougat
Here is a screenshot of Nougat:
![](https://cdn.glitch.com/5b277599-a348-4276-93be-3eb331552a51%2FScreenshot%202021-01-26%20at%201.24.27%20PM.png)
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

`nougat.launch('#display', '7.1');` - Android Nougat

`nougat.launch('#display', '7.0');` - Android Nougat

`nougat.launch('#display', '6.0');` - Android Marshmallow

`nougat.launch('#display', '5.1');` - Android Lollipop

`nougat.launch('#display', '5.0');` - Android Lollipop

`nougat.launch('#display', '4.4');` - Android KitKat


# Ex-7: Interactive Image Gallery
## Date: 06-11-2024

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:

### index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div id="image">Hover over an image below to display here.</div>
    
    <div class="gallery">
        <img class = "preview" alt = "Night Sky" src = "https://images.pexels.com/photos/1624496/pexels-photo-1624496.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" alt = "Rose" src = "https://images.pexels.com/photos/736230/pexels-photo-736230.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" src = "https://images.pexels.com/photos/2130610/pexels-photo-2130610.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt = "Paris" onmouseover = "upDate(this)" onmouseout = "unDo()">
        <img class = "preview" alt = "Turtle" src = "https://images.pexels.com/photos/5277693/pexels-photo-5277693.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" alt = "Cute Puppy" src = "https://images.pexels.com/photos/3687770/pexels-photo-3687770.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" onmouseover = "upDate(this)" onmouseout = "unDo()">
	    <img class = "preview" src = "https://images.pexels.com/photos/1648377/pexels-photo-1648377.jpeg?auto=compress&cs=tinysrgb&w=600" alt = "Baby" onmouseover = "upDate(this)" onmouseout = "unDo()">
    </div>
    <script src="script.js"></script>
</body>
</html>
```

### gallery.css
```
body{
    margin: 2%;
    border: 1px solid black;
    background-color: #b3b3b3;
}
#image{
line-height:650px;
    width: 575px;
height: 650px;
    border:5px solid black;
    margin:0 auto;
background-color: #8e68ff;
background-image: url('');
background-repeat: no-repeat;
color:#FFFFFF;
text-align: center;
background-size: 100%;
margin-bottom:25px;
font-size: 150%;
}
.preview{
    width:10%;
    margin-left:17%;
border: 10px solid black;
}
img{
    width:95%;
}
```

### gallery.js
```
// Reference to the image container
const imageDiv = document.getElementById('image');
const originalImageUrl = ''; // Set this to the URL of your original image
const originalText = "Hover over an image below to display here."; // Original text

function upDate(previewPic) {
    // Change the background image to the source of the hovered image
    imageDiv.style.backgroundImage = `url('${previewPic.src}')`;
    
    // Update the text to the alt text of the hovered image
    imageDiv.innerHTML = previewPic.alt;
}

function unDo() {
    // Reset the background image to the original URL
    imageDiv.style.backgroundImage = `url('${originalImageUrl}')`; // Use the original image URL here
    
    // Change the text back to the original text
    imageDiv.innerHTML = originalText;
}
```
## WEBSITE URL
```
https://codepen.io/Vishwa-Raja-the-sasster/pen/vYozPNy

```
## OUTPUT:

![Screenshot (577)](https://github.com/user-attachments/assets/5286fc72-9884-4922-abc8-a172a82a0c67)
![Screenshot (574)](https://github.com/user-attachments/assets/4d8e25fe-56e4-449d-9b35-c1fb5abc8196)
![Screenshot (576)](https://github.com/user-attachments/assets/aabe2aed-cc7a-409f-a4a5-d261919f0ba6)
![Screenshot (575)](https://github.com/user-attachments/assets/a38c511b-e50c-4e63-9f99-ac1b6716ddb3)

## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.

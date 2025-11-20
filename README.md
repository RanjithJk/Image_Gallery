# Ex.08 Design of Interactive Image Gallery

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Interactive Image Gallery</title>
  <style>
    body {
      margin: 0;
      padding: 30px;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #e71135, #6C7293);
      text-align: center;
    }

    h1 {
      color: #FFF;
      margin-bottom: 20px;
      font-size: 2.5rem;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      max-width: 1200px;
      margin: auto;
    }

    .gallery img {
      width: 180px;
      height: 180px;
      object-fit: cover;
      border-radius: 50%;
      box-shadow: 0 8px 20px rgba(235, 13, 13, 0.2);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      cursor: pointer;
    }

    .gallery img:hover {
      transform: scale(1.05);
      box-shadow: 0 12px 25px rgba(0, 0, 0, 0.3);
    }

    .lightbox {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.85);
      justify-content: center;
      align-items: center;
      z-index: 1000;
    }

    .lightbox img {
      max-width: 90%;
      max-height: 80%;
      border-radius: 10px;
      box-shadow: 0 0 30px #000;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    .footer {
      margin-top: 40px;
      color: #FFF;
      font-weight: bold;
      font-size: 1.1rem;
    }
  </style>
</head>
<body>

  <h1><i><b><u>CAR LINES IMAGE GALLERY</u> </b></i></h1><br><br>

  <div class="gallery">
    <img src="c:\Users\admin\Downloads\160229151906-bugatti-chiron-black-780x439.jpg" alt="car  image 1">
    <img src="c:\Users\admin\Downloads\muscle-cars-pictures-2560-x-1600-5fegcjboutymj74l.jpg" alt="car image 2">
    <img src="c:\Users\admin\Downloads\ss.jpg" alt="car image 3 ">
    <img src="c:\Users\admin\Downloads\car.webp" alt="car image 4">
    <img src="c:\Users\admin\Downloads\ferrari-sf90-stradale.jpg" alt="car Image 5">
    <img src="c:\Users\admin\Downloads\listing_main_Bugatti-La_Voiture_Noire-2019-1280-02.jpg" alt="car Image 6">
    <img src="c:\Users\admin\Downloads\images (1).jpg" alt="car Image 7">
    <img src="c:\Users\admin\Downloads\car.jpg" alt="car Image 8">
  </div>

  <div class="lightbox" id="lightbox">
    <img id="lightbox-img" src="" alt="Full View">
  </div>

  <div class="footer">
    <br><i>NAME: RANJITH JK<br>
 REG NO:   212224230221</i>
  </div>

  <script>
    const lightbox = document.getElementById('lightbox');
    const lightboxImg = document.getElementById('lightbox-img');
    const galleryImgs = document.querySelectorAll('.gallery img');

    galleryImgs.forEach(img => {
      img.addEventListener('click', () => {
        lightboxImg.src = img.src;
        lightbox.style.display = 'flex';
      });
    });

    lightbox.addEventListener('click', () => {
      lightbox.style.display = 'none';
    });
  </script>

</body>
</html>
```

## OUTPUT
<img width="1918" height="1017" alt="image" src="https://github.com/user-attachments/assets/1a3f1dac-0756-4c79-9946-4e76475934e8" />
<img width="1917" height="983" alt="image" src="https://github.com/user-attachments/assets/c3b59145-5476-43fa-9ff1-901d0b489b71" />


## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.

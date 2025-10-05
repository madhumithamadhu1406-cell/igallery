# Ex.08 Design of Interactive Image Gallery
## Date:05/10/2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```

<html lang="en">
<head>
    <meta charset="UTF-8">
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f3f3f3;
            text-align: center;
            padding: 20px;
        }

        h1 {
            color: #333;
        }

        #searchInput {
            padding: 10px;
            width: 300px;
            font-size: 16px;
            margin-bottom: 20px;
            border: 1px solid #ccc;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .photo {
            margin: 10px;
            border: 2px solid #ddd;
            padding: 10px;
            background-color: white;
            transition: transform 0.3s;
        }

        .photo:hover {
            transform: scale(1.05);
            border-color: #888;
        }

        .photo img {
            max-width: 200px;
            max-height: 200px;
        }

        .caption {
            margin-top: 8px;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <h1>MADHUMITHA V (25016067)</h1>
    <div class="gallery" id="photoGallery">
        <div class="photo">
            <img src="photo1.jpg" alt="photo1">
            <div class="caption">photo1</div>
        </div>
        <div class="photo">
            <img src="photo2.jpg" alt="photo2">
            <div class="caption">photo2</div>
        </div>
        <div class="photo">
            <img src="photo3.jpg" alt="photo3">
            <div class="caption">photo3</div>
        </div>
        <div class="photo">
            <img src="photo4.jpg" alt="photo4">
            <div class="caption">photo4</div>
        </div>
        <div class="photo">
            <img src="photo5.jpg" alt="photo5">
            <div class="caption">photo5</div>
        </div>
    </div>

    <script>
        function filterPhotos() {
            const input = document.getElementById('searchInput').value.toLowerCase();
            const photos = document.querySelectorAll('.photo');

            photos.forEach(photo => {
                const caption = photo.querySelector('.caption').innerText.toLowerCase();
                if (caption.includes(input)) {
                    photo.style.display = 'block';
                } else {
                    photo.style.display = 'none';
                }
            });
        }
    </script>

</body>
</html>
```



## OUTPUT:
<img width="1920" height="1080" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/611063c5-e182-46bf-a024-6e81bafe1142" />
<img width="1920" height="1080" alt="Screenshot 2025-10-05 124035" src="https://github.com/user-attachments/assets/10c7eae9-b486-4591-a7c1-aeec0f42d629" />
<img width="1917" height="1076" alt="Screenshot 2025-10-05 124105" src="https://github.com/user-attachments/assets/99890a85-1ff3-4a3f-96db-1a36c9073e85" />
<img width="1919" height="1079" alt="Screenshot 2025-10-05 124122" src="https://github.com/user-attachments/assets/49a96566-feeb-4a40-998f-e542a066de44" />
<img width="1916" height="1067" alt="Screenshot 2025-10-05 124142" src="https://github.com/user-attachments/assets/5788637c-5b5b-432f-8f93-734544520fc7" />
<img width="1920" height="1080" alt="Screenshot 2025-10-05 124154" src="https://github.com/user-attachments/assets/665f2aea-e17b-488f-b162-97d70233410b" />




## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.

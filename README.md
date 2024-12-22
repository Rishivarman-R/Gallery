# Ex.08 Design of Interactive Image Gallery
# Date:21.12.2024
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
    <body>
        <header>
            <h1><font color="orange">IMAGE GALLERY</font></h1>
        </header>
        <header>
            <h2><font color="aqua">7 WONDERS</font></h2>
        </header>
    </body>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
             background-image: url("background.jpg");
            background-size:cover;
        }

        h1 {
            margin-top: 20px;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 300px;
            height: 200px;
            border: 2px solid #ccc;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery">
        <img src="tajmahal.jpg" alt="Image 1" onclick="openModal(this)">
        <img src="chinawall.jpg" alt="Image 2" onclick="openModal(this)">
        <img src="china.jpg" alt="Image 3" onclick="openModal(this)">
        <img src="colosseum.jpg" alt="Image 4" onclick="openModal(this)">
        <img src="cristo.jpg" alt="Image 5" onclick="openModal(this)">
        <img src="Chichen Itza.jpg" alt="Image 5" onclick="openModal(this)">
        <img src="Machu Picchu.jpg" alt="Image 5" onclick="openModal(this)">
    </div>

    <!-- Modal for displaying larger image -->
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        // Function to open the modal and display the clicked image
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }

        // Function to close the modal
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>
```
# OUTPUT:
![Screenshot (64)](https://github.com/user-attachments/assets/86c60e66-bcdc-4c3c-a241-7244912d5af8)

![Screenshot (65)](https://github.com/user-attachments/assets/2d9fde55-4928-468a-abb5-668a5341c7be)

![Screenshot (66)](https://github.com/user-attachments/assets/0ab06138-a822-4166-8e98-d7211e9cf818)

![Screenshot (67)](https://github.com/user-attachments/assets/17df8da0-dc07-4790-83c2-b38d20cc84be)

![Uploading Screenshot (68).png…]()

![Screenshot (69)](https://github.com/user-attachments/assets/1d316d75-2c82-4432-8096-0f2943273c1b)

![Screenshot (70)](https://github.com/user-attachments/assets/987678a4-15ba-479f-af7c-e1af55ba6f3d)

![Screenshot (71)](https://github.com/user-attachments/assets/84b6eda4-10bd-4342-9be2-7738d289cef6)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.

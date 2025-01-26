<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OldBull - Handyman Extraordinaire</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        nav {
            background: #333;
            color: white;
            padding: 10px;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 1.1em;
        }
        nav a:hover {
            text-decoration: underline;
        }
        header {
            background: url('banner.jpg') no-repeat center center/cover;
            height: 300px;
            text-align: center;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        header h1 {
            font-size: 3em;
            text-shadow: 2px 2px 5px #000;
            padding: 20px;
        }
        main {
            padding: 20px;
        }
        .about {
            text-align: center;
            margin-bottom: 40px;
        }
        .about h2 {
            color: #444;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
        }
        .gallery img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.2s;
        }
        .gallery img:hover {
            transform: scale(1.05);
        }
        #contact {
            background: #f4f4f4;
            padding: 20px;
            text-align: center;
        }
        #contact form {
            max-width: 400px;
            margin: 0 auto;
            text-align: left;
        }
        #contact input, #contact textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        #contact button {
            padding: 10px 20px;
            background: #333;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        #contact button:hover {
            background: #555;
        }
        footer {
            text-align: center;
            padding: 10px;
            background: #333;
            color: #fff;
        }
        footer a {
            color: #f4f4f4;
            text-decoration: none;
        }
    </style>
</head>
<body>

<nav>
    <a href="#about">About</a>
    <a href="#gallery">Gallery</a>
    <a href="#contact">Contact</a>
</nav>

<header>
    <h1>OldBull - Handyman Extraordinaire</h1>
</header>

<main>
    <section id="about" class="about">
        <h2>Welcome to My Portfolio!</h2>
        <p>My name is OldBull, and I am a handyman ready to solve your problems.  
        I specialize in all kinds of repairs – from mechanical to home repairs,  
        and I can even help fix your mind!</p>
    </section>

    <section id="gallery" class="gallery">
        <h2>Gallery</h2>
        <p>Thumbnails of cows and bulls:</p>
        <img src="cow1.jpg" alt="A peaceful brown cow grazing in a field." loading="lazy">
        <img src="cow2.jpg" alt="A white cow with black spots standing in the barnyard." loading="lazy">
        <img src="bull1.jpg" alt="A majestic bull with large horns in a meadow." loading="lazy">
        <img src="bull2.jpg" alt="A strong black bull in a rustic setting." loading="lazy">
        <img src="cow3.jpg" alt="A curious cow looking at the camera." loading="lazy">
    </section>

    <section id="contact">
        <h2>Contact Me</h2>
        <p>If you need a reliable handyman, feel free to get in touch:</p>
        <form action="submit_form.php" method="POST">
            <label for="name">Name:</label><br>
            <input type="text" id="name" name="name" required><br><br>

            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email" required><br><br>

            <label for="message">Message:</label><br>
            <textarea id="message" name="message" rows="4" required></textarea><br><br>

            <button type="submit">Send</button>
        </form>
        <p>Or reach me at: <a href="mailto:oldbull@handyman.com">oldbull@handyman.com</a></p>
    </section>
</main>

<footer>
    <p>&copy; 2025 OldBull - All rights reserved. | <a href="#contact">Contact</a></p>
</footer>

</body>
</html>

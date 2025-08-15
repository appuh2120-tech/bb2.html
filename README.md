x;}
        .menu-toggle {display:block<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>My Multi-Page Website</title>
<style>
    * {margin:0; padding:0; box-sizing:border-box;}
    body {font-family: Arial, sans-serif; background:#111; color:#fff; scroll-behavior: smooth;}
    header {background:#222; padding:10px 20px; position:fixed; top:0; width:100%; z-index:100;}
    nav {display:flex; justify-content:space-between; align-items:center;}
    nav .logo {font-size:1.5em; font-weight:bold; color:orange;}
    nav ul {display:flex; list-style:none;}
    nav ul li {margin:0 15px;}
    nav ul li a {color:white; text-decoration:none; font-weight:bold;}
    nav ul li a:hover {color:orange;}
    .menu-toggle {display:none; font-size:1.5em; cursor:pointer;}
    section {padding:100px 20px; min-height:100vh;}
    .home {background:url('https://picsum.photos/1200/800') no-repeat center/cover; text-align:center; display:flex; flex-direction:column; justify-content:center;}
    .home h1 {font-size:3em; animation: fadeIn 2s;}
    .about, .gallery, .contact {background:#181818;}
    .gallery img {width:250px; height:150px; margin:10px; border-radius:8px; transition:0.3s;}
    .gallery img:hover {transform:scale(1.1);}
    footer {background:#222; text-align:center; padding:15px;}
    footer a {color:orange; margin:0 10px; font-size:1.2em; text-decoration:none;}
    @keyframes fadeIn {from {opacity:0;} to {opacity:1;}}
    @media(max-width:768px) {
        nav ul {display:none; flex-direction:column; background:#222; position:absolute; top:60px; right:0; width:200px;}
        nav ul.show {display:fle;}
    }
</style>
</head>
<body>

<header>
    <nav>
        <div class="logo">MyWebsite</div>
        <div class="menu-toggle" onclick="toggleMenu()">☰</div>
        <ul id="menu">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#gallery">Gallery</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<section id="home" class="home">
    <h1>Welcome to My Website</h1>
    <p>Explore my awesome multi-page responsive site!</p>
</section>

<section id="about" class="about">
    <h2>About Me</h2>
    <p>This is an example of a multi-page looking website built with HTML, CSS, and JavaScript.</p>
</section>

<section id="gallery" class="gallery">
    <h2>Gallery</h2>
    <img src="https://picsum.photos/250/150?1" alt="">
    <img src="https://picsum.photos/250/150?2" alt="">
    <img src="https://picsum.photos/250/150?3" alt="">
</section>

<section id="contact" class="contact">
    <h2>Contact</h2>
    <p>Email: you@example.com</p>
    <p>Phone: +91 9876543210</p>
</section>

<footer>
    <p>© 2025 My Website</p>
    <a href="#">🌐</a>
    <a href="#">📘</a>
    <a href="#">🐦</a>
</footer>

<script>
    function toggleMenu() {
        document.getElementById('menu').classList.toggle('show');
    }
</script>

</body>
</html>

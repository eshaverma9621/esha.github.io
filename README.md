<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            background-color: #0F172A; 
            color: #E2E8F0; 
        }
        .navbar {
            background-color: #1E293B;
        }
        .navbar-brand, .navbar-nav .nav-link {
            color: #38BDF8 !important; 
						
        }
				 .navbar-brand {
            color: #38BDF8 !important;
            font-size: 1.5rem;
            font-weight: bold;
            position: absolute;
            left: 50%;
            transform: translateX(-50%); 
        }
        .navbar-nav .nav-link:hover {
            background-color: #334155;
            color: #FFFFFF !important;
        }
        .header {
            position: relative;
            text-align: center;
            background-color: #1E40AF; 
            color: #FFFFFF;
            padding: 0;
        }
        .header-img {
            width: 100%;
            height: 600px;
            object-fit: cover;
            object-position: top;
            display: block;
            transition: transform 0.3s ease;
        }
        .header-img:hover {
            transform: scale(1.05); 
        }
        .header-content h1 {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 2.5rem;
            font-weight: bold;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        .content {
            max-width: 90%;
            margin: 2rem auto;
        }
      	.profile-img {
            width: 150px; 
            height: 150px; 
            border-radius: 50%;
            object-fit: cover;
            display: block;
            margin: 0 auto;
            border: 3px solid #38BDF8;
            overflow: hidden;
            box-sizing: border-box; 
            transition: transform 0.3s ease, box-shadow 0.3s ease; 
            }

        .profile-img:hover {
            transform: scale(1.1) rotate(5deg);
            box-shadow: 0 0 15px rgba(56, 189, 248, 0.7); 
          }
       
        h2 {
            font-size: 1.5rem;
            color: #38BDF8;
            transition: text-shadow 0.3s ease, transform 0.3s ease;
					  text-shadow: 0 0 8px rgba(56, 189, 248, 0.6); 
            transform: scale(1);
            font-size: 1.5rem;
            color: #FFFFFF; 
        }
        p, ul {
            font-size: 1rem;
            color: #FFFFFF;
        }
				p, ul {
				    font-size: 1rem;
						color: white;}
        .btn-custom {
            background-color: #38BDF8;
            color: #FFFFFF;
            font-weight: bold;
        }
        .btn-custom:hover {
            background-color: #0EA5E9;
						text-shadow: 0 0 8px rgba(56, 189, 248, 0.6); 
            transform: scale(1.05);
        }
        .sidebar {
            height: 100%;
            width: 0;
            position: fixed;
            top: 0;
            left: 0;
            background-color: #1E293B;
            overflow-x: hidden;
            transition: 0.3s;
            padding-top: 60px;
            z-index: 1000;
        }
        .sidebar a {
            padding: 8px 8px 8px 32px;
            text-decoration: none;
            font-size: 1.1rem;
            color: #38BDF8;
            display: block;
            transition: 0.3s;
        }
        .sidebar a:hover {
            color: #FFFFFF;
            background-color: #334155;
        }
        .sidebar .closebtn {
            position: absolute;
            top: 0;
            right: 25px;
            font-size: 36px;
            margin-left: 50px;
        }
        .openbtn {
            font-size: 1.2rem;
            cursor: pointer;
            background-color: #1E293B;
            color: #38BDF8;
            padding: 10px 15px;
            border: none;
            position: fixed;
            top: 10px;
            left: 10px;
            z-index: 999;
        }
        .openbtn:hover {
            background-color: #334155;
        }
        @media screen and (max-width: 768px) {
            .header-img {
                height: 400px;
            }
          }
								.header-content h1 {  
								
								 position: absolute;
                 bottom: 20px;
                 left: 50%;
                 transform: translateX(-50%);
                 font-size: 2.5rem;
                 font-weight: bold;
                 transition: text-shadow 0.3s ease, transform 0.3s ease;
                 

            }
				       		.header-content h1:hover {
                 
                 transform: translateX(-50%) scale(1.05);
                 }
        
    </style>
</head>
<body>
    <!-- Sidebar -->
    <div id="mySidebar" class="sidebar">
        <a href="javascript:void(0)" class="closebtn" onclick="closeNav()">×</a>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
    </div>

    <!-- Open Sidebar Button -->
    <button class="openbtn" onclick="openNav()">☰ Menu</button>

    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">Esha's Portfolio</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#home">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#about">About</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact">Contact</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Header -->
    <header class="header">
        <div class="header-content">
            <img src="imagee.jpg" class="header-img" alt="Header Image">
            <h1>Esha Verma - Web Wizard & Data Dynamo</h1>
        </div>
    </header>

    <        <div class="card shadow-lg p-4" style="background-color: #1E293B; border: none;">
            <img src="image.jpg" alt="Profile Picture" class="profile-img mb-3">
            <h2 id="about">About Me</h2>
            <p>Crafting digital experiences with code and creativity, I'm a BCA student passionate about building stunning websites and mastering data. With a knack for storytelling through design and copy, I bring ideas to life.</p>
            <h2 id="skills">My Skills</h2>
            <ul>
                <li><strong>HTML & CSS</strong>: Designing responsive, pixel-perfect webpages</li>
                <li><strong>Bootstrap</strong>: Creating sleek, mobile-first layouts with ease</li>
                <li><strong>WordPress</strong>: Building dynamic blogs and professional sites</li>
                <li><strong>SQL</strong>: Structuring and querying data for seamless management</li>
                <li><strong>Copywriting</strong>: Crafting compelling content that engages and converts</li>
            </ul>
            <h2 id="projects">My Projects</h2>
            <p><strong>Cafe Website</strong>: Designed a vibrant, responsive site using HTML, CSS, and Bootstrap for a local cafe.</p>
            <p><strong>Student Database</strong>: Developed efficient SQL queries for streamlined data management.</p>
            <p><strong>Blog Platform</strong>: Built a WordPress blog with custom copywriting to boost engagement.</p>
            <h2>Testimonial</h2>
            <p>"Esha’s work is exceptional—creative, timely, and professional!" – Local Cafe Owner</p>
            <button class="btn btn-custom" onclick="alert('Let’s create something amazing together!')">Hire Me</button>
        </div>
    <div class="content">

    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        function openNav() {
            document.getElementById("mySidebar").style.width = "250px";
        }

        function closeNav() {
            document.getElementById("mySidebar").style.width = "0";
        }
    </script>
</body>
</html>

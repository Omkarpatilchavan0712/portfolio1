  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PORTFOLIO - Create Your Professional Portfolio</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #6c63ff;
            --secondary-color: #4d44db;
            --dark-color: #2f2e41;
            --light-color: #f8f9fa;
            --text-color: #333333;
            --success-color: #28a745;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            color: var(--text-color);
            overflow-x: hidden;
        }
        
        .navbar {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 15px 0;
        }
        
        .navbar-brand {
            font-weight: 700;
            color: var(--primary-color) !important;
            font-size: 1.8rem;
        }
        
        .nav-link {
            font-weight: 500;
            margin: 0 10px;
            color: var(--dark-color) !important;
        }
        
        .nav-link:hover {
            color: var(--primary-color) !important;
        }
        
        .btn-primary {
            background-color: var(--primary-color);
            border-color: var(--primary-color);
            padding: 8px 20px;
            border-radius: 50px;
        }
        
        .btn-primary:hover {
            background-color: var(--secondary-color);
            border-color: var(--secondary-color);
        }
        
        .btn-outline-primary {
            color: var(--primary-color);
            border-color: var(--primary-color);
            padding: 8px 20px;
            border-radius: 50px;
        }
        
        .btn-outline-primary:hover {
            background-color: var(--primary-color);
            color: white;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #f5f7fa 0%, #e4e8f0 100%);
            padding: 100px 0;
            position: relative;
            overflow: hidden;
        }
        
        .hero-content {
            position: relative;
            z-index: 2;
        }
        
        .hero h1 {
            font-weight: 700;
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--dark-color);
        }
        
        .hero p {
            font-size: 1.1rem;
            margin-bottom: 30px;
            color: #666;
        }
        
        .hero-image-container {
            position: relative;
            perspective: 1000px;
        }
        
        .hero-image {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            transform: rotateY(20deg) rotateX(10deg);
            transition: transform 0.5s ease;
            animation: float 6s ease-in-out infinite;
        }
        
        .hero-image:hover {
            transform: rotateY(0) rotateX(0);
        }
        
        @keyframes float {
            0% { transform: translateY(0) rotateY(20deg) rotateX(10deg); }
            50% { transform: translateY(-20px) rotateY(20deg) rotateX(10deg); }
            100% { transform: translateY(0) rotateY(20deg) rotateX(10deg); }
        }
        
        /* Features Section */
        .features {
            padding: 80px 0;
        }
        
        .feature-card {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: all 0.3s ease;
            margin-bottom: 30px;
            height: 100%;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            width: 80px;
            height: 80px;
            background-color: rgba(108, 99, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
            color: var(--primary-color);
            font-size: 30px;
        }
        
        /* Portfolio Showcase */
        .portfolio {
            padding: 80px 0;
            background-color: #f9f9f9;
        }
        
        .portfolio-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .portfolio-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .portfolio-item:hover .portfolio-img {
            transform: scale(1.1);
        }
        
        .portfolio-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: rgba(108, 99, 255, 0.9);
            overflow: hidden;
            width: 100%;
            height: 0;
            transition: .5s ease;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
        }
        
        .portfolio-item:hover .portfolio-overlay {
            height: 100%;
        }
        
        /* Testimonials */
        .testimonials {
            padding: 80px 0;
            background: linear-gradient(135deg, #6c63ff 0%, #4d44db 100%);
            color: white;
        }
        
        .testimonial-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 30px;
            margin-bottom: 30px;
        }
        
        .testimonial-img {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid rgba(255, 255, 255, 0.2);
        }
        
        /* Contact */
        .contact {
            padding: 80px 0;
        }
        
        .form-control {
            padding: 12px 15px;
            border-radius: 8px;
            margin-bottom: 20px;
            border: 1px solid #e1e1e1;
        }
        
        .form-control:focus {
            box-shadow: 0 0 0 0.25rem rgba(108, 99, 255, 0.25);
            border-color: var(--primary-color);
        }
        
        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-links h5 {
            font-weight: 600;
            margin-bottom: 20px;
        }
        
        .footer-links ul {
            list-style: none;
            padding-left: 0;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        .social-icons a {
            width: 40px;
            height: 40px;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            margin-right: 10px;
            color: white;
            transition: all 0.3s;
        }
        
        .social-icons a:hover {
            background-color: var(--primary-color);
            transform: translateY(-3px);
        }
        
        /* Modal */
        .modal-content {
            border-radius: 10px;
            border: none;
        }
        
        .modal-header {
            border-bottom: none;
            padding-bottom: 0;
        }
        
        .modal-title {
            font-weight: 600;
        }
        
        /* Responsive */
        @media (max-width: 991px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero-image {
                margin-top: 50px;
            }
        }
        
        @media (max-width: 767px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
        }
        
        /* Animation classes */
        .animate-in {
            animation: fadeInUp 0.8s ease forwards;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-light sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#">PORTFOLIO</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link" href="#home">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#features">Features</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#portfolio">Portfolios</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact">Contact</a>
                    </li>
                </ul>
                <div class="d-flex">
                    <button class="btn btn-outline-primary me-2" data-bs-toggle="modal" data-bs-target="#loginModal">Login</button>
                    <button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#registerModal">Sign Up</button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6 hero-content animate-in">
                    <h1>Build Your Perfect Portfolio in Minutes</h1>
                    <p>Showcase your work, skills, and achievements with our easy-to-use portfolio builder. Impress clients and employers with a professional online presence.</p>
                    <div class="d-flex flex-wrap gap-3">
                        <button class="btn btn-primary btn-lg" data-bs-toggle="modal" data-bs-target="#registerModal">Get Started</button>
                        <button class="btn btn-outline-primary btn-lg">View Examples</button>
                    </div>
                </div>
                <div class="col-lg-6 hero-image-container animate-in" style="animation-delay: 0.2s;">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/8a2682d7-8248-4727-88a0-56473e60a2b7.png" alt="Modern laptop screen displaying a professional portfolio website with project thumbnails and profile information" class="hero-image">
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="features">
        <div class="container">
            <div class="row mb-5">
                <div class="col-12 text-center">
                    <h2 class="fw-bold">Why Choose PORTFOLIO</h2>
                    <p class="text-muted">Everything you need to build a stunning portfolio</p>
                </div>
            </div>
            <div class="row">
                <div class="col-md-4 animate-in">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-magic"></i>
                        </div>
                        <h4>Beautiful Templates</h4>
                        <p>Choose from dozens of professionally designed templates tailored for every profession and style.</p>
                    </div>
                </div>
                <div class="col-md-4 animate-in" style="animation-delay: 0.2s;">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-mobile-alt"></i>
                        </div>
                        <h4>Fully Responsive</h4>
                        <p>Your portfolio will look perfect on any device, from smartphones to desktop computers.</p>
                    </div>
                </div>
                <div class="col-md-4 animate-in" style="animation-delay: 0.4s;">
                    <div class="feature-card">
                        <div class="feature-icon">
                            <i class="fas fa-cogs"></i>
                        </div>
                        <h4>Easy Customization</h4>
                        <p>Change colors, fonts, layouts with our intuitive dashboard. No coding required.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Showcase -->
    <section class="portfolio" id="portfolio">
        <div class="container">
            <div class="row mb-5">
                <div class="col-12 text-center">
                    <h2 class="fw-bold">Portfolio Examples</h2>
                    <p class="text-muted">See what our users have created</p>
                </div>
            </div>
            <div class="row">
                <div class="col-md-4 animate-in">
                    <div class="portfolio-item">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/043716cc-a8ac-4235-a92e-eb500a951c57.png" alt="Photography portfolio example showing landscape images in a grid layout" class="portfolio-img">
                        <div class="portfolio-overlay">
                            <h4>Photography</h4>
                            <p>By Sarah Johnson</p>
                            <a href="#" class="btn btn-outline-light mt-3">View Portfolio</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 animate-in" style="animation-delay: 0.2s;">
                    <div class="portfolio-item">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/2d17c0d7-3cda-49d3-a260-9bbbc51e1102.png" alt="Graphic designer's portfolio featuring logo designs and branding projects" class="portfolio-img">
                        <div class="portfolio-overlay">
                            <h4>Graphic Design</h4>
                            <p>By Michael Chen</p>
                            <a href="#" class="btn btn-outline-light mt-3">View Portfolio</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 animate-in" style="animation-delay: 0.4s;">
                    <div class="portfolio-item">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/3fd84ea9-4674-475b-a4dc-4ce69f484232.png" alt="Web developer portfolio showcasing responsive website designs and coding projects" class="portfolio-img">
                        <div class="portfolio-overlay">
                            <h4>Web Development</h4>
                            <p>By Alex Rodriguez</p>
                            <a href="#" class="btn btn-outline-light mt-3">View Portfolio</a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row mt-4">
                <div class="col-12 text-center">
                    <a href="#" class="btn btn-primary">View More Portfolios</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="testimonials">
        <div class="container">
            <div class="row mb-5">
                <div class="col-12 text-center">
                    <h2 class="fw-bold text-white">What Our Users Say</h2>
                    <p>Success stories from professionals like you</p>
                </div>
            </div>
            <div class="row">
                <div class="col-md-4 animate-in">
                    <div class="testimonial-card">
                        <div class="d-flex align-items-center mb-4">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c163c511-27b3-42db-80f8-a740d4eea250.png" alt="Portrait of John Smith, a graphic designer in his studio" class="testimonial-img me-3">
                            <div>
                                <h5 class="mb-0">John Smith</h5>
                                <p class="mb-0">Graphic Designer</p>
                            </div>
                        </div>
                        <p>"PORTFOLIO helped me land my dream job at a top design agency. The templates are gorgeous and the customization options are endless."</p>
                    </div>
                </div>
                <div class="col-md-4 animate-in" style="animation-delay: 0.2s;">
                    <div class="testimonial-card">
                        <div class="d-flex align-items-center mb-4">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/5db55969-8ff3-45a7-abbb-1636c66f55d3.png" alt="Portrait of Emily Wilson, a photographer in outdoor setting" class="testimonial-img me-3">
                            <div>
                                <h5 class="mb-0">Emily Wilson</h5>
                                <p class="mb-0">Photographer</p>
                            </div>
                        </div>
                        <p>"I've doubled my client base since creating my portfolio with this platform. The mobile-friendly design is a game-changer!"</p>
                    </div>
                </div>
                <div class="col-md-4 animate-in" style="animation-delay: 0.4s;">
                    <div class="testimonial-card">
                        <div class="d-flex align-items-center mb-4">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/20be4e2d-5d1a-4335-81cd-6dd8ada5beb5.png" alt="Portrait of David Brown, a web developer working on laptop" class="testimonial-img me-3">
                            <div>
                                <h5 class="mb-0">David Brown</h5>
                                <p class="mb-0">Web Developer</p>
                            </div>
                        </div>
                        <p>"As a developer, I appreciate the clean code and customization options. My portfolio stands out from the crowd now."</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="row">
                <div class="col-lg-6 animate-in">
                    <h2 class="fw-bold mb-4">Have Questions?</h2>
                    <p>Our team is here to help you create the perfect portfolio. Send us a message and we'll get back to you within 24 hours.</p>
                    <div class="mt-5">
                        <h5><i class="fas fa-envelope me-2 text-primary"></i> contact@portfolio.example.com</h5>
                        <h5 class="mt-3"><i class="fas fa-phone-alt me-2 text-primary"></i> +1 (555) 123-4567</h5>
                    </div>
                </div>
                <div class="col-lg-6 animate-in" style="animation-delay: 0.2s;">
                    <form>
                        <div class="row">
                            <div class="col-md-6">
                                <input type="text" class="form-control" placeholder="Your Name">
                            </div>
                            <div class="col-md-6">
                                <input type="email" class="form-control" placeholder="Your Email">
                            </div>
                        </div>
                        <input type="text" class="form-control" placeholder="Subject">
                        <textarea class="form-control" rows="5" placeholder="Your Message"></textarea>
                        <button type="submit" class="btn btn-primary">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-lg-4 mb-4">
                    <h5 class="navbar-brand mb-3">PORTFOLIO</h5>
                    <p>The easiest way to create a professional portfolio and showcase your work to the world.</p>
                    <div class="social-icons mt-3">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 mb-4">
                    <h5>Quick Links</h5>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Features</a></li>
                        <li><a href="#">Pricing</a></li>
                        <li><a href="#">Portfolios</a></li>
                        <li><a href="#">Contact</a></li>
                    </ul>
                </div>
                <div class="col-lg-3 col-md-4 mb-4">
                    <h5>Resources</h5>
                    <ul>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Help Center</a></li>
                        <li><a href="#">Tutorials</a></li>
                        <li><a href="#">FAQ</a></li>
                    </ul>
                </div>
                <div class="col-lg-3 col-md-4 mb-4">
                    <h5>Legal</h5>
                    <ul>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Terms of Service</a></li>
                        <li><a href="#">Cookie Policy</a></li>
                    </ul>
                </div>
            </div>
            <hr class="mt-4" style="border-color: rgba(255,255,255,0.1);">
            <div class="row">
                <div class="col-12 text-center">
                    <p class="mb-0">© 2023 PORTFOLIO. All rights reserved.</p>
                </div>
            </div>
        </div>
    </footer>

    <!-- Login Modal -->
    <div class="modal fade" id="loginModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Login to Your Account</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form>
                        <div class="mb-3">
                            <label for="loginEmail" class="form-label">Email address</label>
                            <input type="email" class="form-control" id="loginEmail" placeholder="name@example.com">
                        </div>
                        <div class="mb-3">
                            <label for="loginPassword" class="form-label">Password</label>
                            <input type="password" class="form-control" id="loginPassword" placeholder="Enter your password">
                        </div>
                        <div class="mb-3 form-check">
                            <input type="checkbox" class="form-check-input" id="rememberMe">
                            <label class="form-check-label" for="rememberMe">Remember me</label>
                        </div>
                        <button type="submit" class="btn btn-primary w-100">Login</button>
                    </form>
                    <div class="text-center mt-3">
                        <a href="#" class="text-decoration-none">Forgot password?</a>
                    </div>
                    <div class="text-center mt-3">
                        <p>Don't have an account? <a href="#" class="text-primary text-decoration-none" data-bs-toggle="modal" data-bs-target="#registerModal" data-bs-dismiss="modal">Sign up</a></p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Register Modal -->
    <div class="modal fade" id="registerModal" tabindex="-1" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title">Create Your Account</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form>
                        <div class="row mb-3">
                            <div class="col-md-6">
                                <label for="firstName" class="form-label">First Name</label>
                                <input type="text" class="form-control" id="firstName" placeholder="First name">
                            </div>
                            <div class="col-md-6">
                                <label for="lastName" class="form-label">Last Name</label>
                                <input type="text" class="form-control" id="lastName" placeholder="Last name">
                            </div>
                        </div>
                        <div class="mb-3">
                            <label for="registerEmail" class="form-label">Email address</label>
                            <input type="email" class="form-control" id="registerEmail" placeholder="name@example.com">
                        </div>
                        <div class="mb-3">
                            <label for="registerPassword" class="form-label">Password</label>
                            <input type="password" class="form-control" id="registerPassword" placeholder="Create a password">
                        </div>
                        <div class="mb-3">
                            <label for="confirmPassword" class="form-label">Confirm Password</label>
                            <input type="password" class="form-control" id="confirmPassword" placeholder="Confirm your password">
                        </div>
                        <div class="mb-3 form-check">
                            <input type="checkbox" class="form-check-input" id="agreeTerms">
                            <label class="form-check-label" for="agreeTerms">I agree to the <a href="#" class="text-primary">Terms of Service</a> and <a href="#" class="text-primary">Privacy Policy</a></label>
                        </div>
                        <button type="submit" class="btn btn-primary w-100">Create Account</button>
                    </form>
                    <div class="text-center mt-3">
                        <p>Already have an account? <a href="#" class="text-primary text-decoration-none" data-bs-toggle="modal" data-bs-target="#loginModal" data-bs-dismiss="modal">Log in</a></p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
    
    <script>
        // Animation on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const animateElements = document.querySelectorAll('.animate-in');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, {
                threshold: 0.1
            });
            
            animateElements.forEach(element => {
                element.style.opacity = '0';
                element.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
                observer.observe(element);
            });
            
            // Hero image animation
            const heroImage = document.querySelector('.hero-image');
            if (heroImage) {
                document.addEventListener('mousemove', function(e) {
                    const x = e.clientX / window.innerWidth;
                    const y = e.clientY / window.innerHeight;
                    heroImage.style.transform = `rotateY(${20 - x * 20}deg) rotateX(${10 - y * 10}deg)`;
                });
            }
            
            // Form validation for registration
            const registerForm = document.querySelector('#registerModal form');
            if (registerForm) {
                registerForm.addEventListener('submit', function(e) {
                    e.preventDefault();
                    
                    const password = document.getElementById('registerPassword').value;
                    const confirmPassword = document.getElementById('confirmPassword').value;
                    
                    if (password !== confirmPassword) {
                        alert('Passwords do not match!');
                        return;
                    }
                    
                    if (!document.getElementById('agreeTerms').checked) {
                        alert('You must agree to the Terms of Service and Privacy Policy');
                        return;
                    }
                    
                    // Here you would typically send the data to your server
                    alert('Account created successfully! Redirecting to your dashboard...');
                    // window.location.href = 'dashboard.html';
                });
            }
            
            // Form validation for login
            const loginForm = document.querySelector('#loginModal form');
            if (loginForm) {
                loginForm.addEventListener('submit', function(e) {
                    e.preventDefault();
                    
                    const email = document.getElementById('loginEmail').value;
                    const password = document.getElementById('loginPassword').value;
                    
                    // Here you would typically validate credentials with your server
                    if (email && password) {
                        alert('Login successful! Redirecting to your dashboard...');
                        // window.location.href = 'dashboard.html';
                    } else {
                        alert('Please enter both email and password');
                    }
                });
            }
        });
    </script>
</body>
</html>


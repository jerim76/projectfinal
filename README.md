# projectfinal<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SchoolUber - Safe Student Transportation</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.0/font/bootstrap-icons.css">
    <style>
        :root {
            --primary: #2563eb;  /* Vibrant blue */
            --primary-dark: #1d4ed8;
            --secondary: #f59e0b; /* Amber accent */
            --light: #f8fafc;
            --dark: #1e293b;
            --success: #10b981;
            --danger: #ef4444;
        }
        
        body {
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
            color: var(--dark);
            line-height: 1.6;
            padding-top: 76px;
            background-color: #ffffff;
        }
        
        /* Navigation */
        .navbar {
            background-color: var(--primary) !important;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 0.8rem 0;
        }
        
        .navbar-brand img {
            height: 40px;
        }
        
        .nav-link {
            font-weight: 500;
            padding: 0.5rem 1rem !important;
        }
        
        /* Hero Section */
        .hero-section {
            background: linear-gradient(135deg, rgba(37, 99, 235, 0.9), rgba(29, 78, 216, 0.9)), 
                        url('https://images.unsplash.com/photo-1541178735493-479c1a27ed24?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 120px 0;
            text-align: center;
            margin-top: -76px;
        }
        
        .hero-section h1 {
            font-size: clamp(2.5rem, 5vw, 3.5rem);
            font-weight: 800;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.3);
        }
        
        .hero-section .lead {
            font-size: 1.25rem;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        
        /* Sections */
        section {
            padding: 80px 0;
        }
        
        .section-title {
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--primary);
        }
        
        .section-subtitle {
            color: #64748b;
            margin-bottom: 3rem;
        }
        
        /* Cards */
        .feature-card {
            border: none;
            border-radius: 12px;
            transition: all 0.3s ease;
            height: 100%;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }
        
        /* Stats */
        .stat-card {
            margin-bottom: 2rem;
        }
        
        .stat-card h3 {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--primary);
        }
        
        /* Team */
        .team-card {
            border: none;
            border-radius: 12px;
            overflow: hidden;
            transition: all 0.3s ease;
        }
        
        .team-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .team-card img {
            height: 250px;
            object-fit: cover;
        }
        
        /* Contact Form */
        #contactForm {
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            padding: 2rem;
            transition: all 0.3s ease;
        }
        
        #contactForm:focus-within {
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        /* Buttons */
        .btn-primary {
            background-color: var(--primary);
            border-color: var(--primary);
            font-weight: 500;
            padding: 0.5rem 1.5rem;
        }
        
        .btn-primary:hover {
            background-color: var(--primary-dark);
            border-color: var(--primary-dark);
        }
        
        .btn-outline-light:hover {
            color: var(--primary);
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 0 1.5rem;
        }
        
        footer a {
            color: #e2e8f0;
            text-decoration: none;
            transition: color 0.2s;
        }
        
        footer a:hover {
            color: white;
        }
        
        /* Responsive adjustments */
        @media (max-width: 768px) {
            .hero-section {
                padding: 100px 0;
            }
            
            section {
                padding: 60px 0;
            }
            
            .display-3 {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body data-bs-spy="scroll" data-bs-target=".navbar">
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-dark fixed-top">
        <div class="container">
            <a class="navbar-brand" href="#">
                <span style="font-weight: 700; font-size: 1.5rem;">SchoolUber</span>
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#problem">Problem</a></li>
                    <li class="nav-item"><a class="nav-link" href="#solution">Solution</a></li>
                    <li class="nav-item"><a class="nav-link" href="#features">Features</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
                    <li class="nav-item ms-2"><a class="btn btn-outline-light" href="#contact">Get Started</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-section">
        <div class="container">
            <h1 class="display-3 fw-bold mb-3">Safe Student Transportation</h1>
            <p class="lead mb-4">Smart tracking and verified drivers for worry-free school commutes</p>
            <div class="d-flex justify-content-center gap-3">
                <a href="#solution" class="btn btn-light btn-lg px-4">Learn More</a>
                <a href="#contact" class="btn btn-outline-light btn-lg px-4">Get Started</a>
            </div>
        </div>
    </section>

    <!-- Problem Section -->
    <section id="problem" class="py-5 bg-light">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6">
                    <h2 class="section-title">The School Transport Crisis</h2>
                    <div class="stat-card">
                        <h3 class="text-danger">475+</h3>
                        <p class="fs-5">school bus accidents causing injuries annually</p>
                    </div>
                    <div class="stat-card">
                        <h3>68%</h3>
                        <p class="fs-5">of parents worry about transport safety daily</p>
                    </div>
                    <div class="stat-card">
                        <h3>30+</h3>
                        <p class="fs-5">minutes wasted due to inefficient routing</p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <img src="https://images.unsplash.com/photo-1600189261867-8e2c085eea4a?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                         alt="Overcrowded school bus" 
                         class="img-fluid rounded-3 shadow">
                </div>
            </div>
        </div>
    </section>

    <!-- Solution Section -->
    <section id="solution" class="py-5">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="section-title">The SchoolUber Solution</h2>
                <p class="section-subtitle">Technology-driven safety for peace of mind</p>
            </div>
            <div class="row g-4">
                <div class="col-md-6 col-lg-3">
                    <div class="card feature-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="feature-icon">
                                <i class="bi bi-geo-alt-fill"></i>
                            </div>
                            <h4>Real-Time Tracking</h4>
                            <p>Parents monitor location via mobile app in real-time</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-3">
                    <div class="card feature-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="feature-icon">
                                <i class="bi bi-shield-check"></i>
                            </div>
                            <h4>Verified Drivers</h4>
                            <p>Rigorous background checks and training for all drivers</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-3">
                    <div class="card feature-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="feature-icon">
                                <i class="bi bi-signpost-split"></i>
                            </div>
                            <h4>Smart Routing</h4>
                            <p>AI reduces commute times by 30% with optimized routes</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 col-lg-3">
                    <div class="card feature-card h-100">
                        <div class="card-body text-center p-4">
                            <div class="feature-icon">
                                <i class="bi bi-bell-fill"></i>
                            </div>
                            <h4>Safety Alerts</h4>
                            <p>Instant notifications for arrivals, departures, and delays</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="py-5 bg-light">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-6 order-lg-2">
                    <h2 class="section-title">Advanced Safety Features</h2>
                    <div class="d-flex mb-4">
                        <div class="me-3 text-primary">
                            <i class="bi bi-exclamation-triangle-fill fs-3"></i>
                        </div>
                        <div>
                            <h5>Emergency SOS</h5>
                            <p>Instant alerts to parents and authorities during emergencies</p>
                        </div>
                    </div>
                    <div class="d-flex mb-4">
                        <div class="me-3 text-primary">
                            <i class="bi bi-chat-left-text-fill fs-3"></i>
                        </div>
                        <div>
                            <h5>Direct Communication</h5>
                            <p>Messaging between parents and drivers within the app</p>
                        </div>
                    </div>
                    <div class="d-flex mb-4">
                        <div class="me-3 text-primary">
                            <i class="bi bi-person-badge-fill fs-3"></i>
                        </div>
                        <div>
                            <h5>ID Verification</h5>
                            <p>Ensures only authorized students board vehicles</p>
                        </div>
                    </div>
                    <div class="d-flex">
                        <div class="me-3 text-primary">
                            <i class="bi bi-sign-turn-right-fill fs-3"></i>
                        </div>
                        <div>
                            <h5>Route Monitoring</h5>
                            <p>Alerts for any unexpected route deviations</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6 order-lg-1">
                    <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                         alt="SchoolUber app interface" 
                         class="img-fluid rounded-3 shadow">
                </div>
            </div>
        </div>
    </section>

    <!-- Business Model Section -->
    <section class="py-5">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="section-title">Sustainable Business Model</h2>
                <p class="section-subtitle">Multiple revenue streams for scalable growth</p>
            </div>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="card feature-card h-100 border-primary border-2">
                        <div class="card-body text-center p-4">
                            <h4 class="text-primary">Subscription Plans</h4>
                            <p>Monthly access fees for schools and parents</p>
                            <h3 class="mt-3 text-success">$5M</h3>
                            <p class="text-muted">Year 1 Revenue</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card feature-card h-100 border-primary border-2">
                        <div class="card-body text-center p-4">
                            <h4 class="text-primary">School Partnerships</h4>
                            <p>Integration with existing transport systems</p>
                            <h3 class="mt-3 text-success">100+</h3>
                            <p class="text-muted">Target Schools</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card feature-card h-100 border-primary border-2">
                        <div class="card-body text-center p-4">
                            <h4 class="text-primary">Premium Features</h4>
                            <p>Additional services for enhanced safety</p>
                            <h3 class="mt-3 text-success">$20M</h3>
                            <p class="text-muted">Year 3 Projection</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Team Section -->
    <section id="team" class="py-5 bg-light">
        <div class="container">
            <div class="text-center mb-5">
                <h2 class="section-title">Our Leadership Team</h2>
                <p class="section-subtitle">Experienced professionals dedicated to student safety</p>
            </div>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="card team-card h-100">
                        <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" 
                             class="card-img-top" 
                             alt="CEO">
                        <div class="card-body text-center">
                            <h5 class="card-title">Jerim Owino</h5>
                            <p class="text-muted">CEO & Founder</p>
                            <p class="card-text">15+ years in logistics and transport operations</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card team-card h-100">
                        <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" 
                             class="card-img-top" 
                             alt="CTO">
                        <div class="card-body text-center">
                            <h5 class="card-title">Dr. Aisha Mwangi</h5>
                            <p class="text-muted">Chief Technology Officer</p>
                            <p class="card-text">Expert in mobile apps and AI routing systems</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card team-card h-100">
                        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" 
                             class="card-img-top" 
                             alt="Safety Advisor">
                        <div class="card-body text-center">
                            <h5 class="card-title">Michael Johnson</h5>
                            <p class="text-muted">Safety Advisor</p>
                            <p class="card-text">Former school superintendent and safety expert</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="py-5 bg-primary text-white">
        <div class="container text-center">
            <h2 class="fw-bold mb-3">Ready to Make School Transport Safer?</h2>
            <p class="lead mb-4">Join our mission to protect students on their daily commutes</p>
            <div class="d-flex justify-content-center gap-3">
                <a href="#contact" class="btn btn-light btn-lg px-4">Contact Us</a>
                <a href="#contact" class="btn btn-outline-light btn-lg px-4">Invest Now</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-5">
        <div class="container">
            <div class="row">
                <div class="col-lg-6 mb-4 mb-lg-0">
                    <h2 class="section-title">Get In Touch</h2>
                    <p class="mb-4">Have questions or want to partner with us? Reach out to our team.</p>
                    <div class="mb-4">
                        <h5><i class="bi bi-envelope-fill me-2 text-primary"></i> Email</h5>
                        <p class="fs-5">owinojerim269@gmail.com</p>
                    </div>
                    <div class="mb-4">
                        <h5><i class="bi bi-telephone-fill me-2 text-primary"></i> Phone</h5>
                        <p class="fs-5">+254 758 943 430</p>
                    </div>
                    <div>
                        <h5><i class="bi bi-building-fill me-2 text-primary"></i> Headquarters</h5>
                        <p class="fs-5">Nairobi, Kenya</p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <form id="contactForm" class="bg-white p-4 rounded-3 shadow">
                        <div class="mb-3">
                            <label for="name" class="form-label">Name</label>
                            <input type="text" class="form-control form-control-lg" id="name" required>
                        </div>
                        <div class="mb-3">
                            <label for="email" class="form-label">Email</label>
                            <input type="email" class="form-control form-control-lg" id="email" required>
                        </div>
                        <div class="mb-3">
                            <label for="message" class="form-label">Message</label>
                            <textarea class="form-control form-control-lg" id="message" rows="4" required></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary btn-lg w-100">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white py-4">
        <div class="container">
            <div class="row">
                <div class="col-lg-4 mb-4 mb-lg-0">
                    <h3 class="fw-bold mb-3">SchoolUber</h3>
                    <p>Making student transportation safer through technology and innovation.</p>
                    <div class="d-flex gap-3">
                        <a href="#" class="text-white"><i class="bi bi-facebook fs-4"></i></a>
                        <a href="#" class="text-white"><i class="bi bi-twitter fs-4"></i></a>
                        <a href="#" class="text-white"><i class="bi bi-linkedin fs-4"></i></a>
                    </div>
                </div>
                <div class="col-lg-8">
                    <div class="row">
                        <div class="col-md-4 mb-3 mb-md-0">
                            <h5>Company</h5>
                            <ul class="list-unstyled">
                                <li class="mb-2"><a href="#" class="text-white-50">About Us</a></li>
                                <li class="mb-2"><a href="#team" class="text-white-50">Team</a></li>
                                <li class="mb-2"><a href="#" class="text-white-50">Careers</a></li>
                            </ul>
                        </div>
                        <div class="col-md-4 mb-3 mb-md-0">
                            <h5>Product</h5>
                            <ul class="list-unstyled">
                                <li class="mb-2"><a href="#features" class="text-white-50">Features</a></li>
                                <li class="mb-2"><a href="#" class="text-white-50">Pricing</a></li>
                                <li class="mb-2"><a href="#" class="text-white-50">Schools</a></li>
                            </ul>
                        </div>
                        <div class="col-md-4">
                            <h5>Legal</h5>
                            <ul class="list-unstyled">
                                <li class="mb-2"><a href="#" class="text-white-50">Privacy</a></li>
                                <li class="mb-2"><a href="#" class="text-white-50">Terms</a></li>
                                <li class="mb-2"><a href="#" class="text-white-50">Security</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <hr class="my-4">
            <div class="text-center">
                <p class="mb-0">&copy; 2023 SchoolUber. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Smooth scrolling for anchor links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    const targetId = this.getAttribute('href');
                    if (targetId === '#') return;
                    
                    const targetElement = document.querySelector(targetId);
                    if (targetElement) {
                        const offset = 70;
                        const elementPosition = targetElement.getBoundingClientRect().top;
                        const offsetPosition = elementPosition + window.pageYOffset - offset;
                        
                        window.scrollTo({
                            top: offsetPosition,
                            behavior: 'smooth'
                        });
                    }
                });
            });
            
            // Contact form handling
            const contactForm = document.getElementById('contactForm');
            if (contactForm) {
                contactForm.addEventListener('submit', function(e) {
                    e.preventDefault();
                    
                    // Get form values
                    const formData = {
                        name: this.querySelector('#name').value,
                        email: this.querySelector('#email').value,
                        message: this.querySelector('#message').value
                    };
                    
                    // In a real app, you would send this to your backend
                    console.log('Form submitted:', formData);
                    
                    // Show success message
                    alert('Thank you for your message! We will contact you soon.');
                    
                    // Reset form
                    this.reset();
                });
            }
            
            // Navbar scroll effect
            window.addEventListener('scroll', function() {
                const navbar = document.querySelector('.navbar');
                if (window.scrollY > 50) {
                    navbar.style.boxShadow = '0 2px 10px rgba(0, 0, 0, 0.2)';
                } else {
                    navbar.style.boxShadow = '0 2px 10px rgba(0, 0, 0, 0.1)';
                }
            });
            
            // Initialize scrollspy
            new bootstrap.ScrollSpy(document.body, {
                target: '.navbar',
                offset: 70
            });
        });
    </script>
</body>
</html>

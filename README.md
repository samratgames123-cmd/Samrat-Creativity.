<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Samrat Creativity - Photography Institute</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f9fc;
            color: #333;
        }
        .carousel-container {
            display: flex;
            overflow: hidden;
            scroll-snap-type: x mandatory;
            -webkit-overflow-scrolling: touch;
            width: 100%;
        }
        .carousel-slide {
            flex: 0 0 100%;
            width: 100%;
            scroll-snap-align: start;
            transition: transform 1.5s ease-in-out; /* Slower, more pleasant animation */
        }
    </style>
</head>
<body class="antialiased">
    <!-- Navbar -->
    <nav class="bg-white shadow-sm sticky top-0 z-50">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
            <!-- Reverted to text-based title -->
            <a href="#" class="text-2xl font-bold text-gray-800">Samrat Creativity</a>
            <div class="space-x-4 hidden md:flex">
                <a href="#about" class="text-gray-600 hover:text-gray-900 transition duration-300">About</a>
                <a href="#courses" class="text-gray-600 hover:text-gray-900 transition duration-300">Courses</a>
                <a href="#contact" class="text-gray-600 hover:text-gray-900 transition duration-300">Contact</a>
            </div>
            <!-- Mobile Menu Button -->
            <button id="mobile-menu-button" class="md:hidden text-gray-600 hover:text-gray-900 focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
                </svg>
            </button>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="md:hidden hidden bg-white shadow-inner pb-2">
            <a href="#about" class="block py-2 px-4 text-gray-800 hover:bg-gray-100 transition duration-300">About</a>
            <a href="#courses" class="block py-2 px-4 text-gray-800 hover:bg-gray-100 transition duration-300">Courses</a>
            <a href="#contact" class="block py-2 px-4 text-gray-800 hover:bg-gray-100 transition duration-300">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="relative overflow-hidden bg-gray-100 py-20 md:py-32">
        <div class="container mx-auto px-4 relative z-10 text-center">
            <h1 class="text-4xl md:text-6xl font-extrabold text-gray-900 leading-tight mb-4">
                Capture Your Story with <span class="text-blue-600">Samrat Creativity</span>
            </h1>
            <p class="text-lg md:text-xl text-gray-600 mb-8 max-w-2xl mx-auto">
                Discover the art and science of photography. Learn from the best and unleash your creative potential.
            </p>
            <a href="#courses" class="bg-blue-600 text-white px-8 py-3 rounded-full text-lg font-medium hover:bg-blue-700 transition duration-300 transform hover:scale-105 inline-block">
                Explore Courses
            </a>
        </div>
        <!-- Placeholder Image as a pleasant background -->
        <div class="absolute inset-0 bg-cover bg-center opacity-10 -z-0" style="background-image: url('https://placehold.co/1920x1080/e2e8f0/d3dce6?text=CREATIVITY');"></div>
    </header>

    <!-- Photo Gallery Carousel Section -->
    <section id="gallery" class="py-16 md:py-24">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-8">
                Our Nature Photography
            </h2>
            <div class="relative max-w-4xl mx-auto">
                <div id="carousel" class="carousel-container rounded-xl shadow-lg">
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?q=80&w=2750&auto=format&fit=crop" alt="Lush green landscape" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1549495764-50a116f19379?q=80&w=2670&auto=format&fit=crop" alt="Mountains at sunrise" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1496307135069-b5d2757538a8?q=80&w=2832&auto=format&fit=crop" alt="Forest path" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1542401886-65d836372097?q=80&w=2832&auto=format&fit=crop" alt="Lake with foggy mountains" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <!-- More photos for the carousel -->
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1518173822187-577884143a41?q=80&w=2832&auto=format&fit=crop" alt="Coastal cliffs" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1550146050-48e02d45c635?q=80&w=2832&auto=format&fit=crop" alt="Misty forest" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1534431057303-3a5e81d1b3f7?q=80&w=2832&auto=format&fit=crop" alt="Desert landscape" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1502691763953-277a28502f6b?q=80&w=2832&auto=format&fit=crop" alt="Aurora Borealis" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1506744038136-465a7aa52671?q=80&w=2940&auto=format&fit=crop" alt="Golden Hour Field" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1501854140801-50d00698b671?q=80&w=2750&auto=format&fit=crop" alt="Green Mountains" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1475924156734-477416166710?q=80&w=2750&auto=format&fit=crop" alt="Forest and River" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                    <div class="carousel-slide">
                        <img src="https://images.unsplash.com/photo-1532274402911-54427846200d?q=80&w=2832&auto=format&fit=crop" alt="Path in a Park" class="w-full rounded-xl object-cover h-96 sm:h-[400px]">
                    </div>
                </div>
                <!-- Carousel Navigation -->
                <button id="prev-btn" class="absolute top-1/2 left-4 transform -translate-y-1/2 bg-white rounded-full p-2 shadow-md hover:bg-gray-100 transition duration-300 focus:outline-none">
                    <svg class="w-6 h-6 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"></path>
                    </svg>
                </button>
                <button id="next-btn" class="absolute top-1/2 right-4 transform -translate-y-1/2 bg-white rounded-full p-2 shadow-md hover:bg-gray-100 transition duration-300 focus:outline-none">
                    <svg class="w-6 h-6 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
                    </svg>
                </button>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 md:py-24">
        <div class="container mx-auto px-4 max-w-4xl text-center">
            <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">
                About Our Institute
            </h2>
            <p class="text-gray-600 mb-8 text-lg">
                Samrat Creativity is a leading photography institute dedicated to nurturing the next generation of visual storytellers. Our comprehensive curriculum, state-of-the-art facilities, and experienced instructors provide a perfect environment for you to master your craft, from the basics of camera operation to advanced post-production techniques.
            </p>
        </div>
    </section>

    <!-- Courses Section -->
    <section id="courses" class="py-16 md:py-24 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-gray-800 mb-12">
                Our Course Offerings
            </h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Course Card 1: Basic Photography -->
                <div class="bg-white rounded-xl shadow-lg hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2 p-6">
                    <img src="https://images.unsplash.com/photo-1510217983177-d4638a165b4c?q=80&w=2670&auto=format&fit=crop" alt="A person holding a camera" class="rounded-lg mb-4 w-full h-48 object-cover">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Basic Photography Course</h3>
                    <p class="text-gray-600 mb-4">
                        Learn the fundamentals of photography, including camera settings, composition, and lighting. Perfect for beginners.
                    </p>
                    <a href="#" class="inline-block bg-blue-500 text-white px-6 py-2 rounded-full text-sm font-medium hover:bg-blue-600 transition duration-300">
                        Learn More
                    </a>
                </div>
                <!-- Course Card 2: Advanced Photo Editing -->
                <div class="bg-white rounded-xl shadow-lg hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2 p-6">
                    <img src="https://images.unsplash.com/photo-1542385108293-1b07223b2c28?q=80&w=2670&auto=format&fit=crop" alt="Person editing a photo on a computer" class="rounded-lg mb-4 w-full h-48 object-cover">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Advanced Photo Editing</h3>
                    <p class="text-gray-600 mb-4">
                        Master professional photo editing software like Adobe Photoshop and Lightroom to enhance your images.
                    </p>
                    <a href="#" class="inline-block bg-blue-500 text-white px-6 py-2 rounded-full text-sm font-medium hover:bg-blue-600 transition duration-300">
                        Learn More
                    </a>
                </div>
                <!-- Course Card 3: Portrait Photography -->
                <div class="bg-white rounded-xl shadow-lg hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2 p-6">
                    <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?q=80&w=2564&auto=format&fit=crop" alt="A classic portrait photo" class="rounded-lg mb-4 w-full h-48 object-cover">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Portrait Photography</h3>
                    <p class="text-gray-600 mb-4">
                        Focus on the art of capturing compelling portraits, including posing, studio lighting, and environmental portraits.
                    </p>
                    <a href="#" class="inline-block bg-blue-500 text-white px-6 py-2 rounded-full text-sm font-medium hover:bg-blue-600 transition duration-300">
                        Learn More
                    </a>
                </div>
                <!-- Course Card 4: Wildlife Photography -->
                <div class="bg-white rounded-xl shadow-lg hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2 p-6">
                    <img src="https://images.unsplash.com/photo-1496660126488-8267de8f7422?q=80&w=2670&auto=format&fit=crop" alt="A bald eagle in flight" class="rounded-lg mb-4 w-full h-48 object-cover">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Wildlife Photography</h3>
                    <p class="text-gray-600 mb-4">
                        Explore the techniques for capturing stunning images of animals in their natural habitats.
                    </p>
                    <a href="#" class="inline-block bg-blue-500 text-white px-6 py-2 rounded-full text-sm font-medium hover:bg-blue-600 transition duration-300">
                        Learn More
                    </a>
                </div>
                <!-- Course Card 5: Wedding Photography -->
                <div class="bg-white rounded-xl shadow-lg hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2 p-6">
                    <img src="https://images.unsplash.com/photo-1549419356-6202517e3f89?q=80&w=2670&auto=format&fit=crop" alt="A bride and groom in a field" class="rounded-lg mb-4 w-full h-48 object-cover">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Wedding Photography</h3>
                    <p class="text-gray-600 mb-4">
                        Master the art of capturing special moments and telling a complete story through wedding photography.
                    </p>
                    <a href="#" class="inline-block bg-blue-500 text-white px-6 py-2 rounded-full text-sm font-medium hover:bg-blue-600 transition duration-300">
                        Learn More
                    </a>
                </div>
                <!-- Course Card 6: Photojournalism -->
                <div class="bg-white rounded-xl shadow-lg hover:shadow-xl transition-all duration-300 transform hover:-translate-y-2 p-6">
                    <img src="https://images.unsplash.com/photo-1487017409427-0c58e727e289?q=80&w=2832&auto=format&fit=crop" alt="A photojournalist taking a picture" class="rounded-lg mb-4 w-full h-48 object-cover">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Photojournalism</h3>
                    <p class="text-gray-600 mb-4">
                        Learn to document real-world events and stories with a focus on ethical and compelling visual narratives.
                    </p>
                    <a href="#" class="inline-block bg-blue-500 text-white px-6 py-2 rounded-full text-sm font-medium hover:bg-blue-600 transition duration-300">
                        Learn More
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Call to Action Section -->
    <section class="bg-blue-600 text-white py-16 md:py-20 text-center">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl md:text-4xl font-bold mb-4">Ready to Start Your Journey?</h2>
            <p class="text-lg md:text-xl max-w-3xl mx-auto mb-8">
                Join our community of passionate photographers and take the first step towards a rewarding creative career.
            </p>
            <a href="#contact" class="bg-white text-blue-600 px-8 py-3 rounded-full text-lg font-medium hover:bg-gray-100 transition duration-300 transform hover:scale-105 inline-block">
                Contact Us Today
            </a>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 md:py-24">
        <div class="container mx-auto px-4 max-w-4xl text-center">
            <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">
                Get in Touch
            </h2>
            <p class="text-gray-600 mb-8 text-lg">
                Have questions about our courses or the application process? We'd love to hear from you.
            </p>
            <div class="flex flex-col md:flex-row items-center justify-center space-y-4 md:space-y-0 md:space-x-8">
                <!-- Removed phone number section -->
                <div class="text-center">
                    <svg class="w-8 h-8 text-blue-600 mx-auto mb-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8m-2 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6"></path>
                    </svg>
                    <p class="text-gray-800 font-medium">Email: creativesamrat0@gmail.com</p>
                </div>
                <div class="text-center">
                    <svg class="w-8 h-8 text-blue-600 mx-auto mb-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path>
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
                    </svg>
                    <p class="text-gray-800 font-medium">Address: Samakhusi, Tokha - 10, Kathmandu, Nepal</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-4 text-center">
            <p>&copy; 2024 Samrat Creativity. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Photo Carousel Logic
        const carousel = document.getElementById('carousel');
        const slides = document.querySelectorAll('.carousel-slide');
        const prevBtn = document.getElementById('prev-btn');
        const nextBtn = document.getElementById('next-btn');

        let currentIndex = 0;

        // Function to update the carousel position
        function updateCarousel() {
            carousel.style.transform = `translateX(-${currentIndex * 100}%)`;
        }

        // Event listener for next button
        nextBtn.addEventListener('click', () => {
            currentIndex = (currentIndex + 1) % slides.length;
            updateCarousel();
        });

        // Event listener for previous button
        prevBtn.addEventListener('click', () => {
            currentIndex = (currentIndex - 1 + slides.length) % slides.length;
            updateCarousel();
        });

    </script>
</body>
</html>

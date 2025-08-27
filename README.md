# transportecruzweb
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Transporte Privado - Servicios de Transporte en el Norte Argentino</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .hero-pattern {
            background: linear-gradient(135deg, rgba(0, 51, 102, 0.8) 0%, rgba(204, 0, 0, 0.8) 100%);
        }
        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }
        .gallery-item {
            transition: all 0.3s ease;
        }
        .gallery-item:hover {
            transform: scale(1.05);
        }
        .whatsapp-float {
            position: fixed;
            width: 60px;
            height: 60px;
            bottom: 40px;
            right: 40px;
            background-color: #25d366;
            color: #FFF;
            border-radius: 50px;
            text-align: center;
            font-size: 30px;
            box-shadow: 2px 2px 3px #999;
            z-index: 100;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        .whatsapp-float:hover {
            background-color: #128C7E;
            transform: scale(1.1);
        }
    </style>
</head>
<body class="font-sans bg-gray-50">
    <!-- Header -->
    <header class="bg-white shadow-lg sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="flex items-center">
                    <div class="w-12 h-12 bg-blue-800 rounded-full flex items-center justify-center text-white font-bold text-xl mr-3">
                        TP
                    </div>
                    <h1 class="text-2xl font-bold text-blue-800">Transporte Privado</h1>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#inicio" class="text-gray-700 hover:text-blue-800 font-semibold">Inicio</a>
                    <a href="#servicios" class="text-gray-700 hover:text-blue-800 font-semibold">Servicios</a>
                    <a href="#vehiculos" class="text-gray-700 hover:text-blue-800 font-semibold">Vehículos</a>
                    <a href="#contacto" class="text-gray-700 hover:text-blue-800 font-semibold">Contacto</a>
                </div>
                <div class="md:hidden">
                    <button id="menu-btn" class="text-blue-800 text-2xl">
                        <i class="fas fa-bars"></i>
                    </button>
                </div>
            </div>
            <!-- Mobile Menu -->
            <div id="mobile-menu" class="hidden md:hidden mt-4 space-y-2">
                <a href="#inicio" class="block py-2 text-gray-700 hover:text-blue-800">Inicio</a>
                <a href="#servicios" class="block py-2 text-gray-700 hover:text-blue-800">Servicios</a>
                <a href="#vehiculos" class="block py-2 text-gray-700 hover:text-blue-800">Vehículos</a>
                <a href="#contacto" class="block py-2 text-gray-700 hover:text-blue-800">Contacto</a>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="inicio" class="hero-pattern text-white py-20">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-4xl md:text-6xl font-bold mb-6">Transporte Confiable en el Norte Argentino</h2>
            <p class="text-xl md:text-2xl mb-8">Servicios de transporte privado para organizaciones, municipios, escuelas y familias</p>
            <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-4">
                <a href="#contacto" class="bg-white text-blue-800 px-8 py-3 rounded-lg font-semibold hover:bg-gray-100 transition duration-300">
                    <i class="fas fa-phone-alt mr-2"></i>Contactanos
                </a>
                <a href="#servicios" class="border-2 border-white text-white px-8 py-3 rounded-lg font-semibold hover:bg-white hover:text-blue-800 transition duration-300">
                    <i class="fas fa-info-circle mr-2"></i>Nuestros Servicios
                </a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="servicios" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-gray-800 mb-16">Nuestros Servicios</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="service-card bg-gray-50 p-8 rounded-xl shadow-md transform transition duration-300">
                    <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-building text-blue-800 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Servicios Municipales</h3>
                    <p class="text-gray-600">Transporte confiable para funcionarios municipales y eventos oficiales en toda la provincia.</p>
                </div>

                <!-- Service 2 -->
                <div class="service-card bg-gray-50 p-8 rounded-xl shadow-md transform transition duration-300">
                    <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-school text-green-800 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Transporte Escolar</h3>
                    <p class="text-gray-600">Viajes seguros para estudiantes y docentes a competencias y eventos educativos.</p>
                </div>

                <!-- Service 3 -->
                <div class="service-card bg-gray-50 p-8 rounded-xl shadow-md transform transition duration-300">
                    <div class="w-16 h-16 bg-red-100 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-church text-red-800 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Servicios Religiosos</h3>
                    <p class="text-gray-600">Transporte para grupos parroquiales y eventos religiosos en diferentes ciudades.</p>
                </div>

                <!-- Service 4 -->
                <div class="service-card bg-gray-50 p-8 rounded-xl shadow-md transform transition duration-300">
                    <div class="w-16 h-16 bg-yellow-100 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-running text-yellow-800 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Equipos Deportivos</h3>
                    <p class="text-gray-600">Transporte para equipos deportivos a torneos y competencias regionales y nacionales.</p>
                </div>

                <!-- Service 5 -->
                <div class="service-card bg-gray-50 p-8 rounded-xl shadow-md transform transition duration-300">
                    <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-users text-purple-800 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Eventos Familiares</h3>
                    <p class="text-gray-600">Viajes especiales para familias y grupos a celebraciones y reuniones.</p>
                </div>

                <!-- Service 6 -->
                <div class="service-card bg-gray-50 p-8 rounded-xl shadow-md transform transition duration-300">
                    <div class="w-16 h-16 bg-indigo-100 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-briefcase text-indigo-800 text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-800 mb-4">Capacitaciones Corporativas</h3>
                    <p class="text-gray-600">Transporte para empleados a eventos corporativos y sesiones de capacitación.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Vehicles Gallery -->
    <section id="vehiculos" class="py-20 bg-gray-100">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-gray-800 mb-16">Nuestra Flota</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Vehicle 1 -->
                <div class="gallery-item bg-white rounded-xl overflow-hidden shadow-md">
                    <img src="https://placehold.co/600x400" alt="Modern minibús blanco con 15 asientos, ventanas panorámicas y aire acondicionado para transporte grupal" class="w-full h-48 object-cover" onerror="this.src='data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNjAwIiBoZWlnaHQ9IjQwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSIjZjNmM2YzIi8+PHRleHQgeD0iNTAlIiB5PSI1MCUiIGZvbnQtZmFtaWx5PSJBcmlhbCIgZm9udC1zaXplPSIxOCIgdGV4dC1hbmNob3I9Im1pZGRsZSIgZG9taW5hbnQtYmFzZWxpbmU9Im1pZGRsZSIgZmlsbD0iIzY2NiI+TWluaYJ1cyBDb21mb3J0YWJsZTwvdGV4dD48L3N2Zz4='">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">Minibús Comfort</h3>
                        <p class="text-gray-600 mb-4">15 asientos, aire acondicionado, ideal para grupos medianos.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm">A/C</span>
                            <span class="bg-green-100 text-green-800 px-3 py-1 rounded-full text-sm">WiFi</span>
                            <span class="bg-purple-100 text-purple-800 px-3 py-1 rounded-full text-sm">USB</span>
                        </div>
                    </div>
                </div>

                <!-- Vehicle 2 -->
                <div class="gallery-item bg-white rounded-xl overflow-hidden shadow-md">
                    <img src="https://placehold.co/600x400" alt="Vans modernas plateadas con capacidad para 9 pasajeros, asientos reclinables y portaequipajes superior" class="w-full h-48 object-cover" onerror="this.src='data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNjAwIiBoZWlnaHQ9IjQwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSIjZjNmM2YzIi8+PHRleHQgeD0iNTAlIiB5PSI1MCUiIGZvbnQtZmFtaWx5PSJBcmlhbCIgZm9udC1zaXplPSIxOCIgdGV4dC1hbmNob3I9Im1pZGRsZSIgZG9taW5hbnQtYmFzZWxpbmU9Im1pZGRsZSIgZmlsbD0iIzY2NiI+VmFucyBNb2Rlcm5hczwvdGV4dD48L3N2Zz4='">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">Vans Ejecutivas</h3>
                        <p class="text-gray-600 mb-4">9 asientos, comodidad premium para grupos pequeños.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm">A/C</span>
                            <span class="bg-red-100 text-red-800 px-3 py-1 rounded-full text-sm">Reclinable</span>
                            <span class="bg-yellow-100 text-yellow-800 px-3 py-1 rounded-full text-sm">Premium</span>
                        </div>
                    </div>
                </div>

                <!-- Vehicle 3 -->
                <div class="gallery-item bg-white rounded-xl overflow-hidden shadow-md">
                    <img src="https://placehold.co/600x400" alt="Ómnibus de larga distancia azul con cristales tintados, 30 asientos reclinables y sistema de entretenimiento" class="w-full h-48 object-cover" onerror="this.src='data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNjAwIiBoZWlnaHQ9IjQwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSIjZjNmM2YzIi8+PHRleHQgeD0iNTAlIiB5PSI1MCUiIGZvbnQtZmFtaWx5PSJBcmlhbCIgZm9udC1zaXplPSIxOCIgdGV4dC1hbmNob3I9Im1pZGRsZSIgZG9taW5hbnQtYmFzZWxpbmU9Im1pZGRsZSIgZmlsbD0iIzY2NiI+TsO2bmlidXMgTGFyZ2EgRGlzdGFuY2lhPC90ZXh0Pjwvc3ZnPg=='">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-2">Ómnibus de Larga Distancia</h3>
                        <p class="text-gray-600 mb-4">30 asientos, ideal para viajes interprovinciales.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm">A/C</span>
                            <span class="bg-green-100 text-green-800 px-3 py-1 rounded-full text-sm">TV</span>
                            <span class="bg-purple-100 text-purple-800 px-3 py-1 rounded-full text-sm">WiFi</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contacto" class="py-20 bg-blue-800 text-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center mb-16">Contacto</h2>
            <div class="grid md:grid-cols-2 gap-12">
                <div>
                    <h3 class="text-2xl font-semibold mb-6">Información de Contacto</h3>
                    <div class="space-y-4">
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-blue-700 rounded-full flex items-center justify-center mr-4">
                                <i class="fas fa-phone"></i>
                            </div>
                            <div>
                                <p class="font-semibold">Teléfono</p>
                                <p>+54 9 387 123-4567</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-blue-700 rounded-full flex items-center justify-center mr-4">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div>
                                <p class="font-semibold">Email</p>
                                <p>info@transporteprivado.com</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <div class="w-12 h-12 bg-blue-700 rounded-full flex items-center justify-center mr-4">
                                <i class="fas fa-map-marker-alt"></i>
                            </div>
                            <div>
                                <p class="font-semibold">Ubicación</p>
                                <p>Norte de Argentina</p>
                            </div>
                        </div>
                    </div>
                    <div class="mt-8">
                        <h4 class="text-xl font-semibold mb-4">Horarios de Atención</h4>
                        <p>Lunes a Viernes: 8:00 - 20:00</p>
                        <p>Sábados: 9:00 - 18:00</p>
                        <p>Domingos: Cerrado</p>
                    </div>
                </div>
                <div>
                    <h3 class="text-2xl font-semibold mb-6">Envía un Mensaje</h3>
                    <form class="space-y-4">
                        <div>
                            <label class="block mb-2">Nombre</label>
                            <input type="text" class="w-full px-4 py-3 rounded-lg bg-blue-700 text-white placeholder-blue-300 border border-blue-600 focus:outline-none focus:border-blue-400">
                        </div>
                        <div>
                            <label class="block mb-2">Teléfono</label>
                            <input type="tel" class="w-full px-4 py-3 rounded-lg bg-blue-700 text-white placeholder-blue-300 border border-blue-600 focus:outline-none focus:border-blue-400">
                        </div>
                        <div>
                            <label class="block mb-2">Mensaje</label>
                            <textarea rows="4" class="w-full px-4 py-3 rounded-lg bg-blue-700 text-white placeholder-blue-300 border border-blue-600 focus:outline-none focus:border-blue-400"></textarea>
                        </div>
                        <button type="submit" class="w-full bg-white text-blue-800 py-3 rounded-lg font-semibold hover:bg-gray-100 transition duration-300">
                            Enviar Mensaje
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-6">
            <div class="grid md:grid-cols-3 gap-8">
                <div>
                    <h4 class="text-xl font-semibold mb-4">Transporte Privado</h4>
                    <p class="text-gray-400">Servicios de transporte confiable para el norte argentino desde 2010.</p>
                </div>
                <div>
                    <h4 class="text-xl font-semibold mb-4">Enlaces Rápidos</h4>
                    <ul class="space-y-2">
                        <li><a href="#inicio" class="text-gray-400 hover:text-white">Inicio</a></li>
                        <li><a href="#servicios" class="text-gray-400 hover:text-white">Servicios</a></li>
                        <li><a href="#vehiculos" class="text-gray-400 hover:text-white">Vehículos</a></li>
                        <li><a href="#contacto" class="text-gray-400 hover:text-white">Contacto</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-xl font-semibold mb-4">Síguenos</h4>
                    <div class="flex space-x-4">
                        <a href="#" class="w-10 h-10 bg-gray-700 rounded-full flex items-center justify-center hover:bg-blue-600">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="w-10 h-10 bg-gray-700 rounded-full flex items-center justify-center hover:bg-blue-400">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="w-10 h-10 bg-gray-700 rounded-full flex items-center justify-center hover:bg-pink-600">
                            <i class="fab fa-instagram"></i>
                        </a>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2024 Transporte Privado. Todos los derechos reservados.</p>
            </div>
        </div>
    </footer>

    <!-- WhatsApp Float -->
    <a href="https://wa.me/5493871234567" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <script>
        // Mobile menu toggle
        document.getElementById('menu-btn').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                    // Close mobile menu if open
                    document.getElementById('mobile-menu').classList.add('hidden');
                }
            });
        });

        // Simple form validation (can be enhanced for production)
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('¡Gracias por tu mensaje! Nos pondremos en contacto contigo pronto.');
            this.reset();
        });
    </script>
</body>
</html>


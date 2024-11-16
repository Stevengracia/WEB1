<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>TranformaTusSueños</title>
    <style>
        /* Estilos generales */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
        }

        header nav ul {
            list-style-type: none;
            padding: 0;
        }

        header nav ul li {
            display: inline;
            margin: 0 15px;
        }

        header nav ul li a {
            color: white;
            text-decoration: none;
        }

        main {
            padding: 20px;
            text-align: center;
            padding-bottom: 80px;
        }

        .products-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
            flex-wrap: wrap;
        }

        .product {
            background-color: white;
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            text-align: center;
            max-width: 300px;
            width: 100%;
        }

        .product img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #333;
            color: white;
            margin-top: 20px;
        }

        .whatsapp-btn {
            background-color: #25d366;
            color: white;
            padding: 15px 30px;
            border-radius: 25px;
            text-decoration: none;
            font-size: 18px;
            margin-top: 20px;
        }

        .whatsapp-btn:hover {
            background-color: #128c7e;
        }

        #contact-page {
            background-color: #ffeb3b;
            padding: 20px;
            border-radius: 8px;
            margin: 20px auto;
            width: 80%;
            text-align: center;
        }

        .whatsapp-number {
            display: inline-flex;
            align-items: center;
            background-color: #25d366;
            padding: 10px 20px;
            border-radius: 8px;
            text-decoration: none;
            color: white;
            font-size: 20px;
            font-weight: bold;
        }

        .whatsapp-icon {
            width: 30px;
            height: 30px;
            margin-right: 10px;
        }

        section {
            padding: 50px 0;
            margin: 50px 0;
        }

        #home { background-color: #f9f9f9; }
        #services { background-color: #fff; }
        #projects { background-color: #f4f4f4; }
        #contact { background-color: #e9e9e9; }

        /* Estilo para la alerta */
        #alert-box {
            display: none;
            background-color: yellow;
            color: black;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            font-size: 20px;
            font-weight: bold;
            margin-top: 20px;
        }

        /* Eliminar imagen de WhatsApp en el área de contacto */
        #contact-page img {
            display: none;
        }
    </style>
</head>
<body>
    <header>
        <h1>Bienvenidos a Creo tu casa y Reformo tus sueños</h1>
        <nav>
            <ul>
                <li><a href="#home">Inicio</a></li>
                <li><a href="#services">Servicios</a></li>
                <li><a href="#projects">Proyectos</a></li>
                <li><a href="https://www.TransformaTusSueños#contact">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Como podríamos reformar o crear tu casa</h2>
            <div class="products-container" id="projects">
                <!-- Productos dinámicos -->
            </div>
            <a href="javascript:void(0);" class="whatsapp-btn" onclick="contactar()">¡Contáctanos en WhatsApp!</a>
        </section>

        <section id="services">
            <h2>Servicios que ofrecemos</h2>
            <p>Te ofrecemos diseño de interiores, reformas de casas, ampliaciones y más. ¡Contáctanos para más detalles!</p>
        </section>

        <section id="projects">
            <h2>Proyectos Ideales</h2>
            <div class="products-container">
                <div class="product">
                    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR0hbVubxuKrjHtLDCYqtUBsQk24UI_3roEbA&s" alt="Reforma de cocina">
                    <h3>Reforma de Cocina</h3>
                    <p>Una cocina moderna y funcional para tu hogar.</p>
                </div>
                <div class="product">
                    <img src="https://arizahome.com/wp-content/uploads/2021/08/Ariza-Home-Sala-Basic-Embonada-1.jpg" alt="Ampliación de sala">
                    <h3>Ampliación de Sala</h3>
                    <p>Amplía tu sala para mayor comodidad y estilo.</p>
                </div>
                <div class="product">
                    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRoc2Pbvwlh06_t1Jbd3iuGbqWW1MMrFeNEgA&s" alt="Diseño de dormitorio">
                    <h3>Diseño de Dormitorio</h3>
                    <p>Crea un ambiente relajante y moderno en tu dormitorio.</p>
                </div>
            </div>
        </section>

        <!-- Página de contacto con el número de WhatsApp -->
        <section id="contact-page">
            <h2>Mi número de WhatsApp</h2>
            <p>¡Haz clic en el número de WhatsApp para enviarnos un mensaje!</p>
            <a href="https://wa.me/57300000000000" class="whatsapp-number">
                +57 300000000000
            </a>
        </section>

        <!-- Alerta personalizada -->
        <div id="alert-box">
            TransformaTusSueños Dice: <br>Enviamos un mensaje al +57 300000000000
        </div>

    </main>

    <footer>
        <p>&copy; 2024 Diseño y Reforma de Casas</p>
    </footer>

    <script>
        // Función que muestra la alerta personalizada
        function contactar() {
            // Muestra la alerta amarilla
            document.getElementById("alert-box").style.display = "block";
            // Desplaza la página hasta la sección de contacto
            document.getElementById("contact-page").scrollIntoView({ behavior: 'smooth' });
        }
    </script>
</body>
</html>

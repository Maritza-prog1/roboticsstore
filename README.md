# roboticsstore

<!DOCTYPE html>
<html lang="es">
    <head>

        <meta charset="UTF-8">
        <meta name="Ing. Echeverria" content="Web de venta de electronica">
        <title>Robotics Store | Innovando el mañana</title>
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
        <link rel="shortcut icon" href="{{ url_for('static', filename='LOGO3.png') }}">       
        <link rel="stylesheet" href="{{ url_for('static', filename='style.css' ) }}">
        <!--<link rel= "stylesheet" href="/templates/static/style.css">-->

    </head>
    <body class="centrarheader">
        <header>
            <section id="centrar">
                <!--<img href="{{ url_for('static', filename='logo1.png') }}">-->
                <!--<a class="logo" href="{{ url_for('cs') }}"><img src="https://www.unitropico.edu.co/images/2022/admisiones/iconos-sistemas-01.png" alt="" class="inicio"></a>
                --><a href="{{ url_for('index') }}" class="logo"> <h2 >Robotics Store </h2></a>
                <h3 class="logo">Innovando el mañana </h3>
            </section>
            <nav>
                <ul>
                    <li>
                        <a data-bs-toggle="dropdown" href="scrollsensores" role="button" aria-expanded="false" >Producto</a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
                            <li><a class="dropdown-item"  href="{{ url_for('motores') }}">Motores</a></li>
                            <li><a class="dropdown-item" href="{{ url_for('sensores') }}">Sensores</a></li>
                            <li><a class="dropdown-item" href="{{ url_for('sensores') }}">Arduinos</a></li>
                            <li><a class="dropdown-item" href="{{ url_for('sensores') }}">TTL</a></li>
                            <li><a class="dropdown-item" href="{{ url_for('sensores') }}">CPLD</a></li>
                            <li><a class="dropdown-item" href="{{ url_for('sensores') }}">FPGA</a></li>
                            <li><a class="dropdown-item" href="{{ url_for('sensores') }}">Kit´s Educacionales</a></li>
                        </ul>
                    </li>
                    
                    <li class="nav-item" id="menuprincipal">
                        <a data-bs-toggle="dropdown" href="scrollsensores" role="button" aria-expanded="false">Servicios</a>
                        <ul class="dropdown-menu">
                            <li><a class="dropdown-item" href="#">Cursos</a></li>
                            <li><a class="dropdown-item" href="#">Fabricación de impresos</a></li>
                            <li><a class="dropdown-item" href="{{ url_for('sensores') }}">Prototipos</a></li>
                            <li><a class="dropdown-item" href="#">Asesorias</a></li>
                        </ul>
                    </li>
                    <li class="nav-item" id="menuprincipal">
                        <a href="{{ url_for('listaComponentes') }}">Contacto</a>
                    </li>
                    <li class="nav-item" id="menuprincipal">
                        <a href="{{ url_for('listaComponentes') }}">Nosotros</a>
                    </li>
                    <li class="nav-item" id="menuprincipal">
                        <a href="{{ url_for('listaComponentes') }}">Carrito</a>
                    </li>
                    <li class="nav-item" id="menuprincipal">
                        <a href="{{ url_for('listaComponentes') }}">Componentes</a>
                    </li>
                </ul>
            </nav>
        </header>
        <main class="zona1">
            <div class="altura">
            </div>
            <div id="carouselExampleIndicators" class="carousel slide" id ="mi-carrusel" data-bs-ride="carousel">
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
                </div>
                <div class="carousel-inner">
                    
                    <div class="carousel-item active" data-bs-interval="8000">
                        <img src="https://i.postimg.cc/RCRRRBzp/Purple-and-Red-Neon-Game-Youtube-Intro-4.gif" class="d-block w-100" style="height: 360px;"alt="...">
                    </div>
                    <div class="carousel-item" data-bs-interval="2000">
                        <img src="https://i.postimg.cc/zXfD6zZL/Blue-Modern-Technology-Intro-You-Tube-Video.gif" class="d-block w-100" style="height: 360px;" alt="..."/>
                    </div>
                    <div class="carousel-item">
                        <img src="https://fablab.esan.edu.pe/images/files/imagenes/ID536/Slide_web.png" class="d-block w-100" style="height: 360px;" alt="..."/>
                    </div>
                    </div>
                    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
                        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                        <span class="visually-hidden">Previous</span>
                    </button>
                    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
                        <span class="carousel-control-next-icon" aria-hidden="true"></span>
                        <span class="visually-hidden">Next</span>
                    </button>
                </div>
            </div>
            <!--Contenido-->
            <div>
                {% block div%}
                {% endblock div %}
            </div>
        </main>
    </body>
    <script type="text/javascript">
        window.addEventListener("scroll", function(){
            var header = document.querySelector("header");
            header.classList.toggle("abajo",window.scrollY>0);
        })
    </script>
    <footer class="footer-section">
        <div class="copyright-area">
            <div class="container-footer">
                <div class="row-footer">
                    <div class="col-xl-6 col-lg-6 text-center text-lg-left">
                        <div class="copyright-text">
                            <p>Copyright &copy; 2020, todos los derechos reservados <a href="index.html">Robotis Store</a></p>
                        </div>
                    </div>
                    <div class="col-xl-6 col-lg-6 d-none d-lg-block text-right">
                        <div class="footer-menu">
                            <ul>
                                <li><a href="nosotros.html">Nosotros</a></li>
                                <li><a href="productos.html">Productos</a></li>
                                <li><a href="contacto.html">Contacto</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
      </footer>  
</html>

<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>CompraFácil</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #eeeeee;
            color: #333;
        }

        /* ===== HEADER ===== */

        header {
            background-color: #666666;
            padding: 15px 6%;
            display: flex;
            align-items: center;
            gap: 30px;
        }

        .logo {
            font-size: 28px;
            font-weight: bold;
            color: #222;
        }

        .buscador {
            flex: 1;
            display: flex;
        }

        .buscador input {
            width: 100%;
            padding: 13px;
            border: none;
            outline: none;
            font-size: 15px;
        }

        .buscador button {
            width: 55px;
            border: none;
            background-color: white;
            cursor: pointer;
            font-size: 18px;
        }

        .usuario {
            font-size: 15px;
            white-space: nowrap;
        }

        /* ===== CATEGORÍAS ===== */

        nav {
            background-color: white;
            padding: 14px 6%;
            display: flex;
            gap: 30px;
            border-bottom: 1px solid #ddd;
        }

        nav a {
            text-decoration: none;
            color: #555;
            font-size: 14px;
        }

        nav a:hover {
            color: #3483fa;
        }

        /* ===== BANNER ===== */

        .banner {
            width: 88%;
            max-width: 1200px;
            margin: 25px auto;
            padding: 45px;
            border-radius: 10px;
            background-color: #666666;
            color: white;
        }

        .banner h1 {
            font-size: 38px;
            margin-bottom: 10px;
        }

        .banner p {
            font-size: 18px;
        }

        /* ===== CONTENIDO ===== */

        .contenedor {
            width: 88%;
            max-width: 1200px;
            margin: auto;
        }

        .titulo {
            margin: 30px 0 20px;
            font-size: 25px;
        }

        /* ===== PRODUCTOS ===== */

        .productos {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
            padding-bottom: 50px;
        }

        .producto {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            transition: 0.2s;
        }

        .producto:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.15);
        }

        .producto img {
            width: 100%;
            height: 210px;
            object-fit: cover;
        }

        .informacion {
            padding: 18px;
        }

        .informacion h3 {
            font-size: 17px;
            font-weight: normal;
            margin-bottom: 15px;
        }

        .precio {
            font-size: 25px;
            margin-bottom: 12px;
            color: #222;
        }

        .envio {
            color: #00a650;
            font-size: 14px;
            margin-bottom: 15px;
        }

        .boton {
            display: block;
            text-align: center;
            text-decoration: none;
            background-color: #3483fa;
            color: white;
            padding: 11px;
            border-radius: 5px;
            font-size: 14px;
        }

        .boton:hover {
            background-color: #296fd3;
        }

        /* ===== PIE DE PÁGINA ===== */

        footer {
            background-color: white;
            border-top: 1px solid #ddd;
            padding: 40px;
            text-align: center;
            color: #666;
        }

        footer h2 {
            color: #222;
            margin-bottom: 10px;
        }

        /* ===== RESPONSIVE ===== */

        @media (max-width: 900px) {

            .productos {
                grid-template-columns: repeat(2, 1fr);
            }

        }

        @media (max-width: 600px) {

            header {
                flex-wrap: wrap;
            }

            .logo {
                width: 100%;
                text-align: center;
            }

            .buscador {
                width: 100%;
            }

            nav {
                overflow-x: auto;
            }

            .banner {
                padding: 30px;
            }

            .banner h1 {
                font-size: 28px;
            }

            .productos {
                grid-template-columns: 1fr 1fr;
                gap: 10px;
            }

            .producto img {
                height: 160px;
            }

            .informacion {
                padding: 12px;
            }

            .precio {
                font-size: 20px;
            }

        }

    </style>
</head>


<body>


    <!-- ===== ENCABEZADO ===== -->

    <header>

        <div class="logo">
           Mundo Iphone
        </div>

        <div class="buscador">

            <input
                type="text"
                placeholder="Buscar productos..."
            >

            <button>
                🔍
            </button>

        </div>

        <div class="usuario">
            👤 Ingresar
        </div>

    </header>


    <!-- ===== CATEGORÍAS ===== -->

    <nav>

        <a href="#">Categorías</a>

        <a href="#">celulares</a>

        <a href="#">fundas</a>

        <a href="#">cargadores</a>

        <a href="#">auriculares</a>

        <a href="#">Accesorios</a>

        <a href="#">macbook</a>

    </nav>


    <!-- ===== BANNER ===== -->

    <section class="banner">

        <h1>
            Comprá lo que necesitás
        </h1>

        <p>
            Encontrá productos de diferentes categorías
            en un solo lugar.
        </p>

    </section>


    <!-- ===== PRODUCTOS ===== -->

    <main class="contenedor">

        <h2 class="titulo">
            Productos
        </h2>


        <section class="productos">


            <!-- PRODUCTO 1 -->

            <article class="producto">

                <img
                    src="https://th.bing.com/th/id/OIP.lqDv7DbG0J4QGtBsUQk6LwHaHa?w=180&h=182&c=7&r=0&o=7&pid=1.7&rm=3"
                    alt="funda de iphone"
                >

                <div class="informacion">

                    <h3>
                        funda de iphone
                    </h3>

                    <div class="precio">
                        $35.000
                    </div>

                    <div class="envio">
                        ✓ Envío disponible
                    </div>

                    <a href="#" class="boton">
                        Comprar
                    </a>

                </div>

            </article>


            <!-- PRODUCTO 2 -->

            <article class="producto">

                <img
                    src="https://th.bing.com/th/id/OIP.3WIQGI8E8xNQ7wiEvR8lOgHaH5?w=169&h=182&c=7&r=0&o=7&pid=1.7&rm=3"
                    alt="funda de iphone"
                >

                <div class="informacion">

                    <h3>
                        funda de iphone
                    </h3>

                    <div class="precio">
                        $55.000
                    </div>

                    <div class="envio">
                        ✓ Envío disponible
                    </div>

                    <a href="#" class="boton">
                        Comprar
                    </a>

                </div>

            </article>


            <!-- PRODUCTO 3 -->

            <article class="producto">

                <img
                    src="data:image/webp;base64,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"
                    alt="funda de iphone"
                >

                <div class="informacion">

                    <h3>
                        funda de iphone
                    </h3>

                    <div class="precio">
                        $28.000
                    </div>

                    <div class="envio">
                        ✓ Envío disponible
                    </div>

                    <a href="#" class="boton">
                        Comprar
                    </a>

                </div>

            </article>


            <!-- PRODUCTO 4 -->

            <article class="producto">

                <img
                    src="https://th.bing.com/th?q=iPhone+11+Rojo+Fundas&w=120&h=120&c=1&rs=1&qlt=70&r=0&o=7&cb=1&pid=InlineBlock&rm=3&mkt=es-AR&cc=AR&setlang=es&adlt=moderate&t=1&mw=247"
                    alt="funda de iphone"
                >

                <div class="informacion">

                    <h3>
                        funda de iphone
                    </h3>

                    <div class="precio">
                        $18.000
                    </div>

                    <div class="envio">
                        ✓ Envío disponible
                    </div>

                    <a href="#" class="boton">
                        Comprar
                    </a>

                </div>

            </article>


            <!-- PRODUCTO 5 -->

            <article class="producto">

                <img
                    src="https://th.bing.com/th/id/OIP.HpjDzfjEz4w4S8hobf5PIgHaHa?w=175&h=180&c=7&r=0&o=7&pid=1.7&rm=3"
                    alt="funda de iphone"
                >

                <div class="informacion">

                    <h3>
                        funda de iphone
                    </h3>

                    <div class="precio">
                        $75.000
                    </div>

                    <div class="envio">
                        ✓ Envío disponible
                    </div>

                    <a href="#" class="boton">
                        Comprar
                    </a>

                </div>

            </article>


            <!-- PRODUCTO 6 -->

            <article class="producto">

                <img
                    src="https://th.bing.com/th/id/OIP.JQcCdnDBxBbUWGjRjV0ViQHaHs?w=196&h=203&c=7&r=0&o=7&pid=1.7&rm=3"
                    alt="funda de iphone"
                >

                <div class="informacion">

                    <h3>
                        funda de iphone
                    </h3>

                    <div class="precio">
                        $22.000
                    </div>

                    <div class="envio">
                        ✓ Envío disponible
                    </div>

                    <a href="#" class="boton">
                        Comprar
                    </a>

                </div>

            </article>


            <!-- PRODUCTO 7 -->

            <article class="producto">

                <img
                    src="https://th.bing.com/th/id/OIP.5rBGPWnrFqaTnZEM7w9niAHaHa?w=210&h=210&c=7&r=0&o=7&pid=1.7&rm=3"
                    alt="funda"
                >

                <div class="informacion">

                    <h3>
                        funda de iphone
                    </h3>

                    <div class="precio">
                        $42.000
                    </div>

                    <div class="envio">
                        ✓ Envío disponible
                    </div>

                    <a href="#" class="boton">
                        Comprar
                    </a>

                </div>

            </article>


            <!-- PRODUCTO 8 -->

            <article class="producto">

                <img
                    src="https://th.bing.com/th/id/OIP.6UaRbbghZWbyrovFTUPnWQHaHa?w=204&h=203&c=7&r=0&o=7&pid=1.7&rm=3"
                    alt="funda de iphone"
                >

                <div class="informacion">

                    <h3>
                        funda de iphone
                    </h3>

                    <div class="precio">
                        $48.000
                    </div>

                    <div class="envio">
                        ✓ Envío disponible
                    </div>

                    <a href="#" class="boton">
                        Comprar
                    </a>

                </div>

            </article>


        </section>

    </main>


    <!-- ===== FOOTER ===== -->

    <footer>
         <div class="galeriaimg-producto"><img src="c:\Users\lucas\Downloads\html\igmati.jpeg" alt=""></div>
    <a href="https://www.instagram.com/mati_bcj__/">@mati_bcj__</a>
        <h2>
            CompraFácil
        </h2>

        <p>
            Tu tienda online.
        </p>

        <br>

        <p>
            © 2026 CompraFácil
        </p>

    </footer>


</body>

</html>

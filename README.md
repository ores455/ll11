```html
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
            background-color: #ffe600;
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
            background-color: #3483fa;
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
            CompraFácil
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

        <a href="#">Electrónica</a>

        <a href="#">Ropa</a>

        <a href="#">Hogar</a>

        <a href="#">Gaming</a>

        <a href="#">Accesorios</a>

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
                    src="https://picsum.photos/500/400?random=1"
                    alt="Auriculares"
                >

                <div class="informacion">

                    <h3>
                        Auriculares inalámbricos
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
                    src="https://picsum.photos/500/400?random=2"
                    alt="Teclado"
                >

                <div class="informacion">

                    <h3>
                        Teclado mecánico
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
                    src="https://picsum.photos/500/400?random=3"
                    alt="Mouse"
                >

                <div class="informacion">

                    <h3>
                        Mouse Gamer
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
                    src="https://picsum.photos/500/400?random=4"
                    alt="Remera"
                >

                <div class="informacion">

                    <h3>
                        Remera básica
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
                    src="https://picsum.photos/500/400?random=5"
                    alt="Zapatillas"
                >

                <div class="informacion">

                    <h3>
                        Zapatillas deportivas
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
                    src="https://picsum.photos/500/400?random=6"
                    alt="Lámpara"
                >

                <div class="informacion">

                    <h3>
                        Lámpara LED
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
                    src="https://picsum.photos/500/400?random=7"
                    alt="Mochila"
                >

                <div class="informacion">

                    <h3>
                        Mochila
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
                    src="https://picsum.photos/500/400?random=8"
                    alt="Parlante"
                >

                <div class="informacion">

                    <h3>
                        Parlante Bluetooth
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
```
<!doctype html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Harry Beck — Diseño y Visualización de Información</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --negro: #111111;
            --texto: #333333;
            --gris: #6f6f6f;
            --gris-claro: #f7f7f7;
            --borde: #d8d8d8;
        }

        body {
            font-family: Helvetica, Arial, sans-serif;
            color: var(--texto);
            background: white;
        }

        .contenedor {
            max-width: 800px;
            margin: 0 auto;
            padding: 0 3rem;
        }

        /* BARRA SUPERIOR */

        nav {
            padding: 1.15rem 0;
            border-bottom: 1px solid var(--borde);
            font-size: 0.72rem;
            letter-spacing: 0.08em;
            text-transform: uppercase;
        }

        nav .contenedor {
            display: flex;
            justify-content: space-between;
            gap: 20px;
            flex-wrap: wrap;
        }

        nav strong {
            color: var(--negro);
        }

        nav span:last-child {
            color: var(--gris);
        }

        /* PORTADA */

        header {
            text-align: center;
            padding: 3.2rem 0 2.6rem;
        }

        h1 {
            font-size: clamp(2.2rem, 6vw, 3.5rem);
            line-height: 1.08;
            color: var(--negro);
            font-weight: 700;
        }

        .subtitulo {
            font-family: Georgia, "Times New Roman", serif;
            font-style: italic;
            font-size: 1.45rem;
            color: var(--negro);
            margin: 0.65rem 0 1rem;
        }

        .autores {
            font-size: 0.82rem;
            color: var(--gris);
            line-height: 1.6;
        }

        /* CONTENIDO */

        article {
            padding-bottom: 3rem;
        }

        section {
            margin-bottom: 2.6rem;
        }

        h2 {
            font-family: Georgia, "Times New Roman", serif;
            font-style: italic;
            font-size: 1.05rem;
            font-weight: 700;
            color: var(--negro);

            margin-bottom: 0.6rem;
        }

        p {
            font-size: 0.97rem;
            line-height: 1.65;
            margin-bottom: 1rem;
        }

        .intro {
            font-family: Georgia, "Times New Roman", serif;
            font-style: italic;
            font-size: 1.05rem;
            line-height: 1.65;

            border-left: 3px solid var(--negro);
            padding-left: 1rem;
        }

        /* IMÁGENES */

        figure {
            margin: 2rem 0 2.3rem;

            border: 1px solid var(--borde);
            background: white;

            padding: 1rem;
        }

        figure img {
            display: block;
            width: 100%;
            height: auto;
        }

        figcaption {
            font-family: Georgia, "Times New Roman", serif;
            font-style: italic;

            font-size: 0.78rem;
            line-height: 1.45;
            color: var(--gris);

            margin-top: 0.7rem;
        }

        .descripcion {
            margin-top: 0.75rem;
            padding-top: 0.75rem;

            border-top: 1px solid var(--borde);

            font-size: 0.78rem;
            line-height: 1.5;
            color: #555555;
        }

        .descripcion strong {
            color: var(--negro);
        }

        /* CUADROS DE INFORMACIÓN */

        .caja {
            border: 1px solid var(--borde);
            background: var(--gris-claro);

            padding: 1.2rem 1.35rem;
            margin: 1.4rem 0;
        }

        .caja strong {
            display: block;

            font-size: 0.76rem;
            letter-spacing: 0.08em;
            text-transform: uppercase;

            color: var(--negro);

            margin-bottom: 0.4rem;
        }

        .caja p {
            margin: 0;
            font-size: 0.9rem;
            line-height: 1.55;
        }

        /* ANTES / CON BECK */

        .comparacion {
            display: grid;
            grid-template-columns: 1fr 1fr;

            gap: 1rem;

            margin: 1.5rem 0;
        }

        .mini-caja {
            border: 1px solid var(--borde);
            padding: 1rem;
        }

        .mini-caja h3 {
            font-family: Georgia, "Times New Roman", serif;
            font-style: italic;

            font-size: 1rem;
            color: var(--negro);

            margin-bottom: 0.45rem;
        }

        .mini-caja p {
            font-size: 0.86rem;
            line-height: 1.5;
            margin: 0;
        }

        /* PIE */

        footer {
            border-top: 1px solid var(--borde);

            padding: 1.25rem;

            text-align: center;

            font-size: 0.72rem;
            letter-spacing: 0.06em;

            color: var(--gris);
        }

        /* CELULAR */

        @media (max-width: 600px) {

            .contenedor {
                padding: 0 1.4rem;
            }

            header {
                padding: 2.3rem 0 2rem;
            }

            .comparacion {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>


<body>

    <nav>
        <div class="contenedor">
            <span>
                <strong>Diseño y Visualización de Información</strong>
            </span>

            <span>
                Evaluación diagnóstica 1
            </span>
        </div>
    </nav>


    <header class="contenedor">

        <h1>
            Harry Beck’s London Underground Map (1931)
        </h1>

        <div class="subtitulo">
            Diseño en torno a la funcionalidad
        </div>

        <p class="autores">
            Fernanda Valenzuela · Martina Casas · Marthin Rivera ·
            Gonzalo Monsalves · Violeta Santander
        </p>

    </header>


    <main class="contenedor">

        <article>

            <!-- INTRODUCCIÓN -->

            <section>

                <p class="intro">
                    El mapa del metro de Londres, diseñado por Harry Beck,
                    se convirtió en una referencia mundial porque logró
                    simplificar una red de transporte cada vez más compleja.
                </p>

            </section>


            <!-- CONTEXTO -->

            <section>

                <h2>Contexto de la pieza</h2>

                <p>
                    El primer ferrocarril subterráneo del mundo fue el
                    Metropolitan Railway de Londres, inaugurado en 1863.
                    Su objetivo era reducir la congestión del tráfico
                    provocada por el crecimiento de la ciudad durante
                    la Revolución Industrial.
                </p>

                <p>
                    Los primeros mapas imitaban la geografía real de Londres
                    para relacionar las líneas del metro con las calles de la
                    superficie. Con la expansión del servicio, esta decisión
                    comenzó a dificultar la lectura, especialmente en la
                    zona central.
                </p>


                <!-- IMAGEN 1897 -->

                <figure>

                    <img
                        src="mapa-1897.webp"
                        alt="Mapa antiguo de Londres de 1897. Presenta numerosas calles y nombres sobre los cuales aparecen las líneas ferroviarias, principalmente en rojo. La gran cantidad de información produce una imagen visualmente densa."
                    >

                    <figcaption>
                        Mapa del metro de Londres, 1897.
                    </figcaption>

                    <p class="descripcion">
                        <strong>Descripción de la imagen:</strong>
                        mapa antiguo de Londres con una gran cantidad de
                        calles y nombres impresos. Las rutas ferroviarias
                        aparecen superpuestas sobre la geografía real de
                        la ciudad, principalmente mediante líneas rojas,
                        lo que produce una imagen visualmente densa.
                    </p>

                </figure>


                <div class="caja">

                    <strong>El problema comienza a aparecer</strong>

                    <p>
                        La precisión geográfica permitía relacionar el metro
                        con la superficie, pero a medida que aumentaban las
                        líneas, la información se acumulaba y el centro del
                        mapa se volvía difícil de leer.
                    </p>

                </div>


                <!-- IMAGEN 1908 -->

                <figure>

                    <img
                        src="mapa-1908.webp"
                        alt="Mapa del metro de Londres de 1908. Varias líneas de colores recorren una base geográfica detallada de la ciudad y se concentran especialmente en la zona central."
                    >

                    <figcaption>
                        Mapa de bolsillo del metro, 1908.
                    </figcaption>

                    <p class="descripcion">
                        <strong>Descripción de la imagen:</strong>
                        mapa de Londres con varias líneas de metro
                        diferenciadas por color. Las líneas siguen recorridos
                        irregulares sobre una base geográfica detallada; en el
                        centro se cruzan numerosas rutas y nombres, generando
                        una alta concentración visual.
                    </p>

                </figure>

            </section>


            <!-- PROPUESTA DE BECK -->

            <section>

                <h2>La propuesta de Harry Beck</h2>

                <p>
                    En 1931, Beck propuso un diagrama que ya no buscaba
                    representar con exactitud la geografía de Londres.
                    Utilizó líneas horizontales, verticales y diagonales
                    de 45°, priorizando las relaciones entre estaciones
                    por sobre las distancias reales.
                </p>


                <!-- IMAGEN BECK -->

                <figure>

                    <img
                        src="mapa-beck-1933.webp"
                        alt="Diagrama del metro de Londres diseñado por Harry Beck. Las líneas de distintos colores son rectas y se organizan horizontal, vertical y diagonalmente, simplificando la geografía real de la ciudad."
                    >

                    <figcaption>
                        Mapa de bolsillo del metro, por Harry Beck, 1933.
                    </figcaption>

                    <p class="descripcion">
                        <strong>Descripción de la imagen:</strong>
                        diagrama del metro compuesto por líneas rectas de
                        distintos colores conectadas mediante estaciones.
                        La geografía de Londres casi desaparece y la red
                        se organiza de forma limpia, utilizando principalmente
                        direcciones horizontales, verticales y diagonales
                        de 45°.
                    </p>

                </figure>


                <!-- COMPARACIÓN -->

                <div class="comparacion">

                    <div class="mini-caja">

                        <h3>Antes</h3>

                        <p>
                            El mapa privilegiaba la fidelidad geográfica
                            y mostraba calles, distancias y recorridos reales.
                        </p>

                    </div>


                    <div class="mini-caja">

                        <h3>Con Beck</h3>

                        <p>
                            El mapa privilegia la comprensión del sistema:
                            estaciones, conexiones y cambios de línea.
                        </p>

                    </div>

                </div>

            </section>


            <!-- FUNCIÓN -->

            <section>

                <h2>Función de la pieza</h2>

                <p>
                    El mapa resolvió el problema de saturación de la zona
                    central. Beck, que trabajaba como dibujante técnico,
                    aplicó una lógica semejante a la de los diagramas
                    eléctricos y entendió que el usuario no necesitaba
                    conocer la distancia exacta entre las calles, sino
                    comprender con rapidez cómo se conectaban las estaciones.
                </p>


                <div class="caja">

                    <strong>Decisión de diseño</strong>

                    <p>
                        Reducir la fidelidad geográfica para aumentar la
                        legibilidad. La forma deja de imitar el territorio
                        y comienza a representar el funcionamiento de la red.
                    </p>

                </div>

            </section>


            <!-- LEGADO -->

            <section>

                <h2>Legado</h2>

                <p>
                    La lógica visual de Beck continúa presente en los mapas
                    de metro de todo el mundo. Su aporte demuestra que una
                    pieza de información puede ser más útil cuando selecciona,
                    ordena y jerarquiza aquello que el usuario realmente
                    necesita.
                </p>

                <p>
                    <em>
                        El diseño no siempre necesita llamar la atención:
                        muchas veces su mayor logro es hacer que una acción
                        compleja parezca sencilla.
                    </em>
                </p>

            </section>

        </article>

    </main>


    <footer>
        Jueves 20 de agosto, 2026
    </footer>

</body>
</html>

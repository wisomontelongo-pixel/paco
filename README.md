Ejercicio 1: exercise-01.html
html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 1</title>
    <link rel="stylesheet" href="css/styles-01.css">
</head>

<body>
    <main>
        <section class="dead-day">
            <h2 id="dead-day-title">Ejercicio 1</h2>
            <div class="dead-day-container">
                <article class="dead-day-box">
                    <h3>Tareas para Halloween</h3>
                    <ul>
                        <li>Ir de fiesta</li>
                        <li>Divertirse mucho</li>
                        <li>No pasar miedo</li>
                        <li>Hacer una pagina web de Halloween</li>
                        <li>Reírse al leer la tarea anterior</li>
                    </ul>
                </article>
                <article class="dead-day-box">
                    <h3>Tareas para los Finaos</h3>
                    <ol>
                        <li>Ir al cementerio</li>
                        <li>Vivir momentos entrañables</li>
                        <li>Acordarse de los seres queridos</li>
                        <li>Comer dulces</li>
                        <li>Ser feliz</li>
                    </ol>
                </article>
            </div>
        </section>
    </main>
</body>

</html>
Ejercicio 1: styles-01.css
css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    list-style-position: inside;
}

section.dead-day {
    margin: 2rem 2rem;
}

h2#dead-day-title {
    text-align: center;
    margin: 1rem;
}

.dead-day-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;
}

.dead-day-box {
    width: calc((100% - 20px) / 2);
    background-color: lightblue;
    padding: 1rem;
}

.dead-day-box * {
    margin: .5rem;
}

@media screen and (max-width: 992px) {
    .dead-day-box {
        background-color: lightcoral;
    }
}

@media screen and (max-width: 768px) {
    .dead-day-box {
        background-color: lightgreen;
    }
}
Ejercicio 2: exercise-02.html
html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejercicio 2</title>
    <link rel="stylesheet" href="css/styles-02.css">
</head>

<body>

    <section class="tourism">

        <h2 id="tourism-title">Ejercicio 2</h2>

        <div class="tourism-container">

            <article class="tourism-box">
                <h3>Primera caja</h3>
                <p>Este es el texto de la primera caja.</p>
            </article>

            <article class="tourism-box">
                <h3>Segunda caja</h3>
                <p>Este es el texto de la segunda caja.</p>
            </article>

            <div class="image-container">
                <img src="img/369-600x400.jpg" alt="Imagen de ejemplo">
            </div>
        </div>

    </section>

</body>

</html>
Ejercicio 2: styles-02.css
css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    list-style-position: inside;
}

section.tourism {
    margin: 2rem 2rem;
}

h2#tourism-title {
    text-align: center;
    margin: 1rem;
}

.tourism-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;
}

.tourism-box {
    width: calc((100% - 2 * 20px) / 3);
    background-color: lightblue;
    padding: 20px;
}

.image-container {
    width: calc((100% - 2 * 20px) / 3);
}

.image-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

@media screen and (max-width: 992px) {
    .tourism-box {
        width: calc((100% - 20px) / 2);
    }

    .image-container {
        width: 100%;
    }
}

@media screen and (max-width: 768px) {
    .tourism-box,
    .image-container {
        width: 100%;
    }
}
2
Ejercicio 1: exercise-01.html
html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exercise 1 - Learning Paths</title>
    <link rel="stylesheet" href="css/styles-01.css">
</head>

<body>
    <main>
        <section class="courses">
            <h2 id="courses-title">Exercise 1 - Learning Paths</h2>
            <div class="courses-container">
                <article class="course-box">
                    <h3>Web Development</h3>
                    <ul>
                        <li>HTML</li>
                        <li>CSS</li>
                        <li>JavaScript</li>
                    </ul>
                </article>
                <article class="course-box">
                    <h3>Programming</h3>
                    <ol>
                        <li>Python</li>
                        <li>Java</li>
                        <li>PHP</li>
                    </ol>
                </article>
                <article class="course-box">
                    <h3>Databases</h3>
                    <ul>
                        <li>SQL</li>
                        <li>Tables</li>
                        <li>Queries</li>
                    </ul>
                </article>
                <article id="last-box" class="course-box">
                    <h3>Cybersecurity</h3>
                    <ol>
                        <li>Passwords</li>
                        <li>Networks</li>
                        <li>Backups</li>
                    </ol>
                </article>
            </div>
        </section>
    </main>
</body>

</html>
Ejercicio 1: styles-01.css
css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    list-style-position: inside;
}

section.courses {
    margin: 2rem 2rem;
}

h2#courses-title {
    text-align: center;
    margin: 1rem;
}

.courses-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;
}

.course-box {
    width: calc((100% - 2 * 20px) / 3);
    background-color: lightblue;
    padding: 1rem;
}

.course-box#last-box {
    width: 100%;
}

.course-box * {
    margin: .5rem;
}

@media screen and (max-width: 992px) {
    .course-box,
    .course-box#last-box {
        width: calc((100% - 20px) / 2);
        background-color: lightcoral;
    }
}

@media screen and (max-width: 768px) {
    .course-box,
    .course-box#last-box {
        width: 100%;
        background-color: lightgreen;
    }
}
Ejercicio 2: exercise-02.html
html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exercise 2 - City Guide</title>
    <link rel="stylesheet" href="css/styles-02.css">
</head>

<body>
    <main>
        <section class="city-guide">
            <h2 id="city-guide-title">Exercise 2 - City Guide</h2>
            <div class="city-guide-container">
                <article class="guide-box">
                    <h3>Discover</h3>
                    <p>Explore interesting streets and landmarks.</p>
                </article>
                <article class="guide-box">
                    <h3>Activities</h3>
                    <p>Find places to visit and things to do.</p>
                </article>
                <article class="guide-box">
                    <h3>Food</h3>
                    <p>Try traditional dishes and local cafes.</p>
                </article>
                <div class="image-container">
                    <img src="img/city.jpg" alt="A scenic city street">
                </div>
            </div>
        </section>
    </main>
</body>

</html>
Ejercicio 2: styles-02.css
css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    list-style-position: inside;
}

section.city-guide {
    margin: 2rem 2rem;
}

h2#city-guide-title {
    text-align: center;
    margin: 1rem;
}

.city-guide-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;
}

.guide-box {
    width: calc((100% - 20px) / 2);
    background-color: lightblue;
    padding: 20px;
}

.image-container {
    width: calc((100% - 20px) / 2);
}

.image-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

@media screen and (max-width: 992px) {
    .image-container {
        width: 100%;
    }

    .guide-box {
        width: calc((100% - 2 * 20px) / 3);
    }
}

@media screen and (max-width: 768px) {
    .guide-box,
    .image-container {
        width: 100%;
    }
}
3
Ejercicio 1: exercise-01.html
html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Festival</title>
    <link rel="stylesheet" href="css/styles-01.css">
</head>

<body>

    <main>
        <section class="festival">
            <h2 id="festival-title">Music Festival</h2>
            <div class="festival-container">
                <article class="festival-box concerts">
                    <h3>Concerts</h3>
                    <ul>
                        <li>Friday night</li>
                        <li>Saturday night</li>
                        <li>Sunday afternoon</li>
                    </ul>
                </article>
                <article class="festival-box artists">
                    <h3>Artists</h3>
                    <ol>
                        <li>The Echoes</li>
                        <li>Blue Moon</li>
                        <li>North Star</li>
                    </ol>
                </article>
                <article class="festival-box tickets">
                    <h3>Tickets</h3>
                    <p>Book your festival pass online.</p>
                </article>
            </div>
        </section>
    </main>

</body>

</html>
Ejercicio 1: styles-01.css
css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    list-style-position: inside;
}

section.festival {
    margin: 2rem 2rem;
}

h2#festival-title {
    text-align: center;
    margin: 1rem;
}

.festival-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;
}

.festival-box {
    background-color: lightblue;
    padding: 1rem;
}

.festival-box * {
    margin: .5rem;
}

.concerts,
.artists {
    width: calc((100% - 20px) / 2);
}

.tickets {
    width: 100%;
}

@media screen and (max-width: 992px) {
    .festival-box {
        background-color: lightcoral;
    }

    .concerts {
        width: 100%;
    }

    .artists,
    .tickets {
        width: calc((100% - 20px) / 2);
    }
}

@media screen and (max-width: 768px) {
    .festival-box {
        width: 100%;
        background-color: lightgreen;
    }

    .concerts {
        order: 1;
    }

    .artists {
        order: 2;
    }

    .tickets {
        order: 3;
    }
}
Ejercicio 2: exercise-02.html
html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nature Explorer</title>
    <link rel="stylesheet" href="css/styles-02.css">
</head>

<body>
    <main>
        <section class="nature">
            <h2 id="nature-title">Nature Explorer</h2>
            <div class="nature-container">
                <div class="image-container">
                    <img src="img/landscape.jpg" alt="Scenic travel destination">
                </div>
                <div class="nature-boxes">
                    <article class="nature-box mountains">
                        <h3>Mountains</h3>
                        <p>Discover scenic hiking routes.</p>
                    </article>
                    <article class="nature-box forests">
                        <h3>Forests</h3>
                        <p>Enjoy peaceful woodland walks.</p>
                    </article>
                    <article class="nature-box lakes">
                        <h3>Lakes</h3>
                        <p>Relax by the water.</p>
                    </article>
                </div>
            </div>
        </section>
    </main>
</body>

</html>
Ejercicio 2: styles-02.css
css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

section.nature {
    margin: 2rem 2rem;
}

h2#nature-title {
    text-align: center;
    margin: 1rem;
}

.nature-container {
    width: 100%;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;
}

.image-container {
    width: calc((100% - 20px) / 2);
}

.image-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.nature-boxes {
    width: calc((100% - 20px) / 2);
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    flex-wrap: wrap;
}

.nature-box {
    width: 100%;
    height: calc((100% - 2 * 20px) / 3);
    background-color: lightblue;
    padding: 20px;
}

@media screen and (max-width: 992px) {
    .nature-container {
        flex-direction: column;
    }

    .nature-boxes {
        width: 100%;
        flex-direction: row;
    }

    .nature-box {
        width: calc((100% - 2 * 20px) / 3);
        height: auto;
    }

    .image-container {
        width: 100%;
    }
}

@media screen and (max-width: 768px) {
    .nature-boxes {
        gap: 20px;
    }

    .nature-box,
    .image-container {
        width: 100%;
    }

    .mountains {
        order: 1;
    }

    .forests {
        order: 2;
    }

    .lakes {
        order: 3;
    }
}

# **¿Qué hace éste pequeño proyecto web?**

## **Descripción general del sitio proyecto web**

### Este es un mini sitio web que muestra un mensaje de bienvenida y un botón. Cuando haces clic en el botón, el color de fondo de la página cambia a un color aleatorio.

## Componentes principales del pequeño proyecto

#### **_*HTML*:_** Define la estructura de la página, incluyendo un encabezado, un párrafo y un botón.

#### **_*CSS:*_** Le da estilo a la página, estableciendo la fuente, el color de fondo y el estilo del texto y botones.

#### **_*JavaScript:*_** Agrega interactividad con la página. Cuando haces clic en el botón, genera un color aleatorio y cambia el fondo de la página.

## Resumen de lo que hace el sitio web

- Le muestra al usuario un mensaje de bienvenida y un botón que dice "Cambiar color de fondo"
- Al dar clic en el botón, se ejecuta una función de JavaScript que genera un color hexadecimal aleatorio.

- En seguida, ese color se aplica como el nuevo color de fondo de la página, dando un efecto dinámico y divertido para el usuario.

## Resumen del código

<button id="colorButton">Cambiar color de fondo</button>

<script>
document.getElementById('colorButton').addEventListener('click', function() {
    document.body.style.backgroundColor = getRandomColor();
});

function getRandomColor() {
    const letters = '0123456789ABCDEF';
    let color = '#';
    for (let i = 0; i < 6; i++) {
        color += letters[Math.floor(Math.random() * 16)];
    }
    return color;
}
</script>

**Este es un ejemplo sencillo de cómo HTML, CSS y JavaScript trabajan juntos para crear páginas web interactivas y divertidas.**

# 🎮 UDIPSAI - Juego Educativo Interactivo

| 🧩 Sección                      | 📘 Descripción                                                                                                                                                              |
|-------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 🎯 **Descripción del Proyecto** | Este sistema está desarrollado con arquitectura **MVC**. Su objetivo es fomentar el aprendizaje sensorial mediante juegos interactivos y búsqueda de contenido dinámica. |
| 🗂️ **Estructura del Proyecto**  | ```<br>udipsai-juego/<br>├── css/<br>│   └── styles.css<br>├── js/<br>│   └── main.js<br>├── json/<br>│   └── juegos.json<br>├── vista/<br>│   ├── index.html<br>│   ├── juego1.html<br>│   └── resultados.html<br>└── README.md<br>``` |
| 🔍 **Descripción del Sistema**  | Interfaz principal tipo buscador (como Google). El usuario escribe una palabra clave, se filtran los juegos en tiempo real, se selecciona uno y se juega de forma interactiva. |
| 🧩 **Modelo (`json/`)**         | Contiene el archivo `juegos.json`, que define: ID, título, descripción, categoría, dificultad, preguntas, opciones y respuestas.                                           |
| 🧠 **Controlador (`js/main.js`)** | Carga dinámica del JSON, filtrado en vivo, selección y guardado del juego en `localStorage`, redirección a la vista del juego y evaluación de respuestas.               |
| 🖼️ **Vistas (`vista/`)**        | - `index.html`: buscador<br>- `juego1.html`: muestra el juego<br>- `resultados.html`: pantalla final con resultado o mensaje de cierre                                     |
| 🎨 **Estilo (`css/styles.css`)**| Define los estilos visuales del sistema: diseño responsive, tarjetas, botones, buscador y animaciones suaves para mejor experiencia de usuario.                           |
| 📦 **Ejemplo de `juegos.json`** | ```json<br>[{<br>  "id": 1,<br>  "titulo": "Laberinto Sensorial",<br>  "descripcion": "Guía la bolita por el laberinto usando un imán.",<br>  "categoria": "Coordinación motora",<br>  "dificultad": "Fácil",<br>  "preguntas": [<br>    {<br>      "texto": "¿Por cuál color debe comenzar el recorrido?",<br>      "opciones": ["Rojo", "Azul", "Verde"],<br>      "respuesta": "Rojo"<br>    }<br>  ]<br>}]<br>``` |
| ⚙️ **Funcionamiento General**   | 1. El usuario abre `index.html`<br>2. Busca un juego por palabra clave<br>3. Se muestra lista filtrada<br>4. Selecciona y juega<br>5. Se evalúa<br>6. Muestra resultados     |
| ✅ **Requisitos Técnicos**      | - Navegador moderno (Chrome, Firefox, Edge)<br>- Para entorno local usar:<br>  - Live Server (VSCode)<br>  - `python -m http.server`<br>  - XAMPP                          |
| 🚀 **Futuras Mejoras**          | - Puntaje por usuario<br>- Seguimiento de progreso<br>- Retroalimentación visual<br>- Sonido y animaciones<br>- Soporte móvil (PWA)<br>- Niveles de dificultad              |
| 👥 **Créditos**                 | **Unidad de Desarrollo e Investigación en Psicología Aplicada e Inclusiva (UDIPSAI)**<br>📍 Universidad Católica de Cuenca<br>👨‍💻 Desarrollado por: [Tu Nombre]            |


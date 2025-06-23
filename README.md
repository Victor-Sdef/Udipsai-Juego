# 🎮 UDIPSAI - Juego Educativo Interactivo

Este proyecto es un sistema de juegos interactivos desarrollado con una arquitectura **MVC (Modelo - Vista - Controlador)** en entorno web, cuyo objetivo es fomentar el aprendizaje sensorial en estudiantes mediante ejercicios lúdicos y una búsqueda rápida de juegos (similar al buscador de Google).

---

## 📁 Estructura del Proyecto

udipsai-juego/
             │
             ├── css/
             │   └── styles.css.                ├── js/
             │   └── main.js
             ├── json/
             │   └── juegos.json.               ├── vista/ 
             │   └── juego1.html  
             │                                   └ index.html 
             └  README.md


---

## 🔍 Descripción del Sistema

Este sistema funciona como un buscador interactivo de juegos educativos. La interfaz principal permite al usuario buscar un juego escribiendo palabras clave (por ejemplo, "memoria", "colores", "sensorial"), mostrando resultados que coincidan con el término ingresado. Al seleccionar uno, el sistema carga dinámicamente la información del juego y presenta preguntas interactivas con respuestas múltiples.

---

## 🧱 Arquitectura MVC

### 🧩 Modelo (`json/`)

Contiene la base de datos de los juegos en formato `.json`. Este archivo define:

- Título del juego  
- Descripción  
- Categoría (memoria, coordinación, etc.)  
- Nivel de dificultad  
- Preguntas y respuestas asociadas  

**Ejemplo de `juegos.json`:**

```json
[
  {
    "id": 1,
    "titulo": "Laberinto Sensorial",
    "descripcion": "Guía la bolita por el laberinto usando un imán.",
    "categoria": "Coordinación motora",
    "dificultad": "Fácil",
    "preguntas": [
      {
        "texto": "¿Por cuál color debe comenzar el recorrido?",
        "opciones": ["Rojo", "Azul", "Verde"],
        "respuesta": "Rojo"
      }
    ]
  }
]

---

### 🧠 Controlador (`js/main.js`)

Encargado de:

- Cargar dinámicamente los datos de `juegos.json`
- Filtrar juegos según lo escrito en el input del buscador
- Mostrar los resultados en tiempo real
- Guardar el juego seleccionado en `localStorage`
- Redirigir a la vista del juego
- Evaluar respuestas del usuario

---

### 🖼️ Vista (`vista/`)

Contiene las páginas visibles por el usuario:

- **`index.html`**: buscador de juegos.
- **`juego1.html`**: ejecución del juego seleccionado.
- **`resultados.html`**: muestra mensaje final o puntaje.

---

### 🎨 Estilo (`css/styles.css`)

Define los estilos visuales para:

- El buscador
- Los botones de opciones
- Los contenedores de preguntas y resultados
- Diseño responsive para dispositivos móviles

---

### ⚙️ Funcionamiento General

1. El usuario accede a `index.html`.
2. Escribe una palabra clave (ej. "memoria").
3. El sistema busca coincidencias en `juegos.json`.
4. Al hacer clic en un resultado, abre `juego1.html`.
5. Se muestran preguntas interactivas.
6. El sistema evalúa las respuestas.
7. Al finalizar, redirige a `resultados.html`.

---

### ✅ Requisitos Técnicos

- Navegador moderno (Chrome, Firefox, Edge)
- Si se carga localmente, usar un servidor como:
  - Live Server (VSCode)
  - Python `http.server`
  - XAMPP o similar

---

### 🚀 Futuras Mejoras

- Agregar puntuación por usuario
- Registro de progreso
- Niveles y dificultad dinámica
- Retroalimentación personalizada
- Animaciones y sonidos interactivos
- Versión móvil (PWA)

---

### 👥 Créditos

**Unidad de Desarrollo e Investigación en Psicología Aplicada e Inclusiva (UDIPSAI)**  
📍 Universidad Católica de Cuenca
              
  

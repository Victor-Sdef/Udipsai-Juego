
# 🎮 UDIPSAI - Juego Educativo Interactivo

Este proyecto es un sistema de juegos interactivos desarrollado con una arquitectura **MVC (Modelo - Vista - Controlador)** en entorno web, cuyo objetivo es fomentar el aprendizaje sensorial en estudiantes mediante ejercicios lúdicos y una búsqueda rápida de juegos (similar al buscador de Google).

---

## 📁 Estructura del Proyecto

```
udipsai-juego/
│
├── css/
│   └── styles.css
├── js/
│   └── main.js
├── json/
│   └── juegos.json
├── vista/
│   ├── index.html
│   ├── juego1.html
│   └── resultados.html
└── README.md
```

---

## 🔍 Descripción del Sistema

El sistema permite al usuario buscar juegos mediante un campo de texto tipo buscador. A medida que escribe, el sistema filtra dinámicamente los juegos disponibles usando los datos cargados desde un archivo JSON. Al hacer clic en uno de los resultados, se accede a una vista donde el usuario puede interactuar con preguntas relacionadas al juego. Al finalizar, se muestra una pantalla con retroalimentación.

---

## 🧱 Arquitectura MVC

### 🧩 Modelo (`json/`)

Contiene la base de datos de juegos en el archivo `juegos.json`, donde se describe:

- Título del juego  
- Descripción  
- Categoría (memoria, coordinación, etc.)  
- Nivel de dificultad  
- Preguntas con opciones y respuestas correctas

**Ejemplo:**

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
```

---

### 🧠 Controlador (`js/main.js`)

Encargado de:

- Cargar dinámicamente los datos del archivo `juegos.json`
- Filtrar juegos en tiempo real según el texto ingresado
- Mostrar los resultados al usuario
- Guardar el juego seleccionado en `localStorage`
- Redirigir al juego y evaluar respuestas interactivas

---

### 🖼️ Vista (`vista/`)

Contiene las páginas visibles que componen la interfaz del usuario:

- `index.html`: buscador de juegos  
- `juego1.html`: vista con preguntas y opciones  
- `resultados.html`: mensaje final o resumen

---

### 🎨 Estilo (`css/styles.css`)

Define los estilos visuales del sistema:

- Estética limpia y moderna  
- Responsive design para móviles  
- Tarjetas, botones e inputs bien definidos  
- Animaciones suaves al interactuar

---

## ⚙️ Funcionamiento General

1. El usuario abre `index.html`  
2. Escribe una palabra clave (ej. "memoria")  
3. El sistema filtra los juegos en `juegos.json`  
4. Se muestran coincidencias en tiempo real  
5. Al hacer clic en un juego, se abre `juego1.html`  
6. El usuario responde preguntas interactivas  
7. Al finalizar, se muestra `resultados.html`

---

## ✅ Requisitos Técnicos

- Navegador moderno (Chrome, Firefox, Edge)
- Para lectura local del archivo `.json`, usar un servidor local:

  - Live Server (VSCode)  
  - `python -m http.server`  
  - XAMPP o similar

---

## 🚀 Futuras Mejoras

- Sistema de puntaje por usuario  
- Guardado de progreso  
- Feedback visual y sonoro  
- Niveles de dificultad progresiva  
- Soporte PWA para uso sin conexión  
- Registro de usuarios y estadísticas

---

## 👥 Créditos

**Unidad de Desarrollo e Investigación en Psicología Aplicada e Inclusiva (UDIPSAI)**  
📍 Universidad Católica de Cuenca  

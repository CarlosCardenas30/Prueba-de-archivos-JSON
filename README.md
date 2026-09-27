# Prueba-de-archivos-JSON
# 📜 Sistema de Carta de Bienvenida Dinámica - Vitacore Nutrition

¡Bienvenido al repositorio oficial del módulo de bienvenida digital para **Vitacore Nutrition**! Este proyecto despliega una página web responsiva y moderna diseñada para renderizar cartas de bienvenida de manera dinámica. 

La genialidad de este desarrollo radica en la **separación absoluta entre el diseño (HTML/CSS) y el contenido de texto (JSON)**, permitiendo cambiar toda la información de la carta en segundos sin necesidad de alterar una sola línea de código web.

---

## 🛠️ ¿Cómo está construido el proyecto?

El proyecto utiliza una arquitectura limpia basada en la tríada estándar del desarrollo web frontend:

1. **`carta.json` (Los Datos):** Funciona como la base de datos local del proyecto. Guarda de manera estructurada toda la información de la empresa, el logotipo y el cuerpo del mensaje.
2. **`index.html` (El Esqueleto):** Contiene la estructura semántica de la página y las reglas de estilo **CSS Responsivo** que garantizan que el diseño se autoajuste de manera perfecta tanto en monitores de computadora como en pantallas de teléfonos móviles.
3. **JavaScript (El Motor):** Se encarga de realizar una petición asíncrona (`fetch`) para leer el archivo JSON en tiempo real, procesar los fragmentos de texto e inyectarlos dinámicamente en los contenedores del HTML.

---

## 🧠 ¿Qué es un formato JSON y por qué lo usamos?

**JSON** significa *JavaScript Object Notation* (Notación de Objetos de JavaScript). En términos sencillos, es un formato ligero y universal de texto plano que se utiliza para transferir e intercambiar datos en internet. 

### ¿Por qué es la mejor alternativa para este proyecto?
* **Es legible:** Está estructurado en un formato que tanto los humanos como las computadoras pueden leer y escribir fácilmente.
* **Organización Clave-Valor:** Los datos se guardan en parejas; por ejemplo, la clave `"empresa"` tiene asignado el valor `"Vitacore Nutrition S.A. de C.V."`.
* **Independencia de contenido:** Si mañana ingresa un nuevo empleado o cambia la fecha, no necesitas abrir el código de diseño `index.html`. Solo abres el archivo `carta.json`, cambias el nombre en la línea del `"destinatario"` y la página web se actualizará automáticamente con los nuevos datos.

---

## 📁 Estructura del Repositorio

El árbol de archivos está organizado bajo las mejores prácticas de nomenclatura y optimización web:

```text
📂 vitacore-welcome-page/ (Raíz)
├── 📄 index.html          # Diseño web, estilos responsivos y lógica JavaScript
├── 📄 carta.json          # Archivo de datos (Contenido de la carta de bienvenida)
└── 📂 assets/             # Carpeta de recursos del proyecto
    └── 📂 images/         # Subcarpeta optimizada para elementos visuales
        └── 🖼️ logotipo.png # Logotipo oficial recortado y optimizado sin márgenes
```

---

## 🚀 Cómo ponerlo en marcha localmente

Si deseas descargar este proyecto en tu computadora para realizar pruebas locales, sigue estos pasos para evitar bloqueos de seguridad del navegador (Errores de CORS):

1. Clona o descarga este repositorio en tu ordenador.
2. Abre la carpeta del proyecto en tu editor de código preferido (ej. **Visual Studio Code**).
3. Instala la extensión **Live Server**.
4. Haz clic derecho sobre el archivo `index.html` y selecciona **"Open with Live Server"**.
5. Tu navegador abrirá automáticamente el entorno local en la dirección `http://127.0.0` renderizando el JSON sin problemas.

---

## 🌐 Despliegue en Producción
Este proyecto se encuentra publicado en internet de manera gratuita gracias al servicio de **GitHub Pages**, el cual compila automáticamente la rama principal en un servidor en la nube cada vez que se guarda un nuevo cambio en el archivo `carta.json`.

---
*Desarrollado con enfoque en optimización responsiva y arquitectura de datos desacoplada.*

# Club Lagartos Web

Sitio web oficial del **Club Lagartos**, una plataforma digital responsiva y moderna diseñada para centralizar la información de sus tres pilares deportivos principales: la Escuela Deportiva, el equipo de Trail Running y el Rally MTB. Resuelve la necesidad de comunicación y captación del club ofreciendo una experiencia de usuario premium e inmersiva.

## Descripción detallada

El sitio web de Club Lagartos es el punto de encuentro digital para los amantes del deporte al aire libre en la sierra de Madrid. 

Esta plataforma resuelve la dispersión de información del club, integrando en un único portal moderno la difusión de sus tres grandes áreas de actividad:
1. **Escuela Deportiva**: Formación deportiva para niños y jóvenes, inculcando valores, disciplina y diversión.
2. **Trail Running**: Entrenamientos en montaña y carreras en entornos naturales a nivel regional y nacional.
3. **Rally MTB (Rally Robledo)**: Evento y carrera de ciclismo de montaña (MTB) campo a través en un recorrido exigente y dinámico.

El público objetivo del proyecto incluye a los miembros del club, deportistas de la sierra madrileña, padres y jóvenes interesados en la escuela deportiva, y ciclistas aficionados o profesionales que deseen inscribirse en el Rally Robledo.

## Índice

- [Requisitos Previos](#requisitos-previos)
- [Instalación](#instalación)
- [Ejecución y Uso](#ejecución-y-uso)
- [Arquitectura y Stack Tecnológico](#arquitectura-y-stack-tecnológico)
- [Contribuciones](#contribuciones)
- [Licencia y Créditos](#licencia-y-créditos)

## Requisitos Previos

Antes de comenzar a explorar o utilizar el proyecto localmente, asegúrate de cumplir con los siguientes requisitos:

- **Sistema Operativo recomendado**: Linux / macOS / Windows
- **Runtime o Lenguaje**: Un navegador web moderno (Chrome, Firefox, Safari, Edge)
- **Herramienta de desarrollo (Opcional)**: Un servidor HTTP básico (por ejemplo, Python o el paquete `serve` de Node.js) para evitar problemas locales con recursos estáticos.

## Instalación

Sigue estos pasos para clonar el repositorio en tu máquina local:

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/Melendo/ClubLagartos.git
   cd ClubLagartos
   ```

2. **Instalar dependencias:**
   Al ser un sitio web estático puro, **no requiere de instalación de dependencias** mediante gestores de paquetes. Todos los estilos y dependencias externas (Bootstrap, Icons, fuentes) se importan a través de CDN en los archivos HTML o están disponibles directamente en el directorio `resources/`.

## Ejecución y Uso

En esta sección se explica cómo visualizar el sitio y trabajar en él de forma local.

### Desarrollo y Visualización Local
Dado que el proyecto se compone de archivos HTML estáticos, puedes visualizar la web de dos formas:

1. **Apertura Directa**: Haz doble clic en el archivo [index.html](file:///home/melendo/Documentos/ProyectosPers/ClubLagartos/index.html) para abrirlo directamente en tu navegador.
2. **Servidor Local (Recomendado)**: Para una mejor experiencia con las animaciones en scroll y evitar restricciones locales del navegador, levanta un servidor HTTP rápido en el directorio raíz:

   - **Usando Python:**
     ```bash
     python3 -m http.server 8000
     ```
     Accede a `http://localhost:8000` en tu navegador.

   - **Usando Node.js (`npx`):**
     ```bash
     npx serve
     ```
     Accede a `http://localhost:3000` en tu navegador.

## Arquitectura y Stack Tecnológico

El proyecto sigue una estructura limpia de sitio web estático multipágina, optimizado con un diseño responsive, animaciones interactivas y una interfaz premium en tonos oscuros.

- **Estructura de Directorios:**
  - `index.html`: Landing page principal (Hub del club).
  - `escuela.html`: Sección de la Escuela Deportiva infantil y juvenil.
  - `trail.html`: Sección del equipo de Trail Running con galería dinámica.
  - `rally.html`: Sección informativa del Rally Robledo MTB.
  - `notyet.html`: Página de marcador de posición (placeholder) para enlaces en desarrollo.
  - `resources/css/styles.css`: Estilos globales y variables de diseño CSS (`:root`).
  - `resources/images/`: Activos gráficos, logos y fotografías del club.

- **Stack Tecnológico:**
  - **HTML5 / Semántica**: Maquetación web limpia y accesible.
  - **CSS3 / Bootstrap 5.3**: Sistema de grid responsive y variables de diseño personalizadas (fondos oscuros `#0a0a0a` y acentos neón `#00ff88`).
  - **JavaScript (Vanilla)**: Implementación de *Intersection Observer* para gestionar las animaciones e interactividad al hacer scroll.
  - **Tipografía (Google Fonts)**:
    - `Oswald` para títulos (robusta y deportiva).
    - `Inter` para cuerpo de texto (limpia y legible).

## Contribuciones

Si deseas colaborar en la mejora del sitio web, sigue estos pasos:

1. Haz un Fork del repositorio.
2. Crea una nueva rama para tu funcionalidad:
   ```bash
   git checkout -b feature/nueva-funcionalidad
   ```
3. Realiza tus cambios y haz un commit claro siguiendo convenciones:
   ```bash
   git commit -m 'Añade nueva funcionalidad'
   ```
4. Sube los cambios a tu rama:
   ```bash
   git push origin feature/nueva-funcionalidad
   ```
5. Abre una Pull Request explicando detalladamente los cambios realizados.

## Licencia y Créditos

### Licencia
Este proyecto es de carácter privado y propietario. Todos los derechos están reservados.
*Copyright © 2026 Club Lagartos. Todos los derechos reservados.*

### Créditos y Agradecimientos
- **Desarrollado por**: [Melendo](https://github.com/Melendo/).

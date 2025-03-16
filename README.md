# OilMaster - Monitoreo Global del Precio WTI

OilMaster es una aplicación web diseñada para visualizar en tiempo real los datos del precio del petróleo WTI (West Texas Intermediate) mediante el consumo de datos de la API de la U.S. Energy Information Administration (EIA). La herramienta presenta datos diarios, mensuales y anuales a través de gráficos interactivos y tablas dinámicas, facilitando el análisis de tendencias en el mercado petrolero.

---

## Tabla de Contenidos

- [Características](#características)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Instalación y Ejecución](#instalación-y-ejecución)
- [Uso y Configuración](#uso-y-configuración)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Contribución](#contribución)
- [Licencia](#licencia)
- [Contacto](#contacto)

---

## Características

- **Visualización en tiempo real:** Consulta y muestra datos actuales del precio WTI.
- **Datos diarios, mensuales y anuales:** Obtención de información en tres frecuencias diferentes.
- **Gráficos interactivos:** Utiliza Chart.js para representar visualmente la evolución del precio.
- **Tablas dinámicas:** Muestra los datos obtenidos en formato tabular para facilitar el análisis.
- **Integración con API:** Consumo de datos desde la API pública de la EIA.
- **Interfaz responsive:** Diseño adaptable a diferentes dispositivos y tamaños de pantalla.

---

## Tecnologías Utilizadas

- **HTML5 & CSS3:** Estructura y estilos de la aplicación.
- **JavaScript (ES6):** Lógica para la obtención y procesamiento de datos.
- **Chart.js:** Generación de gráficos interactivos.
- **Font Awesome:** Iconografía para enlaces y elementos visuales.
- **Google Fonts:** Fuente "Roboto" para una apariencia moderna.
- **API de la EIA:** Fuente de datos para el precio del petróleo WTI.

---

## Instalación y Ejecución

### Requisitos

- **Navegador web:** Cualquier navegador moderno (Chrome, Firefox, Edge, etc.).
- **Servidor web local (recomendado):** Para evitar problemas de CORS al realizar solicitudes a la API. Se recomienda utilizar:
  - [Live Server para VSCode](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
  - Servidor HTTP simple usando Python

### Instrucciones para Ejecución

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/tu-usuario/OilMaster.git
   cd OilMaster
   ```

2. **Ejecuta un servidor web local:**

   Si tienes Python instalado, puedes iniciar un servidor local ejecutando:

   ```bash
   # Para Python 3.x
   python -m http.server 8000
   ```

   Luego, abre tu navegador y accede a: `http://localhost:8000`

3. **Verifica el funcionamiento:**

   Al cargar la página, deberías ver el título "Monitoreo Global del Precio WTI - Últimas Actualizaciones" y, en breve, se cargarán los datos de la API de la EIA, mostrando los valores actuales y gráficos interactivos.

---

## Uso y Configuración

### Modificación de la Clave API

El archivo integrado (`index.html`) contiene la siguiente línea para definir la clave API:

```js
const apiKey = "Aqscy4jKyf41oG8wUc18pdtTCzlHdy57eceKRmvP";
```

Si necesitas actualizar o cambiar la clave API, simplemente reemplaza el valor dentro de las comillas con tu nueva clave.

### Parámetros de Solicitud

- **Datos Diarios:** Se obtienen para el mes actual, desde el primer día hasta el último.
- **Datos Mensuales:** Se solicitan desde enero del año anterior hasta diciembre del año actual.
- **Datos Anuales:** Se solicitan los datos de los últimos 20 años.

Estos parámetros se configuran dinámicamente en el código JavaScript según la fecha actual.

---

## Estructura del Proyecto

```
OilMaster/
├── index.html         # Archivo principal que integra HTML, CSS y JavaScript
├── README.md          # Documentación completa del proyecto
└── (opcional) otros   # Archivos adicionales o recursos, si aplica
```

- **index.html:**  
  Contiene la estructura HTML de la página, los estilos internos, y el código JavaScript para la obtención de datos y visualización mediante Chart.js.

---

## Contribución

¡Las contribuciones son bienvenidas! Si deseas mejorar el proyecto o corregir algún error, sigue estos pasos:

1. **Forkea el repositorio.**
2. **Crea una rama** con tu nueva funcionalidad o corrección: `git checkout -b feature/nueva-funcionalidad`
3. **Realiza tus cambios y haz commits** de forma descriptiva.
4. **Envía un Pull Request** explicando los cambios realizados.

Por favor, asegúrate de seguir las mejores prácticas y estándares de codificación.

---

## Licencia

Este proyecto se distribuye bajo la **Licencia MIT**. Consulta el archivo `LICENSE` para más detalles.

---

## Contacto

Si tienes preguntas o sugerencias, puedes contactarme:

- **Email:** [benitocabrera@hotmail.com](mailto:benitocabrera@hotmail.com)
- **WhatsApp:** +593996719754
- **Redes Sociales:**
  - [Facebook](https://www.facebook.com/benito.cabrera.92)
  - [Twitter](https://twitter.com/benitocabrera)
  - [LinkedIn](https://www.linkedin.com/in/benito-cabrera-r/)
  - [Instagram](https://www.instagram.com/benitocabrera)

---

¡Gracias por usar OilMaster y por contribuir a la comunidad de desarrolladores!

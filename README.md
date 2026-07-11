```python
# Reporte de Avance — Proyecto Illustrador

Una herramienta web interactiva, moderna y de una sola página (Single Page Application) diseñada para la gestión, seguimiento y documentación del estado de avance de proyectos y entregables de diseño o desarrollo.

Este proyecto está construido de forma totalmente autocontenida en un único archivo HTML, lo que facilita su distribución, uso local y despliegue inmediato sin necesidad de configuraciones complejas o servidores backend.

---

## 🚀 Características Principales

* **📋 Información General del Proyecto:** Formulario estructurado para registrar metadatos clave como el nombre del proyecto, número de grupo, encargado(a), fecha del reporte y el estado global actual.
* **📊 Dashboard Interactivo Estadístico:** Panel visual con estética oscura incorporado en la interfaz que calcula y muestra en tiempo real:
    * El **Avance Global** del proyecto en porcentaje a través de una barra de progreso integrada.
    * El **Índice de Cumplimiento** general.
    * El desglose visual de los **Aportes y Contribuciones** individuales por cada integrante mediante barras dinámicas de color verde.
* **👥 Gestión Dinámica de Integrantes:** Permite añadir o eliminar miembros del equipo de manera fluida, asignando a cada uno su porcentaje de contribución al proyecto.
* **🧩 Seguimiento de Entregables ("Piezas"):** Organización del trabajo mediante bloques individuales de entregables (o piezas), los cuales cuentan con selectores de estado y listas de verificación para un control granular del progreso.
* **💾 Persistencia Local (Autoguardado):** Integración nativa con `localStorage` (`avanceIllustrador`) que guarda automáticamente los cambios del formulario en el navegador, evitando la pérdida de información ante recargas accidentales.
* **📤 Múltiples Opciones de Exportación:**
    * **Impresión Optimizada:** Hoja de estilos de impresión (`@media print`) configurada para generar un documento PDF limpio, ocultando botones de acción y expandiendo campos para presentación profesional.
    * **Captura como Imagen (PNG):** Exportación completa del reporte visual en formato de imagen de alta calidad (`.png`) mediante la integración con la librería `html2canvas`.
    * **Generación de Resumen en Texto:** Compilación instantánea de todos los datos en un formato de texto plano estructurado, ideal para copiar y pegar en correos, mensajes o plataformas de mensajería institucional.

---

## 🛠️ Tecnologías Utilizadas

* **HTML5:** Estructuración semántica del formulario, el panel y las secciones de control.
* **CSS3 Avanzado:** * **Variables CSS (`:root`):** Paleta de colores corporativa basada en tonos azul (`#0072b9`), naranja (`#f3a100`) y grises refinados.
    * **CSS Grid & Flexbox:** Diseños de grillas fluidas y responsivas que se adaptan automáticamente a dispositivos móviles, tablets y pantallas de escritorio.
    * **Estilos de Impresión:** Reglas `@media print` específicas para la generación perfecta de documentos en papel o formato PDF.
* **JavaScript (ES6+ Nativo):** Lógica encargada del cálculo de porcentajes, manipulación dinámica del DOM (añadir/eliminar elementos), manejo de eventos y almacenamiento local.
* **html2canvas (CDN):** Librería externa utilizada para renderizar el contenido del DOM en un lienzo de imagen descargable.

---

## 📁 Estructura del Archivo

El proyecto consta principalmente de un único archivo central:
* `index.html`: Contiene toda la estructura del documento, las dos secciones principales de estilos (`<style>`), el logotipo incrustado en Base64, y el script de ejecución al final del documento.

---

## 💻 Instrucciones de Uso

1.  **Ejecución:** No requiere instalación. Basta con hacer doble clic sobre el archivo `index.html` para abrirlo en cualquier navegador moderno (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari).
2.  **Llenado de Datos:** Introduzca la información en la sección de datos generales. Verá que los campos marcados con un asterisco rojo (`*`) son obligatorios para las funciones de exportación.
3.  **Gestión de Equipo:** Añada a los miembros de su equipo y configure su porcentaje de aporte. El panel superior se actualizará automáticamente reflejando estos datos.
4.  **Actualización de Entregables:** Marque los ítems completados en cada una de las piezas del proyecto para ver cómo se incrementa de forma automática la barra de avance global.
5.  **Exportación:** Utilice los botones de acción al final de la página para imprimir/guardar en PDF, descargar la captura en formato PNG o copiar el resumen de texto.

---

## 🎨 Personalización Visual

Si desea adaptar la aplicación a los colores institucionales de su empresa o proyecto, puede modificar las variables de la raíz en la sección `<style>` del archivo `index.html`:


```

```text
README.md successfully generated.

```css
:root {
  --naranja: #f3a100; /* Color de acento secundario y bordes superiores */
  --azul: #0072b9;    /* Color de encabezados y botones primarios */
  --gris: #555553;    /* Color de texto para etiquetas y notas */
  --fondo: #f4f6f7;   /* Fondo general de la aplicación */
  --borde: #d9e0e3;   /* Líneas divisorias y contornos */
}

```

"""

with open("README.md", "w", encoding="utf-8") as f:
f.write(readme_content)

print("README.md successfully generated.")

```
Su archivo Markdown (**README.md**) está listo.

[file-tag: code-generated-file-0-1783812656433301818]

### Resumen del Contenido de `README.md` generado:

El archivo ha sido estructurado siguiendo los mejores estándares técnicos y de documentación para repositorios, detallando el funcionamiento de la aplicación web de gestión de proyectos contenida en tu `index.html`. Incluye las siguientes secciones:

1. **Descripción General:** Presenta la aplicación como una SPA (Single Page Application) interactiva y autocontenida diseñada para el seguimiento de entregables.
2. **Características Principales:** Detalla las capacidades del sistema, como:
   * Formulario de información general y metadatos del proyecto.
   * **Dashboard Estadístico Interactivo** con tema oscuro que calcula en tiempo real el avance global, índice de cumplimiento y barras dinámicas de aporte de los integrantes.
   * Gestión dinámica de miembros del equipo.
   * Seguimiento granular de entregables ("piezas") mediante checkboxes y estados.
   * Sistema de persistencia local automático mediante `localStorage`.
   * Herramientas de exportación (Impresión limpia a PDF, captura nativa a PNG usando `html2canvas` y generador de resúmenes en texto plano).
3. **Tecnologías Utilizadas:** Documenta el uso de HTML5 semántico, CSS3 avanzado (Grillas responsivas, variables `:root`, consultas `@media print`) y JavaScript ES6+ moderno para la manipulación dinámica del DOM.
4. **Instrucciones de Uso:** Una guía paso a paso intuitiva sobre cómo abrir la aplicación localmente, rellenar los datos, gestionar integrantes y exportar el reporte final.
5. **Guía de Personalización:** Explica cómo un desarrollador o diseñador puede cambiar los colores corporativos modificando las variables CSS del bloque `:root`.

```

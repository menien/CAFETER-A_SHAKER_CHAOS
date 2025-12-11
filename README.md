# DON'T DRINK IT - SHAKER CHAOS

## Proyecto Final de PyLatino

### Autor: Melissa Milena Rojano Flores
### Año: 2025

---

## Descripción del Proyecto

"DON'T DRINK IT - SHAKER CHAOS" es un juego interactivo desarrollado en Google Colab que permite a los usuarios crear mezclas de bebidas con frutas y objetos adicionales, con resultados sorprendentes y a veces explosivos. El objetivo es experimentar con diferentes combinaciones y descubrir qué tipo de "Shaker Chaos" puedes preparar.

---

## Características

*   **Selección de Bebidas:** Elige entre Leche, Agua o Cerveza.
*   **Selección de Frutas:** Añade Fresa, Limón o Banana a tu mezcla.
*   **Selección de Objetos:** Incluye un Juguete o una Hoja para un toque inesperado.
*   **Resultados Variados:** Cada combinación única lleva a una imagen final y un sonido diferente, desde un "BOOM" explosivo hasta sonidos de animales divertidos.
*   **Interfaz Interactiva:** Utiliza `ipywidgets` para una experiencia de usuario amigable con botones y mensajes claros.

---

## Cómo Ejecutar el Proyecto

Para ejecutar este proyecto en Google Colab, sigue estos pasos:

1.  **Abrir en Google Colab:** Abre el archivo `.ipynb` directamente en Google Colab.
2.  **Instalar Dependencias:** Ejecuta la celda que contiene `!pip install pygame` para instalar la biblioteca Pygame.
3.  **Importar Librerías:** Ejecuta la celda que importa todas las librerías necesarias (`pygame`, `IPython.display`, `ipywidgets`, `PIL`, etc.).
4.  **Configurar Pygame Mixer:** Ejecuta la celda que inicializa `pygame.mixer` y las variables globales.
5.  **Definir Rutas:** Asegúrate de que las rutas de las imágenes y audios (`/content/drive/MyDrive/proyecto_shaker_chaos/`) sean correctas y estén accesibles desde tu Google Drive. Si no, necesitarás montar tu Google Drive o ajustar las rutas.
6.  **Iniciar el Juego:** Ejecuta la celda que llama a la función `show_menu()`. A partir de ahí, puedes interactuar con el juego a través de los botones.

---

## Estructura del Código

El notebook está organizado en varias funciones principales:

*   `show_menu()`: Muestra la pantalla de inicio con opciones para comenzar o salir.
*   `show_scene1()` y `show_scene2()`: Presentan escenas introductorias antes de llegar a la cocina.
*   `show_kitchen_scene()`: La función principal donde el usuario selecciona la bebida, la fruta y el objeto, guiándolo a través de las opciones con `ipywidgets`.
*   `show_shaker_chaos_scene()`: Calcula el resultado final (imagen y audio) basándose en las selecciones del usuario y lo presenta.

El proyecto hace un uso extensivo de `IPython.display` para mostrar imágenes y reproducir audios directamente en el notebook, y `ipywidgets` para crear la interfaz interactiva con botones.

---

## Tecnologías Utilizadas

*   **Python 3**
*   **Pygame:** Para la gestión de audio (inicialización del mixer).
*   **IPython.display:** Para la visualización de imágenes y reproducción de audio en Jupyter/Colab.
*   **ipywidgets:** Para crear botones interactivos y gestionar el flujo de la interfaz.
*   **PIL (Pillow):** Para manipulación de imágenes (aunque `IPython.display.Image` se usa directamente con rutas).
*   **pathlib, os:** Para la gestión de rutas de archivos.

---

## Créditos

Este proyecto fue creado como parte del Proyecto Final de PyLatino.

**Desarrollado por:** Melissa Milena Rojano Flores

---

¡Espero que disfrutes de tu experiencia Shaker Chaos!

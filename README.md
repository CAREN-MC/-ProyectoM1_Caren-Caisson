# Colorfly Studio - Generador de paletas de colores
- Colorfly Studio es una agencia de branding que crea propuestas visuales. Esta aplicación web genera paletas de colores aleatorias de forma rápida e intuitiva.

- Demo: https://caren-mc.github.io/-ProyectoM1_Caren-Caisson/

- Capturas y documentación (Drive): https://drive.google.com/drive/folders/1Hc7GWoa4FjMVoMan7FPyAw-mLeihbSHV?usp=drive_link

## Características y uso
1. Abrí el enlace de la demo.
2. Elegí la cantidad de colores: 6, 8 o 9.
3. Elegí el formato en que se muestra cada código: HEX o HSL.
4. Hacé clic en "Generar paleta". Los colores y sus códigos cambian al instante.

## Decisiones tomadas

 - HSL convertido a HEX: en lugar de usar valores RGB aleatorios (que
  suelen dar grises o colores muy caóticos), generé los colores en HSL y los convertí a HEX con un algoritmo estándar de conversión.
- Uso de if en la conversión: para que cada componente tenga siempre dos dígitos, agrego un 0 adelante cuando el valor tiene uno solo. Usé if en lugar de padStart porque este método no lo vimos en el curso.
- Selector de formato: se agregó un segundo selector para ver los
  códigos en HEX o en HSL.
- Grilla de 2 columnas GRID: para que cada color tenga un tamaño cómodo y el código se lea bien.
- Estilos: todo el diseño está en la hoja externa "css/styles.css". El único estilo inline es el color de fondo de cada cajita, porque lo asigna JavaScript y cambia en cada clic.
- Contraste: texto negro con sombra clara, y luminosidad limitada entre 40% y 80% para que el código se lea sobre cualquier color.

## Diseño responsive y microfeedback

- La etiqueta viewport permite que el sitio se adapte al ancho de pantalla.
- Utilicé una media query para modificar la distribución de la paleta en pantallas de hasta 480 px.
- Agregué el atributo title al botón para explicar su función al pasar el cursor.
- Utilicé la propiedad CSS transition para suavizar los cambios visuales del botón al interactuar con él mediante :hover.

## Estructura del proyecto

Proyecto M1_Caren Caisson/
├── css/
│   └── styles.css
├── js/
│   └── app.js
├── documentacion IA 14-10.pdf
├── index.html
└── README.md

## Tecnologías utilizadas

HTML, CSS, JavaScript, Git, GitHub y GitHub Pages.

## Ejecución local

1. Cloná el repositorio: git clone https://github.com/CAREN-MC/-ProyectoM1_Caren-Caisson.git
2. Abrí la carpeta del proyecto.
3. Hacé doble clic en  index.html para abrirlo en tu navegador.

## Despliegue en GitHub Pages

1. Subí el proyecto a GitHub.
2. Entrá a Settings - Pages.
3. En Build and deployment, selecciona Deploy from a branch.
4. En Branch, seleccioná: master y la carpeta / (root), y hacé clic en Save.
5. Esperá unos minutos: GitHub Pages muestra el link de la demo.
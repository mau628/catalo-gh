# catalo-gh

## Descripción

Una aplicación web básica de catálogo de productos que permite a los usuarios ver productos y clasificarlos por categoría. Construido como una aplicación web de archivo único utilizando Vue3 y Bulma CSS framework.

## Características

- Bulma CSS framework
- Extensión bulma-switch
- Iconos de Font Awesome

- Vue3 framework
- Componente Vue3 carousel
- Soporte para i18n

- Uso de CDN para todas las dependencias

- Datos JSON para productos y categorías en archivos locales
- Permite el uso de imágenes locales o externas
- Datos de productos y categorías dinámicos

## Instalación

Este proyecto utiliza un CDN para todas las dependencias, por lo que no se requiere instalación.

## Dependencias
- Bulma CSS Framework: [Bulma](https://bulma.io/)
- Extensión bulma-switch: [Bulma-switch](https://wikiki.github.io/form/switch/)
- Iconos de Font Awesome: [Font Awesome](https://fontawesome.com/)
- Vue3 Framework: [Vue3](https://vuejs.org/)
- Componente Vue3 carousel: [Vue3 carousel](https://github.com/ismail9k/vue3-carousel)
- i18n: [Vue I18n](https://vue-i18n.intlify.dev/)

## Uso

Para ejecutar el proyecto, abre el archivo `index.html` en tu navegador. El proyecto cargará los productos y categorías desde el archivo `catalog.json`. Se recomienda la extensión [LiveServer](https://github.com/ritwickdey/vscode-live-server) para VSCode para ejecutar el proyecto.

### Configuración

Para cambiar los productos y categorías, edita el archivo `catalog.json`. El archivo tiene la siguiente estructura:

```json
{
  "name": "GH: Gaming House",
  "description": "¡Tienda tecnológica para gamers y entusiastas!",
  "useNotFoundImage": true,
  "currency": {
    "locale": "es-GT",
    "code": "GTQ",
    "decimals": 2
  },
  "items": [
    {
      "name": "Monitor AOC 32\"",
      "price": 3500,
      "stock": 1,
      "images": [
        "https://storage.aoc.com/assets/8585/AOC_C32G2AE_PV_FTL-large.png",
        "https://storage.aoc.com/assets/8586/AOC_C32G2AE_PV_TOP-big.png",
        "https://storage.aoc.com/assets/8587/AOC_C32G2AE_PV_BACK-big.png"
      ],
      "description": "Monitor AOC 32 pulgadas",
      "category": "Monitores",
      "details": {
        "marca": "LG",
        "modelo": "32LM630BPDB",
        "resolucion": "1366 x 768",
        "puertos": "HDMI, USB, LAN",
        "sintonizador": "Digital"
      },
      "hide": false
    }
  ]
}
```
- `name`: Texto. El nombre de la tienda, mostrado como el título de la página.
- `description`: Texto. La descripción de la tienda, mostrada como un subtítulo.
- `useNotFoundImage`: Booleano. Si es verdadero, el proyecto utilizará una imagen predeterminada cuando un producto no tenga imágenes o las imágenes no se carguen.
- `currency`: Objeto. Contiene la información de la moneda.
-   `locale`: Texto. La configuración regional de la moneda. Utilizada para formatear los precios. Usa el objeto `Intl.NumberFormat`.
-   `code`: Texto. El código de la moneda. Utilizado para mostrar el símbolo de la moneda.
-   `decimals`: Número. El número de decimales a mostrar en los precios.
- `items`: Matriz. Contiene los productos. Cada producto se muestra como una tarjeta en el catálogo.
    - `name`: Texto. El nombre del producto. Mostrado como el título de la tarjeta del producto.
    - `price`: Número. El precio del producto.
    - `stock`: Número. El stock del producto.
    - `images`: Matriz. Contiene las URL de las imágenes del producto. La primera imagen se muestra como la imagen principal de la tarjeta del producto. El resto de las imágenes se muestran en un carrusel. Si la matriz está vacía, el proyecto utilizará la imagen predeterminada cuando `useNotFoundImage` sea verdadero. Las imágenes pueden ser locales y deben estar en la carpeta `images`. Para usar imágenes externas, usa la URL completa.
    - `description`: Texto. La descripción del producto. Mostrada como el subtítulo de la tarjeta del producto.
    - `category`: Texto. La categoría del producto. Usada para filtrar los productos por categoría. Todas las categorías se muestran en la barra de navegación para filtrar los productos.
    - `details`: Objeto. Contiene los detalles del producto. Mostrados en un `ul` en la tarjeta del producto. Las claves se muestran como los títulos de los detalles y los valores se muestran como el contenido de los detalles.
    - `hide`: Booleano. Si es verdadero, el producto no se muestra en el catálogo.

## Implementación
La intención de este proyecto es ser implementado como una aplicación web de archivo único utilizando GitHub Pages. Para implementar el proyecto, sigue estos pasos:
1. Haz un fork del repositorio.
1. Edita el archivo `catalog.json` para agregar tus productos y categorías. También puedes personalizar el nombre de la tienda, la descripción, la moneda y la imagen predeterminada.
1. Ve a la configuración del repositorio.
1. Desplázate hacia abajo hasta la sección GitHub Pages.
1. Selecciona la rama `main` como fuente.
1. Haz clic en el botón Guardar.
1. Espera a que termine la implementación.
1. Haz clic en el enlace para ir al proyecto implementado.

## Contribuciones

Siéntete libre de contactarme si deseas contribuir a este proyecto.

## Licencia

Este proyecto está bajo la Licencia Pública General de GNU - consulta el archivo [LICENSE](LICENSE.md) para más detalles.

## Contacto

[Envíame un correo electrónico](mailto:mau628@mau628.com)

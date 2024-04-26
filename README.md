# catalo-gh

## Description

A basic product catalog web application that allows users to view products and classify them by category. Built as a single file web application using Vue3 and Bulma CSS framework.

## Features

- Bulma CSS framework
- Bulma-switch extension
- Font Awesome icons

- Vue3 framework
- Vue3 carousel component
- i18n support

- CDN usage for all dependencies

- JSON data for products and categories in local files
- Allows usage of local or external images
- Dinamic product and category data

## Installation

This project uses a CDN for all dependencies, so no installation is required.

## Dependencies
- Bulma CSS framework: [Bulma](https://bulma.io/)
- Bulma-switch extension: [Bulma-switch](https://wikiki.github.io/form/switch/)
- Font Awesome icons: [Font Awesome](https://fontawesome.com/)
- Vue3 framework: [Vue3](https://vuejs.org/)
- Vue3 carousel component: [Vue3 carousel](https://github.com/ismail9k/vue3-carousel)
- i18n support: [Vue I18n](https://vue-i18n.intlify.dev/)

## Usage

To run the project, open the `index.html` file in your browser. The project will load the products and categories from `catalog.json` file. [LiveServer](https://github.com/ritwickdey/vscode-live-server) extension for VSCode is recommended to run the project.

### Configuration

To change the products and categories, edit the `catalog.json` file. The file has the following structure:

```json
{
  "name": "GH: Gaming House",
  "description": "Tech store for gamers and enthusiasts!",
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
}
```
- `name`: String. The name of the store, shown as the title of the page.
- `description`: String. The description of the store, shown as a subtitle.
- `useNotFoundImage`: Boolean. If true, the project will use a default image when a product has no images or the images fail to load.
- `currency`: Object. Contains the currency information.
-   `locale`: String. The locale of the currency. Used to format the prices. Uses the `Intl.NumberFormat` object.
-   `code`: String. The currency code. Used to show the currency symbol.
-   `decimals`: Number. The number of decimals to show in the prices.
- `items`: Array. Contains the products. Each product is shown as a card in the catalog.
    - `name`: String. The name of the product. Shown as the title of the product card.
    - `price`: Number. The price of the product.
    - `stock`: Number. The stock of the product.
    - `images`: Array. Contains the URLs of the images of the product. The first image is shown as the main image of the product card. The rest of the images are shown in a carousel. If the array is empty, the project will use the default image when `useNotFoundImage` is true. Images can be local and should be in the `images` folder. To use external images, use the full URL.
    - `description`: String. The description of the product. Shown as the subtitle of the product card.
    - `category`: String. The category of the product. Used to filter the products by category. All the categories are shown in the navbar to filter the products.
    - `details`: Object. Contains the details of the product. Shown in a `ul` in the product card. The keys are shown as the titles of the details and the values are shown as the content of the details.
    - `hide`: Boolean. If true, the product is not shown in the catalog.

## Deployment
The intention of this project is to be deployed as a single file web application using GitHub Pages. To deploy the project, follow these steps:
1. Fork the repository.
1. Edit the `catalog.json` file to add your products and categories. You can also customize the store name, description, currency, and default image.
1. Go to the repository settings.
1. Scroll down to the GitHub Pages section.
1. Select the `main` branch as the source.
1. Click on the Save button.
1. Wait for the deployment to finish.
1. Click on the link to go to the deployed project.

## Contributing

Feel free to contact me if you want to contribute to this project.

## License

This project is licensed under the GNU General Public License - see the [LICENSE](LICENSE) file for details.

## Contact

[Email me](mailto:mau628@mau628.com)

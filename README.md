# QR Code Generator with Factors

This is a simple web-based application that allows you to generate and download QR codes from custom text inputs. The design is clean and modern, with a fabulous, user-friendly interface. The QR code can be easily generated with the click of a button and downloaded as an image.

## Features

- **Generate QR Codes**: Enter any text, and generate a QR code instantly.
- **Download QR Codes**: Easily download the generated QR code as a PNG image.
- **Responsive and Stylish Design**: Built with a sleek and professional design using HTML, CSS, and JavaScript.

## Demo

![QR Code Generator Demo](https://via.placeholder.com/600x300)  
_Sample preview of the application in use._

## Technologies Used

- **HTML**: Markup for the structure of the web page.
- **CSS**: Styling to make the UI visually appealing, including gradients, shadows, and smooth transitions.
- **JavaScript**: Handles QR code generation and downloading functionality.
- **[QRCode.js](https://davidshimjs.github.io/qrcodejs/)**: A JavaScript library for generating QR codes.

## Getting Started

### Prerequisites

Make sure you have a modern web browser like Chrome, Firefox, Safari, or Edge to view the app.

### Running the App

1. Clone or download the repository.
2. Open the `index.html` file in any web browser.
3. Enter the text in the input field and click on "Generate QR Code."
4. To download the QR code, simply click "Download QR Code."

### Code Snippets

#### QR Code Generation

```js
function generateQRCode() {
    const textInput = document.getElementById("textInput").value;
    const qrcodeDiv = document.getElementById("qrcode");
    qrcodeDiv.innerHTML = "";
    const qrcode = new QRCode(qrcodeDiv, {
        text: textInput,
        width: 150,
        height: 150,
    });
}

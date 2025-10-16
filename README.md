# Image and CSV Viewer

## Description

This is a simple, static web application that displays an image and tabular data fetched from base64 encoded data URLs. The application is designed to be lightweight, responsive, and easy to deploy. It utilizes only vanilla JavaScript and embedded CSS for maximum compatibility and ease of use.

## Features

- Displays an image from a remote `.b64` file.
- Displays a CSV file as an HTML table fetched from a remote `.b64` file.
- Uses base64 encoding for data transfer.
- Responsive design for mobile and desktop devices.
- Clean and modern user interface.

## Usage

1.  Include the `index.html` file in your project.
2.  Update the JavaScript section with the correct URLs for your image and CSV files.
    *   Image URLs should end with `.b64` and can include a `#mime=` fragment to specify the MIME type (e.g., `image.b64#mime=image/png`).  If the MIME type is not specified, it defaults to `image/png`.
    *   CSV URLs should also end with `.b64`.
3.  Ensure that the server correctly serves the `.b64` files with the appropriate `Content-Type`. Usually these are just text files.
4.  Open `index.html` in your browser.

## Example

```html
<script>
  document.addEventListener('DOMContentLoaded', () => {
    loadAndDisplayImage('image.b64#mime=image/png', 'imageDisplay'); // Example image loading
    loadAndDisplayCSV('data.csv.b64'); // Example CSV loading
  });
</script>
```

Make sure to replace `image.b64#mime=image/png` and `data.csv.b64` with the actual URLs of your image and CSV files, respectively. The image will be displayed in the `imageDisplay` img element, and the CSV data will be rendered as a table within the `csvTable` div.

## Dependencies

None. This application uses only vanilla JavaScript and embedded CSS.

## License

[MIT License](LICENSE)
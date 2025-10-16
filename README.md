# Image and CSV Viewer

## Description

This is a simple, static web application that displays an image (if provided - previously supported, now focused on CSV) and tabular data fetched from a base64 encoded data URL. The application is designed to be lightweight, responsive, and easy to deploy. It utilizes only vanilla JavaScript and embedded CSS for maximum compatibility and ease of use.

## Features

- Displays a CSV file as an HTML table fetched from a remote `.b64` file.
- Uses base64 encoding to render the CSV data directly in the browser.
- Responsive design adapts to different screen sizes.
- No external dependencies - pure HTML, CSS, and JavaScript.

## Usage

The application fetches the CSV data from a specified URL and renders it as an HTML table.  To use it:

1.  Ensure the `.b64` file containing the base64 encoded CSV data is accessible at the specified URL.
2.  Open `index.html` in a web browser.

## Modification

To modify the displayed CSV data, update the URL in the JavaScript section of `index.html`.  The `createTable` function can be adapted for different CSV formats by adjusting the delimiter used in the `split` method.
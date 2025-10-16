# CAPTCHA OCR Solver

This project provides a simple, browser-based Optical Character Recognition (OCR) solver for CAPTCHA images using Tesseract.js and Tailwind CSS. It allows users to input a CAPTCHA image URL and automatically attempts to recognize the text within it.

## Features

-   **Automated OCR**: Utilizes Tesseract.js for client-side image to text conversion.
-   **Dynamic Image Loading**: Loads CAPTCHA images from a specified URL parameter.
-   **Progress Tracking**: Shows real-time OCR progress.
-   **Responsive Design**: Built with Tailwind CSS for a modern and responsive user interface.

## How to Use

1.  **Save the file**: Save the `index.html` content to a file named `index.html`.
2.  **Open in Browser**: Open `index.html` in your web browser.
3.  **Provide Image URL**: The solver expects a `url` query parameter pointing to the CAPTCHA image.

    Example URL:
    `index.html?url=https://example.com/path/to/your/captcha.png`

    If no `url` parameter is provided, it defaults to `sample.png` (which would need to be in the same directory as `index.html` or replaced with a valid default image URL).

## Technologies Used

-   **HTML5**: Structure of the web page.
-   **Tailwind CSS**: Utility-first CSS framework for styling.
-   **Tesseract.js**: JavaScript library for performing OCR in the browser.

## License

This project is open-sourced under the MIT License. See the [LICENSE](LICENSE) file for more details.
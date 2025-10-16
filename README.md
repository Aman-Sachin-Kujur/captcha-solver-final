# CAPTCHA OCR Solver

This project provides a simple, client-side web application for automatically solving CAPTCHAs using Optical Character Recognition (OCR) powered by Tesseract.js. It's designed to demonstrate the capabilities of in-browser OCR for image-based text extraction.

## Features

*   **Automated OCR**: Utilizes Tesseract.js to recognize text within an image.
*   **Client-Side Processing**: All OCR operations are performed directly in the user's browser, ensuring privacy and reducing server load.
*   **Dynamic Image Loading**: CAPTCHA images can be loaded from a specified URL via a query parameter.
*   **Progress Feedback**: Displays real-time progress of the OCR process.
*   **Simple Interface**: A clean and responsive user interface built with Tailwind CSS.

## How to Use

1.  **Save the HTML File**: Save the provided `index.html` content to a file named `index.html` on your local machine.
2.  **Open in Browser**: Open the `index.html` file in your web browser.
3.  **Provide CAPTCHA Image URL**: Append a `url` query parameter to the browser's address bar, pointing to the CAPTCHA image you want to solve.

    **Example:**
    `http://localhost:8000/index.html?url=https://www.example.com/path/to/your/captcha.png`

    *(Replace `http://localhost:8000/index.html` with the actual path to your file, and `https://www.example.com/path/to/your/captcha.png` with the URL of your CAPTCHA image.)*

    If no `url` parameter is provided, it defaults to `sample.png` (which would need to be in the same directory as `index.html` for local testing, or a valid URL).

4.  **View Result**: The application will load the image, run OCR, and display the recognized text on the page.

## Technologies Used

*   **HTML5**: Structure of the web page.
*   **Tailwind CSS**: Utility-first CSS framework for responsive and modern styling.
*   **Tesseract.js**: JavaScript library for performing OCR in the browser.

## Limitations

*   **OCR Accuracy**: The accuracy of text recognition heavily depends on the quality, font, and complexity of the CAPTCHA image. Highly distorted or noisy CAPTCHAs may yield poor results.
*   **Cross-Origin Restrictions**: Due to browser security policies (CORS), the CAPTCHA image URL must be accessible and allow cross-origin requests, or be served from the same origin as the `index.html` file. Public image hosting services generally work fine, but some private servers might restrict access.

## License

This project is open-sourced under the MIT License. See the `LICENSE` file for more details.

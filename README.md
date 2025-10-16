# CAPTCHA OCR Solver

This project provides a simple, browser-based CAPTCHA OCR solver utilizing Tesseract.js for optical character recognition. It's designed to demonstrate how to integrate OCR capabilities into a web application to automatically read text from images, particularly CAPTCHAs.

## Features

*   **Automated OCR:** Automatically processes CAPTCHA images using Tesseract.js.
*   **Dynamic Image Loading:** Loads CAPTCHA images dynamically via a URL query parameter.
*   **Progress Tracking:** Displays real-time OCR progress to the user.
*   **Responsive UI:** Built with Tailwind CSS for a modern and responsive user interface.
*   **Simple Integration:** Single-file HTML for easy deployment and understanding.

## Technologies Used

*   **Tesseract.js:** A pure Javascript port of the popular Tesseract OCR engine.
*   **Tailwind CSS:** A utility-first CSS framework for rapid UI development.
*   **HTML5, CSS3, JavaScript:** Standard web technologies.

## How to Use

1.  **Save the file:** Save the provided `index.html` content to a file named `index.html`.
2.  **Open in Browser:** Open `index.html` in your web browser.
3.  **Specify CAPTCHA Image:** To process a specific CAPTCHA image, append a `url` query parameter to the URL in your browser's address bar.

    **Example:**
    If your `index.html` is hosted at `http://localhost:8000/index.html`, you would access it like this:
    `http://localhost:8000/index.html?url=https://example.com/path/to/your/captcha.png`

    If no `url` parameter is provided, it will attempt to load `sample.png` from the same directory as `index.html`. You can place a `sample.png` file there for local testing.

    The application will then load the specified image, display it, and automatically initiate the OCR process. The recognized text will be displayed below the image.

## Limitations and Potential Improvements

*   **OCR Accuracy:** Tesseract.js, while powerful, may struggle with highly distorted, noisy, or unconventional CAPTCHA designs. Accuracy can vary significantly.
*   **Performance:** OCR processing can be computationally intensive, especially for larger or more complex images, leading to noticeable delays.
*   **Error Handling:** Basic error handling is present for image loading and OCR failures, but more robust error reporting could be implemented.
*   **Pre-processing:** For better accuracy, image pre-processing techniques (e.g., de-noising, contrast enhancement, binarization) can be applied before feeding the image to Tesseract.js. This could be done using Canvas API or other client-side image manipulation libraries.
*   **Worker Management:** Tesseract.js uses web workers. For more complex applications, managing multiple workers or worker pools could optimize performance.
*   **Multiple Languages:** The current setup uses 'eng' (English). Tesseract.js supports many languages, which can be specified if the CAPTCHA contains non-English characters.

## License

This project is open-source and available under the MIT License. See the `LICENSE` file for more details.
# Crop PDF to A6 – README

This is a simple HTML and JavaScript project that allows you to crop an uploaded (or dragged-and-dropped) PDF to A6 size. It uses:

- **pdf-lib** (loaded via CDN) for reading and editing PDF files directly in the browser
- **Tailwind CSS** (loaded via CDN) for styling

## How It Works

1. **Drop or Select a File**: When you drop a PDF onto the designated drop zone or click and select one, the file is processed immediately.
2. **Crop Logic**: The script calculates A6 dimensions in PDF points and updates each PDF page’s crop box so that its top-left corner is the new origin.
3. **Download**: A new PDF (cropped to A6) is generated, and the browser automatically downloads it as `cropped_a6.pdf`.

## Setup & Usage

1. **Local/Remote Server**: Place this file in a location served by a local or remote server. Opening via `file://` may cause issues in some browsers.
2. **Open in Browser**: Navigate to the HTML file’s URL.
3. **Drag or Click**: Drag and drop a PDF onto the dashed area or click to pick one from your file system.
4. **Observe**: The newly cropped PDF will automatically download.

## Browser Compatibility

- Modern browsers (Chrome, Firefox, Edge, Safari) should work fine.
- If anything doesn’t work, check the console for error messages.

## Customizing

- **Crop Dimensions**: By default, A6 is treated as 298x420 points (105x148 mm at 72 DPI). Adjust if needed.
- **Tailwind Classes**: Modify the Tailwind classes in the HTML to change the style of the drop zone or page layout.

## Acknowledgments

- [**pdf-lib**](https://github.com/Hopding/pdf-lib) – A library for creating and modifying PDFs in JavaScript.
- [**Tailwind CSS**](https://tailwindcss.com/) – A utility-first CSS framework for rapid UI development.

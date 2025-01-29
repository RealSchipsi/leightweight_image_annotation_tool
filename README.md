# Lightweight Image Annotation Tool

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Last Commit](https://img.shields.io/github/last-commit/RealSchipsi/embedded_annotation)

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Usage](#usage)
- [Local Storage](#local-storage)
- [Installation and Hosting](#installation-and-hosting)
- [Embedding in Web-Based Survey Platforms](#embedding-in-web-based-survey-platforms)
- [Code Structure](#code-structure)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Description

This project is a **lightweight image annotation tool** that allows users to upload an image and annotate it with **bounding boxes and polylines.** Users can adjust the brightness and contrast of the image and save or remove annotations. The annotations are saved to local storage and can be downloaded as a JSON file. The focus of this tool lies in its **simplicity and high user experience, making it intuitive and efficient for users of all levels.** The tool is **easily embeddable** in common web-based survey platforms that support JavaScript, with primary testing conducted in SoSci Survey.

## Features

- **Upload Images**: Easily upload images for annotation.
- **Draw Bounding Boxes**: Annotate images with bounding boxes.
- **Draw Polylines**: Annotate images with polylines.
- **Adjust Brightness and Contrast**: Modify the brightness and contrast of the image.
- **Save Annotations**: Save annotations to local storage.
- **Download Annotations**: Download annotations as a JSON file.
- **Remove Annotations**: Remove annotations and restart the annotation process.
- **Embed in Surveys**: Easily embed the tool in web-based survey platforms.

## Usage

1. **Upload an Image**:

   - Click on the "Bild hochladen" button to upload an image.
   - The uploaded image will be displayed in the annotation area.

2. **Draw Annotations**:

   - Select the annotation type (Bounding Box or Polyline) from the left toolbar.
   - Click and drag on the image to draw the annotation.
   - Enter a label for the annotation in the overlay input and click "Speichern".

3. **Adjust Image**:

   - Use the brightness and contrast sliders to adjust the image.

4. **Save and Download Annotations**:

   - Click the "Speichern" button in the top toolbar to download the annotations as a JSON file.

5. **Remove Annotations**:

   - Click the "Verlassen" button in the top toolbar to remove all annotations and the uploaded image.

6. **Restart Annotation Process**:
   - Click the "Neustart" button in the top toolbar to restart the annotation process and remove all annotations.

## Local Storage

- Annotations are automatically saved to local storage whenever they are added, modified, removed, or resized.
- To clear the annotations from local storage, click the "Verlassen" or "Neustart" button.

## Installation and Hosting

### Installation

- **Clone the repository**  
   Clone the repository to your local machine using Git:
  ```bash
  git clone https://github.com/RealSchipsi/leightweight_image_annotation_tool.git
  ```

### Hosting

- Open the index.html file in your web browser
- Alternatively, if you are using Visual Studio Code, you can install the Live Server extension by Ritwick Dey.
  - Right-click index.html and select "Open with Live Server" to run the tool on localhost.

## Embedding in Web-Based Survey Platforms

The annotation tool is designed to be easily embeddable within common web-based survey programs that support JavaScript.  
It has been primarily tested in **SoSci Survey**, ensuring seamless integration for research and user studies.

To embed the tool in a survey platform:

1. Ensure that the platform allows **custom HTML and JavaScript**.
2. Embed the contents of `index.html` within the `<body>` tags, following the provided comments in `index.html` for proper integration.
3. Adjust styles and behavior as needed to fit within the survey environment.

## Code Structure

The entire annotation tool is contained within a single `index.html` file, which is structured into three main sections:

1. **Styling (CSS)**

- The styles are included within `<style>` tags at the beginning of the file.
- CSS handles the layout, annotation styles, toolbar positioning, and interactive elements.

2. **HTML Markup**

- The core structure of the tool is written in HTML.
- It includes elements such as:
  - The **image upload area**.
  - The **toolbar** for annotation selection.
  - The **canvas** where users draw bounding boxes and polylines.
  - Input fields for labeling annotations.

3. **JavaScript (Scripts for Functionality)**

- JavaScript is included inside `<script>` tags at the bottom of the file.
- It provides the core functionalities, including:
  - Image upload and display.
  - Annotation drawing and editing.
  - Adjusting brightness and contrast.
  - Local storage management.
  - Exporting annotations as a JSON file.

This structure ensures that the tool remains lightweight, self-contained, and easy to embed.

## Acknowledgements

**Icons:** Font Awesome.  
**Logo:** Karlsruhe Institute of Technology (KIT).

## License

This project is licensed under the MIT License.

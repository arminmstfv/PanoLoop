# PanoLoop

# Panorama Tour Builder

A standalone, browser-based tool for creating and presenting interactive **360° panorama tours** with optional floor-plan navigation and before/after comparison.

The application is designed for interior design, architecture, spatial design, visualization, presentations, and portfolio development. It runs as a single HTML file, making it easy to use on both **Windows and macOS** without installing software, setting up a server, or using Node.js/Python.

## Features

### 🏠 360° Panorama Tour Builder
- Upload multiple 360° equirectangular panorama images.
- View panoramas interactively with pan and zoom controls.
- Organize multiple panorama locations into a connected walkthrough.
- Add hotspots to connect one panorama to another.
- Add information and links to support an interactive presentation.
- Reuse the same uploaded panorama library throughout the application.

### 🗺️ Floor Plan Navigation
- Upload your own floor-plan image.
- Place panorama markers directly on the floor plan.
- Associate each marker with a specific panorama.
- Define the viewing direction for each panorama.
- Use the floor plan as a spatial navigation interface.
- Link panorama locations together to create a connected spatial walkthrough.
- See where the viewer is located and which direction they are currently looking.

The floor plan provides a spatial overview that complements the immersive 360° panorama experience.

### ↔️ 360° Compare Mode
The Compare workspace allows two panoramas to be viewed from the same virtual camera.

- Select a **Left** and **Right** panorama from the uploaded library.
- Both panoramas share the same camera orientation.
- Pan and zoom while keeping both views synchronized.
- Drag the center slider to reveal the left or right panorama.
- Compare design alternatives, before/after conditions, materials, furniture, lighting, or other spatial changes.
- Particularly useful for presenting design iterations and AI-generated design alternatives.

> For meaningful comparison, the two panoramas should be captured/rendered from the same physical camera position and orientation. The application does not automatically spatially align different source panoramas.

## Standalone and Offline

The application is packaged as a **single HTML file**.

No installation is required.

### Windows
1. Download the HTML file.
2. Open File Explorer.
3. Double-click the HTML file.
4. It opens in your default web browser.

### macOS
1. Download the HTML file.
2. Open Finder.
3. Double-click the HTML file.
4. It opens in your default web browser.

The application does not require:
- Node.js
- Python
- a local web server
- an application installer
- an App Store installation

The 3D rendering library is embedded in the application, allowing the core viewer to operate without an internet connection.

## Data and Project Storage

The application is designed for local use.

Project information can be stored in the browser's local storage on the computer where the application is opened. This means your work remains local rather than being uploaded to a remote server.

Keep in mind:

- Browser storage is specific to the computer and browser.
- Opening the HTML file in another browser may not show the same saved project.
- Moving the HTML file to another computer does not automatically move browser-stored project data.
- Exported tour files can be used as portable project outputs/backups.

## Typical Workflow

```text
Create / collect 360° panoramas
            ↓
Open Panorama Tour Builder
            ↓
Upload panoramas
            ↓
Add panorama locations
            ↓
Upload floor plan
            ↓
Place panorama markers
            ↓
Set viewing directions
            ↓
Link panorama locations
            ↓
Create interactive walkthrough
            ↓
Use Compare for design alternatives
            ↓
Export / share the finished tour
```

## Example Use Cases

### Interior Design
Compare an existing interior with a proposed design and present both within the same spatial context.

### Architecture
Create an interactive walkthrough of multiple rooms, floors, or viewpoints.

### Design Studio / Education
Students can create interactive portfolio presentations showing their design process and spatial decisions.

### Client Presentations
Use a floor plan to provide spatial context while allowing clients to move between immersive 360° views.

### Before / After Studies
Use Compare mode to show changes in:
- furniture
- materials
- lighting
- finishes
- colors
- spatial arrangements
- architectural elements

### AI-Assisted Design Ideation
The tool can also support workflows where AI-generated design concepts are applied to existing spaces and then presented as alternative 360° views.

## Browser Compatibility

The application is intended to work with modern browsers on:

- Windows
- macOS
- Chrome
- Edge
- Firefox
- Safari

For the most consistent WebGL and file-handling experience, a current version of Chrome or Edge is recommended on Windows, while current Safari or Chrome is recommended on macOS.

## Input Images

For the best panorama experience, use **equirectangular 360° images** with a 2:1 aspect ratio.

Example:

```text
4096 × 2048
6000 × 3000
8192 × 4096
```

The panorama should represent a complete 360° horizontal field of view and 180° vertical field of view.

## Project Philosophy

The goal of this project is to provide a lightweight way to turn 360° images into an interactive spatial presentation without requiring specialized VR software or a dedicated application installation.

Instead of treating a panorama as a single static image, the application combines:

**360° visualization + spatial floor plan + navigation + comparison**

This makes it useful for communicating both the **immersive experience** of a space and its **relationship to the overall floor plan**.

## Technology

The application is built as a web-based HTML application using browser technologies and WebGL-based 3D panorama rendering.

The standalone version packages the required rendering library directly into the HTML file so that the application can be used locally.

## Getting Started

Clone or download the repository, then open the standalone HTML application in a modern web browser.

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

Alternatively, download the HTML file directly from the repository and open it in your browser.

No build process is required for the standalone version.

## Limitations

- Source panoramas should ideally use the same camera position when creating meaningful comparisons.
- The application does not automatically align panoramas captured from different locations.
- Browser local storage is not a substitute for a full project database or cloud backup.
- Very large panorama images may require significant browser memory.
- The standalone application is intended primarily for local presentation and lightweight project management.

## Future Development

Potential future improvements include:

- Exporting the Compare workspace as a standalone presentation.
- Saving and loading complete project files.
- Automatic panorama alignment.
- Improved floor-plan editing tools.
- Automatic camera-direction detection.
- VR headset support.
- Web-based project sharing.
- Cloud storage and collaboration.
- AI-assisted panorama editing.
- AI-generated interior design alternatives.
- Integration with architectural and interior-design workflows.

## License

Add your preferred license here, such as MIT, Apache-2.0, or a custom license.

---

**Panorama Tour Builder**  
A lightweight standalone tool for turning 360° images into interactive spatial experiences.

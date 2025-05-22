# Simple Backbone.js Note-Taking App

## Description

This is a simple client-side CRUD (Create, Read, Update, Delete) application for managing notes. It is built using Backbone.js, jQuery, and Underscore.js, with Bootstrap for styling.

This application serves as a demonstration of Backbone.js concepts. It operates entirely client-side and does not communicate with a server; all note data is managed within the browser session and will be lost upon closing or reloading the page.

## How to Run

1.  Clone this repository to your local machine (or download the files).
2.  Navigate to the project directory.
3.  Open the `index.html` file in your web browser.

No build steps or server setup is required as this is a purely client-side application.

## Features

*   **CRUD Operations:** Create, Read, Update, and Delete notes.
*   **Client-Side Data:** All note data is managed in the browser using Backbone.js Models and Collections. No data is sent to or stored on a server.
*   **Input Validation:** Basic validation is implemented for note fields (title, author, description).
*   **Debug Output:** A section on the page displays the current state of the notes collection in JSON format for debugging purposes.

## Project Structure

```
.
├── css/
│   └── bootstrap.min.css      # Bootstrap styling
├── img/
│   ├── glyphicons-halflings-white.png # Bootstrap icons
│   └── glyphicons-halflings.png   # Bootstrap icons
├── js/
│   ├── libs/                  # Third-party JavaScript libraries
│   │   ├── backbone.min.js
│   │   ├── jquery.min.js
│   │   └── underscore.min.js
│   ├── models/
│   │   └── note_model.js      # Backbone model for notes
│   ├── views/                 # Backbone views
│   │   ├── note_edit.js
│   │   ├── note_index.js
│   │   ├── note_new.js
│   │   ├── note_row.js
│   │   └── note_show.js
│   └── note_router.js         # Backbone router for handling application routes
├── index.html                 # Main HTML file, application entry point, and templates
└── README.md                  # This file
```

*   `index.html`: The main application page. It includes the necessary HTML structure, Underscore.js templates for different views, and initializes the Backbone application with some sample data.
*   `css/`: Contains stylesheets, primarily Bootstrap CSS for UI components.
*   `img/`: Contains image assets, such as icons used by Bootstrap.
*   `js/libs/`: Holds the core JavaScript libraries: jQuery, Underscore.js, and Backbone.js.
*   `js/models/`: Contains Backbone.js models. `note_model.js` defines the structure and validation for a single note.
*   `js/views/`: Contains Backbone.js views, responsible for rendering the UI components and handling user interactions for different parts of the application (e.g., displaying a list of notes, editing a note).
*   `js/note_router.js`: Defines the application's routes using Backbone.Router, mapping URLs to specific actions (e.g., showing the note index, opening the edit view for a note).

## Technology Stack

*   **[Backbone.js](https://backbonejs.org/):** Provides the Model-View-Router (MVR) framework for structuring the application.
*   **[Underscore.js](https://underscorejs.org/):** A utility library providing helpful functions, used extensively by Backbone.js and for templating.
*   **[jQuery](https://jquery.com/):** Used for DOM manipulation and event handling.
*   **[Bootstrap](https://getbootstrap.com/2.3.2/):** (Version 2.3.2 as indicated by `index.html` and file structure) Used for UI styling and components.

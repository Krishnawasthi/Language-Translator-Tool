# Language converter extension

Language Translator is a Google Chrome extension designed to facilitate easy text translation between multiple languages. With features such as text-to-speech, copy functionality, and easy language swapping, this tool aims to enhance your language learning and translation experience.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [API Information](#api-information)


## Features

- **Easy Text Translation:** Translate text between various languages with ease.
- **Copy Functionality:** Quickly copy the translated text to your clipboard.
- **Text-to-Speech:** Listen to the pronunciation of the text in both the source and target languages.
- **Language Swapping:** Swap between source and target languages with a single click for convenience.

## Technologies Used

- **HTML5:** For structuring the extension's popup interface.
- **CSS3:** For styling the extension to ensure a modern and clean look.
- **JavaScript:** For creating a dynamic and interactive user interface.
- **Google Chrome Extensions API:** For integrating the translation functionality within the Chrome browser.
- **Font Awesome:** For providing iconography.
- **MyMemory Translated API:** For providing translation services.

## Project Structure

The project is organized as follows:

- **manifest.json:** Configuration file for the Chrome extension.
- **index.html:** Main HTML file for the extension popup.
- **App.js:** Main JavaScript file for the extension functionality.
- **App.css:** Styles for the extension.
- **pop.js:** JavaScript functionality for the extension.
- **countries.js:** List of countries and their codes.

  # 📖 Word Popup Chrome Extension

A lightweight **Google Chrome Extension** designed to provide a convenient popup-based interface for working with words and language-related functionality.

This extension is part of the **Language Translator Tool** project and uses Chrome's **Manifest V3** architecture.

## ✨ Features

* 🧩 **Chrome Extension** — Runs directly inside Google Chrome.
* 💬 **Popup Interface** — Provides functionality through the browser extension popup.
* 🌐 **Language Support** — Uses a country/language mapping for language-related functionality.
* 🖼️ **Custom Extension Icons** — Includes multiple icon sizes for Chrome.
* 💾 **Chrome Storage Support** — Configured to use Chrome's storage API.
* ⚡ **Lightweight** — Built using HTML, CSS, and JavaScript.

## 🛠️ Technologies Used

| Technology                | Purpose                                  |
| ------------------------- | ---------------------------------------- |
| **HTML5**                 | Creates the popup interface              |
| **CSS3**                  | Styles the popup                         |
| **JavaScript**            | Handles popup functionality              |
| **Chrome Extensions API** | Provides browser extension functionality |
| **Manifest V3**           | Defines the extension configuration      |
| **Chrome Storage API**    | Provides storage functionality           |
| **PNG**                   | Extension icon assets                    |

## 📁 Project Structure

```text
word-popup-extension/
│
├── countries.js
├── llogo.png
├── manifest.json
├── mlogo.png
├── nlogo.png
├── pop.css
├── pop.html
└── pop.js
```

### File Description

#### `manifest.json`

The main configuration file of the Chrome extension.

It defines:

* Extension name
* Version
* Description
* Permissions
* Popup page
* Extension icons
* Manifest version

The project uses:

```json
"manifest_version": 3
```

which is the modern Chrome Extension Manifest format.

#### `pop.html`

Contains the structure of the extension's popup interface.

It acts as the main HTML page displayed when the extension icon is clicked.

#### `pop.css`

Contains the styling and layout of the popup interface.

It controls the visual appearance of the extension.

#### `pop.js`

Contains the JavaScript functionality of the popup.

It is responsible for handling user interactions and connecting the popup interface with the extension's functionality.

#### `countries.js`

Contains the language/country information used by the extension.

This data can be used to populate language selections and work with language codes.

#### `nlogo.png`

Small extension icon used by Chrome.

#### `mlogo.png`

Medium-sized extension icon.

#### `llogo.png`

Large extension icon.

## ⚙️ Manifest Configuration

The extension uses **Chrome Manifest V3**.

A simplified configuration looks like:

```json
{
    "manifest_version": 3,
    "name": "Word Popup Extension",
    "version": "1.0",
    "permissions": [
        "activeTab",
        "storage"
    ],
    "action": {
        "default_popup": "pop.html"
    }
}
```

## 🔐 Permissions

The extension currently uses two Chrome permissions.

### `activeTab`

Allows the extension to access the currently active tab when the extension is invoked.

This permission is useful when an extension needs to work with the content or context of the active webpage.

### `storage`

Provides access to Chrome's storage functionality.

It can be used to save extension-related data such as:

* User preferences
* Settings
* Language selections
* User-specific extension data

## 🔄 How the Extension Works

The basic flow is:

```text
User Opens Chrome
        ↓
Clicks Extension Icon
        ↓
Chrome Loads pop.html
        ↓
CSS Styles the Popup
        ↓
JavaScript Initializes Functionality
        ↓
User Interacts With Extension
        ↓
Extension Performs Requested Action
```

## 🚀 Installation

The extension can be installed locally using Chrome's **Load unpacked** feature.

### 1. Clone the Repository

```bash
git clone https://github.com/Krishnawasthi/Language-Translator-Tool.git
```

### 2. Open Chrome Extensions

Navigate to:

```text
chrome://extensions/
```

### 3. Enable Developer Mode

Enable **Developer mode** from the top-right corner.

### 4. Load the Extension

Click:

```text
Load unpacked
```

Navigate to:

```text
Language-Converter-Extension-main/
└── word-popup-extension/
```

Select the `word-popup-extension` folder.

### 5. Use the Extension

After installation, the extension will appear in your Chrome extensions list.

Pin it to the toolbar for convenient access.

## ▶️ Usage

1. Open Google Chrome.
2. Click the **Word Popup Extension** icon.
3. The popup interface will open.
4. Interact with the available functionality.
5. The extension uses its JavaScript logic to process user actions.

## 🧠 Architecture

The extension follows a simple three-layer frontend structure:

```text
             Chrome Extension
                    │
                    ▼
              ┌──────────┐
              │ pop.html │
              └────┬─────┘
                   │
          ┌────────┴────────┐
          ▼                 ▼
     ┌─────────┐       ┌─────────┐
     │ pop.css │       │  pop.js  │
     └─────────┘       └────┬────┘
                             │
                             ▼
                       Extension APIs
```

### HTML

Responsible for the popup structure.

### CSS

Responsible for the popup's visual design.

### JavaScript

Responsible for behavior, interactions, and application logic.

### Chrome APIs

Provide browser-level functionality such as active-tab access and storage.

## 📌 Why Manifest V3?

Manifest V3 is the modern extension platform used by Chrome.

Using Manifest V3 provides a more modern architecture for developing Chrome extensions and aligns the project with current Chrome extension development practices.

## 🎯 Use Cases

The extension can be useful for:

* 📚 Language learners
* 👨‍🎓 Students
* 🌍 Users working with multiple languages
* 📖 Reading and understanding online content
* 💻 Developers experimenting with Chrome Extensions
* 🧪 Learning browser extension development

## 💡 Learning Outcomes

This project demonstrates several practical web-development concepts:

* Chrome Extension development
* Manifest V3
* HTML/CSS/JavaScript integration
* Browser permissions
* Popup-based extension architecture
* Chrome Storage API
* Working with language/country data
* Browser extension icons and configuration

## 🔮 Future Improvements

Possible improvements include:

* 🔍 Automatic word detection
* 📖 Dictionary definitions
* 🔊 Word pronunciation
* 🌐 Direct translation of selected words
* ⭐ Save favorite words
* 🕘 Word/translation history
* 📚 Example sentences
* 🌙 Dark mode
* ⌨️ Keyboard shortcuts
* 💾 Persistent user preferences

## ⚠️ Notes

* The extension requires Google Chrome or a Chromium-based browser that supports Manifest V3.
* Some functionality depends on the permissions granted through `manifest.json`.
* The available features are determined by the implementation in `pop.js`.

## 👨‍💻 Author

**Krishna Mohan Awasthi**

GitHub: [Krishnawasthi](https://github.com/Krishnawasthi)

## 📄 License

This project is created for **learning and development purposes**.

If you plan to distribute or modify the project publicly, consider adding an appropriate open-source license.


## API Information

https://api.mymemory.translated.net/get?q={text}&langpair={translateFrom}|{translateTo}




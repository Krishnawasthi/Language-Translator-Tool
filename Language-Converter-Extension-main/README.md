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

## API Information

https://api.mymemory.translated.net/get?q={text}&langpair={translateFrom}|{translateTo}




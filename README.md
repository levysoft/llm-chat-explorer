# LLM Chat Explorer
A privacy-focused web application for locally processing and analyzing ChatGPT and Claude chat exports. The search functions provided by official platforms are often slow and impractical for users with many conversations. This application allows for more efficient management of AI chat history, ensuring quick and organized access to saved conversations.

![GitHub release (latest by date)](https://img.shields.io/github/v/release/levysoft/llm-chat-explorer?label=latest) [![Github All Releases](https://img.shields.io/github/downloads/levysoft/llm-chat-explorer/total.svg)](https://github.com/levysoft/llm-chat-explorer/releases) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-yellow.svg)](https://opensource.org/licenses/GPLv3) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/levysoft/llm-chat-explorer/graphs/commit-activity) [![GitHub contributors](https://img.shields.io/github/contributors/levysoft/llm-chat-explorer.svg)](https://github.com/levysoft/llm-chat-explorer/graphs/contributors) [![made-with-html](https://img.shields.io/badge/Made%20with-HTML-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/HTML) [![made-with-css](https://img.shields.io/badge/Made%20with-CSS-blue.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS) [![made-with-javascript](https://img.shields.io/badge/Made%20with-JavaScript-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

[ [English](README.md) | [Italiano](README.it.md) ]

This repository provides a web application for viewing and analyzing chat exports from ChatGPT and Claude, with a strong focus on privacy. All data is processed locally in the browser, ensuring that personal information is not sent to external servers. If desired, you can download the HTML page to inspect the source code and verify the application’s functionality firsthand. The entire project was developed to be completely standalone, using only HTML, CSS, and JavaScript, with no external dependencies (except for fonts). This allows users to download and use the page locally without any additional configuration.

Although ChatGPT and Claude offer internal search functions, these can be slow and cumbersome, especially for users with a large number of saved conversations. By downloading the chat backup and using this application, users can manage their AI interactions more quickly and conveniently. This approach ensures structured and fast access to past conversations, improving efficiency in retrieving information and revisiting previous discussions. Additionally, working locally bypasses platform-imposed limitations, such as losing old chats or difficulties in exporting entire archives.

## Exporting Chats from ChatGPT and Claude

To use this application, you first need to export conversations from ChatGPT or Claude. The official procedures are available at the following links:

- **ChatGPT**: [How to export ChatGPT history](https://help.openai.com/en/articles/7260999-how-do-i-export-my-chatgpt-history-and-data)
- **Claude**: [How to export Claude chat history](https://support.anthropic.com/en/articles/9450526-how-can-i-export-my-claude-ai-data)

## Contents

1. [Introduction](#introduction)
2. [Privacy and Security](#privacy-and-security)
3. [Requirements](#requirements)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Application Description](#application-description)
7. [File Structure](#file-structure)
8. [Screenshots](#screenshots)
9. [Feedback and Contributions](#feedback-and-contributions)
10. [Changelog](#changelog)
11. [Author](#author)
12. [License](#license)

## Introduction

**LLM Chat Explorer** is a web application that allows users to upload and analyze JSON files containing exported conversations from ChatGPT and Claude. Its intuitive interface makes it easy to search and view chats, providing a lightweight and fast solution without compromising data privacy.

One of the main advantages of this application is the ability to easily analyze AI conversations without having to decipher raw JSON files. While ChatGPT provides both a JSON file and a preformatted HTML file with all chats integrated, Claude, on the other hand, only offers a JSON file, making it particularly difficult to navigate, especially when dealing with large files. **LLM Chat Explorer** solves this problem by allowing users to seamlessly view and navigate their conversations through an intuitive and accessible interface.

## Privacy and Security

The application is designed with a strong focus on privacy:
- **Local Processing**: All data is processed directly in the browser, with no external server communication.
- **No Tracking**: Personal data and chat history remain entirely on the user’s device.
- **Source Code Inspection**: If desired, you can download the HTML page and analyze the source code.
- **Standalone**: The entire application is built with simple HTML, CSS, and JavaScript, with no external dependencies (except for Font Awesome), specifically to allow users to download and use the HTML page locally without any additional setup.
- **Open Source**: The project is released under the GPL v3 license, ensuring transparency and allowing the community to verify and improve the code.

## Requirements

- A modern web browser (Chrome, Firefox, Edge, Safari)
- Internet connection required only to load the external Font Awesome CSS file (optional, for full offline use, download the corresponding CSS file).

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/levysoft/llm-chat-explorer.git
    ```
2. Open the `llm-chat-explorer.html` file in your preferred web browser.
3. *(Optional)* For full offline usage, simply download the Font Awesome CSS file to remove any external asset dependencies.

## Usage

1. Launch the application by opening the `llm-chat-explorer.html` file in your browser.
2. Drag and drop the JSON file (e.g., `conversations.json`) into the upload area or click to select it.
3. Browse the list of chats and select one to analyze.
4. Use the search bar to filter conversations by title or content.
5. Customize the interface by changing the language, dark mode settings, and scroll position through the settings menu.

## Application Description

The application is built with HTML, CSS, and JavaScript and offers the following features:
- **Local JSON File Processing**: Data is read and processed using the `FileReader` object without being sent online.
- **Advanced Chat Management**: Supports ChatGPT and Claude’s export formats, normalizing the chat order and enabling advanced searches within titles and content.
- **Dynamic and Responsive Interface**: A sidebar for navigating chats and a display area for messages, with search and customization support.
- **Multilanguage and Dark/Light Mode**: The interface supports multiple languages (English, Italian, Spanish, French, German, Polish, Chinese, Korean, and Japanese) and allows enabling or disabling dark mode.
- **Chat Position**: This setting controls the order of messages within individual chats. By selecting "At end," the most recent message will appear at the bottom, similar to common messaging apps. Choosing "At start" will display the latest messages at the top.
- **Direct Chat Viewing**: Each individual chat in the backup can be accessed directly within the user's ChatGPT or Claude account by clicking the associated share link.

## File Structure
```
llm-chat-explorer/
├── llm-chat-explorer.html      # Main application page
├── assets/                     # Folder containing images and screenshots
│   ├── screenshot1.jpg
│   ├── screenshot2.jpg
│   ├── screenshot3.jpg
│   └── screenshot4.jpg
├── README.md                   # This file
└── LICENSE                     # License file (GPL v3)
```

## Screenshots

Here are some screenshots of the application:

- **Upload Page**:

  ![Upload Page](assets/screenshot1.jpg)

- **Chat List**:

  ![Chat List](assets/screenshot2.jpg)

- **Settings**:

  ![Settings](assets/screenshot3.jpg)

- **Advanced Search**:

  ![Advanced Search](assets/screenshot4.jpg)
  
## Feedback and Contributions

Your feedback is valuable! If you encounter issues or have suggestions, please open an [issue](https://github.com/levysoft/llm-chat-explorer/issues) or submit a pull request. Contributions and suggestions for improvements are always welcome.

## Changelog

All changes and updates to the application are documented in the [CHANGELOG.md](./CHANGELOG.md) file.

## Author

Antonio Troise

## License

This project is released under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.en.html) license. See the LICENSE file for more details.


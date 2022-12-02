---
layout: software-project
title: Yet Another Language Learning Extension
description: "🗃️ An extension create flashcards in the browser"
published: True
---

<img src="/assets/software-project/yet-another-language-learning-extension/github_logo.png" alt="Yet Another Language Learning Extension Logo" width="20%" style="display: block; margin: 0 auto"/>

## Yet Another Language Learning Extension ([repository](https://github.com/johanneshagspiel/yet-another-language-learning-extension))

| Summary  |
| -------------------------------------------------- |
| 🗃️ A Google Chrome extension to translate words and create flashcards in the browser. The purpose of this application is to help save time with the time-consuming and boring parts of learning a new language such as looking up a word in a dictionary, checking whether it already is in ones vocabulary list and then creating a flash card for it. "Yet Another Language Learning Extension" (YALLE) combines all these activities in one simple Google Chrome extension that automates parts of it like checking for duplicates. |

## Features  

"Yet Another Language Learning Extension" currently:
- supports the [PONS](https://en.pons.com/) dictionary
  - the user can look up words in all supported languages
  - the results are visually represented similarly to the original website
- is integrated with the [Anki](https://apps.ankiweb.net/) flashcard program
  - the user can select which deck and model to store a flashcard in
  - YALLE automatically checks whether a note for a word already exists
- uses a [Tiptap](https://tiptap.dev/) based text editor
  - the user can format the content on the flash card in common ways such as i.e. bold text or create a list

## To-Do

YALLE is very much still under development and not bug-free and without any styling. However, its baseline functionality as outlined above already works. The main points of future improvement are: 

- Optimize the React components to minimize re-renders
- Sanity check user input
- Style the entire application with CSS 
- Support more storage options such as Google docs
- Support more dictionaries with an API such as the one provided by the Oxford Dictionary
- Comment the code base
- Add more formatting options to the editor such as justifying text

The ultimate goal is to extend YALLE's functionality further to the actual learning process by implementing features such as:
- replacing the new tab page with a screen where the user can review flash cards 
- help user learn by motivating them through activity trackers and progress bars 

## Tools

| Purpose                               | Name                                                                            |
|---------------------------------------|---------------------------------------------------------------------------------|
| Programming language                  | [Javascript](https://nodejs.org/en/)                                            |
| Package manager                       | [npm](https://www.npmjs.com/)                                                   |
| Version control system                | [Git](https://git-scm.com/)                                                     |  
| UI Framework                          | [React 17](https://reactjs.org)                                                 | 
| JavaScript bundler                    | [Webpack 5](https://webpack.js.org/)                                            |
| Development server for live reloading | [Webpack Dev Server 4](https://webpack.js.org/configuration/dev-server/)        | 
| Hot loader for React components       | [React Hot Loader](https://github.com/gaearon/react-hot-loader)                 |
| ESLint configuration for react app    | [eslint-config-react-app](https://www.npmjs.com/package/eslint-config-react-app) |
 | Code formatter                        | [Prettier](https://prettier.io/)                                                |
| WYSIWYG Text Editor |[Tiptap](https://tiptap.dev/)                                                    |

## Installation

To simply install the extension, you can find the most recent compiled build with the [latest release](https://github.com/johanneshagspiel/yet-another-language-learning-extension/releases/). Then, you should load the extension in Google Chrome by:
1. Going to `chrome://extensions/`
2. Checking the option `Developer mode`
3. Clicking on `Load unpacked extension`
4. Selecting the unzipped `yet-another-language-learning-extension` folder from the release

To build the application yourself, you have to:

1. Check if your Node.js version is >= 14 with `node -v`
2. Clone this repository with `git clone https://github.com/johanneshagspiel/yet-another-language-learning-extension.git`
3. Run `npm install` to install all the dependencies
4. Run `npm start` to launch the webpack server
5. Load the extension in Google Chrome by:
   1. Going to `chrome://extensions/`
   2. Checking the option `Developer mode`
   3. Clicking on `Load unpacked extension`
   4. Selecting the generated `build` folder

## Licence

The "Yet Another Language Learning Extension" is published under the MIT licence, which can be found in the [LICENSE](https://github.com/johanneshagspiel/yet-another-language-learning-extension/blob/main/LICENSE) file. 

## References

- This program is based on a boilerplate template created by [Michael Xieyang Liu](https://github.com/lxieyang/chrome-extension-boilerplate-react).
- The flashcard symbol used in the logo was created by [iconixar](https://www.flaticon.com/de/autoren/iconixar) on [flaticon](https://www.flaticon.com/free-icons/flashcard).
- The editor symbols were taken from [Remix Icon](https://remixicon.com/).
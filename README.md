# Spell Check and Auto-Correction

This project is a simple React application that implements a basic spell check and auto-correction feature using a custom dictionary. As you type, the app suggests corrections for common spelling mistakes in real time.

## Features

- **Custom Dictionary:** Predefined corrections for common spelling mistakes.
- **Real-time Spell Check:** As the user types, the application checks each word and suggests corrections if a match is found in the dictionary.
- **Interactive User Interface:** Displays suggested corrections dynamically based on user input.

## Demo

You can see the live demo of the project deployed on Vercel:
[Spell Check and Auto-Correction Demo](https://xspellcheck-rose-five.vercel.app/)

## Getting Started

### Prerequisites

Before you begin, ensure you have the following tools installed on your machine:

- **Node.js** (version 14 or higher)
- **npm** (Node package manager)

### `Installation`

Follow these steps to set up and run the project locally:

1. Clone the repository:

```bash
git clone https://github.com/surendergupta/xspellcheck.git

```

2. Navigate into the project directory:

```bash
cd xspellcheck

```

3. Install dependencies:

```bash
npm install

```

4. Start the development server:

```bash
npm start

```

The application will run on http://localhost:3000.

### Usage

1. Once the app is running, you'll see a text area where you can enter text.
2. As you type, the app will suggest corrections for any words that match predefined entries in the custom dictionary.
3. If a correction is available, it will be displayed as a suggestion below the text area.

### Example

For example, typing the following text:

```bash

I will wrok on teh project fot exampl.

```

Will suggest corrections:

```bash

Did you mean: work? (for wrok)
Did you mean: the? (for teh)
Did you mean: for? (for fot)
Did you mean: example? (for exampl)


```

## Code Structure

The project consists of a functional component, App, implemented using React's useState hook to manage state for the input text and the suggested correction.

## Key Components:

- **App Component:** The core logic of the app, responsible for capturing user input, checking for spelling mistakes, and displaying suggestions.
- **State Management:**
    - **inputText:** Tracks the user's typed input.
    - **suggestedText:** Holds the current suggested correction, if any.
- **Custom Dictionary:** A predefined object mapping common misspellings to their correct form.

## How It Works

1. The ```handleInputChange``` function listens for input changes in the textarea.
2. It splits the input text into words and checks each word against the custom dictionary.
3. If a correction is found, the first misspelled word is displayed as a suggestion.


## Custom Dictionary

The application currently uses the following custom dictionary:

```javascript

const customDictionary = {
  teh: "the",
  wrok: "work",
  fot: "for",
  exampl: "example",
};


```

Feel free to expand the dictionary by adding more words and their corrections.

## Future Improvements

- **Dynamic Dictionary:** Allow users to add custom corrections to the dictionary dynamically.
- **Multiple Suggestions:** Show corrections for all misspelled words in the input text, not just the first one.
- **Enhance UI/UX:** Add a button to apply the suggested corrections directly to the input text.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. Contributions, bug reports, and feature requests are welcome!

1. Fork the project
2. Create your feature branch: ```git checkout -b feature/my-new-feature```
3. Commit your changes: ```git commit -am 'Add some feature'```
4. Push to the branch: ```git push origin feature/my-new-feature```
5. Create a new pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## **Author**

Made with ❤️ by [Surender Gupta](mailto:gupta.surender.1990@gmail.com)

Feel free to reach out via email for any questions or suggestions!
# Language Translation Tool

A web-based language translation tool built with HTML, CSS and JavaScript. Users can enter text, choose the source and target languages, and get the translated text instantly on the screen.

## Features

- Simple user interface with a text box and source and target language dropdowns
- Supports 12 languages, including English, Hindi, Telugu, Tamil, Kannada, Malayalam, French, German, Spanish, Arabic, Japanese and Korean
- Sends the text to a translation API and displays the translated response clearly
- Copy button to copy the translated text
- Text-to-speech (Listen button) to hear the translation
- Swap button to switch the source and target languages
- Clear button to reset the input and output
- Error messages for empty text, identical languages, and connection problems

## Technologies Used

- HTML5
- CSS3
- JavaScript (Fetch API, Clipboard API, Web Speech API)

## APIs Used

- Google Cloud Translation API (used when an API key is added in the code)
- MyMemory Translation API (free, used when no key is set)
- Google Translate web endpoint (used as a backup if the other APIs fail)

## How It Works

1. The user types text and selects the source and target languages.
2. On clicking **Translate**, the text is sent to the translation API using `fetch()`.
3. The API returns the translated text in JSON format.
4. The translated text is displayed in the output box.
5. The user can copy the result or listen to it using text-to-speech.

## How to Run

1. Download or clone this repository.
2. Open `translator.html` in a web browser such as Chrome.
3. Enter text, choose the languages, and click **Translate**.

An internet connection is required to use the translation APIs.

## Optional: Using the Google Translate API

Open `translator.html` and paste your Google Cloud Translation API key into this line:

const GOOGLE_API_KEY = "";

If the key is left empty, the app uses the free MyMemory API.

## Author

Susmitha

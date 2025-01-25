# Smart Reply Assistant

This is a web application that uses AI to generate professional email replies. The app allows users to input an email content and choose the tone of the reply (e.g., formal, friendly), and the backend generates a response based on the Gemini API.

## Features
- **Email Reply Generation**: Input your email content and select a tone to generate a professional email reply.
- **Gemini API Integration**: Communicates with the Gemini API to fetch reply suggestions.
- **Chrome Extension**: Easily generate email replies directly from your browser.

## Tech Stack
- **Backend**: Spring Boot
  - `WebClient`: Used to interact with the Gemini API.
  - `ObjectMapper` and `JsonNode`: For parsing and extracting data from the Gemini API response.
- **Frontend**: React
- **Chrome Extension**: For generating email replies directly from your browser.

### Chrome Extension
1. Go to `chrome://extensions/` in your Chrome browser.
2. Enable **Developer Mode**.
3. Click **Load unpacked** and select the `smart-reply-ext` directory.
4. The extension will now be available in your Chrome toolbar.

## Usage
1. In the frontend, enter the email content and select the tone (formal, friendly, etc.).
2. The app will send a request to the backend to generate a reply based on the tone and email content.
3. View the generated reply in the UI.
4. Use the Chrome extension to generate replies directly from your browser.

## Configuration
The backend requires the following properties to be set:
- `gemini.api.url`: The URL of the Gemini API.
- `gemini.api.key`: Your Gemini API key.

You can add these in the `application.properties` file.



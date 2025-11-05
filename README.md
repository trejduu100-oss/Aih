# AI Voice Generator

A text-to-speech application that uses Google's Gemini API to generate high-quality, natural-sounding AI voices. Enter text, choose a voice, adjust speed and pitch, and then listen to or download the generated audio.

This project is built with React, TypeScript, and Tailwind CSS.

## Features

- **Text-to-Speech:** Convert any text into spoken audio.
- **Multiple Voices:** Choose from a diverse list of high-quality AI voices.
- **Audio Controls:** Adjust the playback speed and pitch (low, medium, high).
- **Playback & Download:** Listen to the generated speech directly in the app and download it as a `.wav` file.
- **Responsive UI:** A clean and modern interface that works on all screen sizes.
- **Loading & Error States:** Clear feedback during API calls and for any potential errors.

## How to Run Locally

This project is set up to run in an environment that supports modern JavaScript features, including ES modules and direct rendering of TSX/JSX files, such as Google's AI Studio or a pre-configured local development server.

To run this project on your own machine, you will need a build tool and development server like [Vite](https://vitejs.dev/) or [Create React App](https://create-react-app.dev/).

### General Steps for Local Setup:

1.  **Prerequisites:**
    *   Node.js and a package manager (npm, yarn, etc.).
    *   A Google Gemini API Key. You can get one from [Google AI Studio](https://aistudio.google.com/app/apikey).

2.  **Set Up Your Environment:**
    *   Download the project files.
    *   In the project directory, you would typically set up a `package.json` file to manage dependencies like `react`, `react-dom`, and `@google/genai`.
    *   Set up a local development server (e.g., Vite).

3.  **Configure API Key:**
    *   The application expects the Gemini API key to be available as an environment variable named `API_KEY`.
    *   When using a tool like Vite, you can create a `.env` file in the root of your project and add your key. Your local server must be configured to expose this variable to the client-side code under `process.env.API_KEY`.

4.  **Run the Server:**
    *   Start your development server (e.g., `npm run dev`).
    *   Open the provided URL in your browser.

## How to Use the Application

1.  **Enter Text:** Type or paste the text you want to convert to speech into the text area.
2.  **Choose a Voice:** Select one of the available voice options.
3.  **Adjust Settings (Optional):** Use the sliders and buttons to change the speed and pitch of the voice.
4.  **Generate:** Click the "Generate Speech" button. The app will contact the Gemini API and create the audio.
5.  **Play/Download:** Once generation is complete, use the play button to listen to the audio or the download button to save it as a WAV file.

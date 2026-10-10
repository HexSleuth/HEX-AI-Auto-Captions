Here is a comprehensive README.md for the HEX-AI-Auto-Captions repository, based on the features and technical details of the web application.
# HEX Captions Online

An entirely browser-based, privacy-first tool for generating real-time live captions and AI-powered subtitles from audio/video files. Built with Hugging Face Transformers.js and OpenAI Whisper, HEX Captions processes everything locally on your device—meaning no servers, no API keys, and no uploads.

## 🚀 Features

* **AI Caption Generator**: Drop in a media file and generate timestamped subtitles without uploading your confidential files to the cloud.
* **Real-time Live Captions**: Instant speech-to-text directly from your microphone using the browser's native Web Speech API. 
* **100% On-Device Processing**: Powered by WebAssembly and Web Audio. Your media is never uploaded, logged, or stored.
* **Instant Subtitle Styling**: Customize font families, text effects, background colors, spacing, and positions. Changes apply instantly and embed directly into your exported VTT files.
* **Export Options**: Preview, copy, or download your transcripts as ready-to-use **SRT** or **WebVTT** files.
* **Customizable UI**: Choose from 33 built-in themes with custom color overrides (dark mode enabled by default).

## 🛠️ Technology Stack

* **[Hugging Face Transformers.js](https://github.com/huggingface/transformers.js)**: Runs state-of-the-art machine learning models directly in the browser.
* **[OpenAI Whisper](https://github.com/openai/whisper)**: The industry-standard open-source speech recognition model.
* **Web Speech API**: For low-latency live microphone transcription.
* **WebAssembly (WASM)**: Enables high-performance local execution of Python-based ML models in standard web browsers.

## 🧠 Supported AI Models

The tool downloads your selected model on the first use and caches it in your browser for fast, offline-capable repeat usage.

| Model | Size | Best For |
| :--- | :--- | :--- |
| **Whisper Tiny** | ~45 MB | Fastest processing; works smoothly on almost any device. |
| **Whisper Base** | ~80 MB | A great balance between transcription speed and word accuracy. |
| **Whisper Small** | ~250 MB | Highest accuracy; recommended for devices with higher RAM. |

## 📁 Supported Media Formats

The AI Generator can decode audio tracks directly from the following file types:
* **Audio**: MP3, WAV, M4A
* **Video**: MP4, WebM, MOV

## 💻 Usage

Since the application is a static, browser-based web app, there is zero setup or installation required. 

1. **Visit the App**: Go to the live [HEX Captions Online environment](https://hexsleuth.github.io/HEX-AI-Auto-Captions/).
2. **Choose your Mode**:
   * **Live Captions**: Grant microphone permissions and tap "Start" to dictate.
   * **AI Generator**: Drag and drop your media file, select your preferred Whisper model, and wait for the local processing to complete.
3. **Customize**: Head to the "Subtitle Style" tab to visually tweak your captions.
4. **Export**: Go to the "Transcript" section to view your timestamped cues and export them as `.srt` or `.vtt`.

*Note: Processing time depends on the media duration, selected model, available CPU/RAM, and your specific browser. Google Chrome, Microsoft Edge, and Safari are recommended for full Web Speech API and WASM support.*

## 🔒 Privacy Guarantee

Because all processing happens on the edge via WebAssembly, this tool is completely safe for unpublished videos, internal meetings, and confidential recordings. **No tracking, no servers, no cloud storage.**


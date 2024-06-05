# AI Video Generator

The **AI Video Generator** automates the creation of videos from web pages by processing their content into a video format using natural language processing (NLP), computer vision, and audio synthesis.

## Features
- **URL Parsing:** Opens the provided URL and extracts the webpage content.
- **Content Summarization:** Uses AI to generate a summary of the extracted text.
- **Text-to-Speech (TTS):** Converts the summarized text into a natural voiceover.
- **Image Generation:** Creates B-roll images related to the text using AI image generators.
- **Subtitles & Text Overlay:** Transcribes the summarized text for subtitles and on-screen text.
- **Video Assembly:** Combines all elements (voiceover, images, subtitles) into a complete video using the FFmpeg library.

## How It Works
1. **Input URL**: The user provides a webpage URL.
2. **Text Extraction**: The system extracts and summarizes the textual content of the page.
3. **Voiceover Generation**: The summarized text is converted to speech using TTS.
4. **B-roll Creation**: AI-generated images provide relevant visuals for the video.
5. **Subtitles Creation**: Transcription of the summarized content is used for subtitles or text overlays.
6. **Video Rendering**: FFmpeg is used to combine voiceover, images, and subtitles into a finished video.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/ai-video-generator.git
    cd ai-video-generator
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Install FFmpeg:
    Follow [FFmpeg installation instructions](https://ffmpeg.org/download.html) for your OS.

## Usage

1. Run the script with a URL:
    ```bash
    python main.py --url https://example.com
    ```

2. The system will process the URL and output a video in the `output/` folder.

## Requirements
- Python 3.8+
- FFmpeg
- TensorFlow/PyTorch (for AI models)
- OpenAI GPT for text summarization
- Google Cloud TTS or equivalent for voiceover
- DALL·E or Stable Diffusion for image generation
# Video to Reels

Video to Reels is a Streamlit-based application that allows users to upload a video, automatically generate short highlight reels, and download them. This project uses OpenAI's Whisper model for audio-to-text conversion, along with other tools for video processing and summarization. 

## Features
- **Video Upload**: Users can upload their video files.
- **Automatic Reel Generation**: The app automatically identifies and generates short, engaging highlight reels.
- **Custom Resolution**: Allows users to select their preferred resolution for the generated reel. 
- **Download**: Once the reel is generated, users can download the video.

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.7 or later
- [Streamlit](https://streamlit.io/)
- [Whisper](https://github.com/openai/whisper) by OpenAI
- OpenAI API Key for Whisper and GPT usage

### Installation

1. **Clone the Repository**
    ```bash
    git clone [repository URL]
    cd video-to-reels
    ```

2. **Set Up Environment Variables**
   - Create a `.env` file in the root directory and add the following environment variables:

      ```plaintext
      DB_HOST=your_database_host
      DB_DATABASE=your_database_name
      DB_USERNAME=your_database_username
      DB_PASSWORD=your_database_password
      DB_PORT=your_database_port
      EMAIL_USER=your_email_user
      EMAIL_PASSWORD=your_email_password
      ```

3. **Install Dependencies**
   - Use the following command to install required packages:
      ```bash
      pip install -r requirements.txt
      ```

4. **Install Whisper by OpenAI**
   - Follow [Whisper's installation instructions](https://github.com/openai/whisper) to set up the model.

5. **Run the Application**
   - Start the Streamlit app with:
      ```bash
      streamlit run app.py
      ```

## Configuration

The application uses various settings controlled by environment variables set in the `.env` file, including database credentials, email server settings, and API keys for OpenAI services.

## Technologies Used

- **Streamlit**: For building the web application.
- **OpenAI Whisper**: For audio transcription.
- **FFmpeg and MoviePy**: For video processing.
- **OpenAI GPT**: For content analysis and summarization.

## Troubleshooting

- **Database Connection Issues**: Verify that database environment variables in `.env` are correct.
- **OpenAI API Errors**: Make sure that the `OPENAI_API_KEY` is valid and has necessary permissions.
- **Video Processing Errors**: Ensure that `ffmpeg` and `moviepy` are correctly installed.

## License

This project is licensed under the MIT License.
# License Plate Recognition System

The main functionality of the system is to identify license plates in provided images, extract the text using Optical Character Recognition (OCR), and then convert that extracted text into an audio output. This system is designed specifically for visually impaired individuals who need to know if a ride-sharing service vehicle (e.g., Uber, Lyft) has arrived. By taking a picture of the area around them, the system can detect the license plate of the arriving vehicle and audibly confirm its presence. Additionally, it can be useful in other scenarios such as automated parking systems or vehicle monitoring.

## Features

- Image Preprocessing: Resizes license plate images, applies Gaussian blur, and uses binary thresholding to enhance OCR accuracy.

- Text Extraction: Uses Tesseract OCR to extract text from the processed license plate images.

- Text Filtering: Filters the extracted text to include only valid characters (letters and digits) to remove unnecessary noise.

- Text-to-Speech Conversion: Converts the recognized text into an audio file that can be played back to the user using Google's gTTS API.

## Dependencies
- Python
- pytesseract
- OpenCV
- numpy
- matplotlib
- gtts

To install the necessary dependencies, use the following command:

    pip install opencv-python pytesseract gtts matplotlib

Additionally, you will need to install Tesseract-OCR. For Mac OS, you can use the following command:

    brew install tesseract

## Running the Application

1. Clone the repository: Clone the project repository to your local machine.

2. Install Required Libraries: Install the required libraries using the command below.

    pip install opencv-python pytesseract gtts matplotlib

3. Run the Application: Execute the application script to start recognizing license plates and converting them to audio.

    python main.py

4. Access the Output: The recognized license plate text will be converted to audio and played back to the user.

## Future Improvements
- Add More Platforms: Update the audio playback feature to support multiple operating systems.
  
- User Authentication: Add user login functionality to personalize the experience and track user interactions.
  
- Persistent Data Storage: Store user actions and detected license plates in a database for long-term tracking.

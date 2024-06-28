## FastAPI Audio Transcription Application
This application allows you to transcribe audio files using the Deepgram API and store transcripts in a PostgreSQL database.

## Prerequisites
Before running the application, ensure you have the following installed:

Python 3.x
pip (Python package installer)
PostgreSQL (with appropriate credentials and a database created)

## Installation
Clone the repository:

bash
Copy code
git clone <repository_url>
cd <repository_name>
Install dependencies:

bash
Copy code
pip install -r requirements.txt
## Configuration
Set up environment variables:

DATABASE_URL: PostgreSQL database connection string.
SECRET_KEY: Secret key for JWT token encryption.
DEEPGRAM_API_KEY: API key for Deepgram API.
Example:

bash
Copy code
export DATABASE_URL="postgresql://postgres:password@localhost/christal"
export SECRET_KEY="your-secret-key"
export DEEPGRAM_API_KEY="your-deepgram-api-key"
Alternatively, you can set these variables in a .env file and use python-dotenv to load them.
## Voice 


https://github.com/christalselvin/Audio-Transcription-Backend/assets/127867279/be0d6817-554c-49df-9846-b8c691bd1a1c



## Running the Application
Run the FastAPI application using Uvicorn:

bash
Copy code
uvicorn main:app --host 127.0.0.1 --port 8001 --reload
Replace main with the name of your Python file containing the FastAPI app object (main.py in your case).

Once the server is running, navigate to the Swagger documentation to explore and test the API:

Open your browser and go to http://127.0.0.1:8001/docs
## images
![Screenshot 2024-06-28 082223](https://github.com/christalselvin/Audio-Transcription-Backend/assets/127867279/96ea0b8b-ced7-4e58-9716-8a975993996c)
![Screenshot 2024-06-28 082325](https://github.com/christalselvin/Audio-Transcription-Backend/assets/127867279/e31bb676-2ba2-49db-b838-0418740b97ea)
![Screenshot 2024-06-28 082342](https://github.com/christalselvin/Audio-Transcription-Backend/assets/127867279/57883a8d-b9f2-4bb4-919b-0d786f595010)


## API Endpoints
POST /token: Obtain an access token for authentication.
POST /transcribe: Upload an audio file for transcription.
POST /save_transcript: Save a transcript to the database.
Notes
Ensure PostgreSQL is running and accessible with the provided credentials.
Replace placeholder values (<repository_url>, <repository_name>, password, etc.) with your actual values.

## Notes
Ensure PostgreSQL is running and accessible with the provided credentials.
Replace placeholder values (<repository_url>, <repository_name>, password, etc.) with your actual values.

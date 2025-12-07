# Fulldoodler
AutoDoodler Local Setup Guide

Follow these steps to run the AutoDoodler app on your local machine using Python 3.

1. Prerequisites

Ensure you have Python 3 installed. You can verify this by running:

python3 --version


2. Project Setup

Open your terminal or command prompt and navigate to the folder where you saved autododler.py.

Create a Virtual Environment

It is best practice to run this in a virtual environment to avoid conflicts.

On macOS / Linux:

python3 -m venv venv
source venv/bin/activate


On Windows (Command Prompt):

python -m venv venv
venv\Scripts\activate


On Windows (PowerShell):

python -m venv venv
.\venv\Scripts\Activate.ps1


(You will know it worked if you see (venv) at the start of your terminal line)

3. Install Dependencies

Save the requirements.txt file provided below in the same folder, then run:

pip install -r requirements.txt


Note: If you run into issues with OpenCV, you may need to install opencv-python instead of opencv-python-headless depending on your OS, but headless is generally recommended for server-based apps like Streamlit.

4. Run the Application

Once the installation finishes, launch the app:

streamlit run autododler.py


This will automatically open your default web browser to http://localhost:8501.

5. Troubleshooting

MoviePy/FFmpeg errors: If MoviePy complains about missing FFmpeg, usually it installs its own binary, but if it fails, you can try: pip install imageio-ffmpeg.

OpenCV errors: If headless fails, try: pip uninstall opencv-python-headless followed by pip install opencv-python.

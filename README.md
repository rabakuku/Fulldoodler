🎨 AutoDoodlerAutoDoodler is a Python-based whiteboard animation generator that uses OpenCV and MoviePy to create "hand-drawn" video effects from images and text. This application runs locally in your browser using Streamlit.🚀 Quick Start GuideFollow these instructions to set up and run the project on your local machine.1. PrerequisitesPython 3.8+: Ensure you have Python installed.python3 --version
2. InstallationNavigate to the project folder in your terminal/command prompt.Create and Activate a Virtual Environment (Recommended):macOS / Linux:python3 -m venv venv
source venv/bin/activate
Windows (Command Prompt):python -m venv venv
venv\Scripts\activate
Windows (PowerShell):python -m venv venv
.\venv\Scripts\Activate.ps1
Install Dependencies:You can install the required libraries directly using pip.Option A: Create a requirements.txt fileCreate a file named requirements.txt with the following content:streamlit
opencv-python-headless
moviepy
numpy
imageio-ffmpeg
Then run:pip install -r requirements.txt
Option B: Install directly via command linepip install streamlit opencv-python-headless moviepy numpy imageio-ffmpeg
Note: If you encounter errors with OpenCV, you may need to use the standard package instead of headless:pip install opencv-python3. UsageOnce installed, start the application by running:streamlit run autododler.py
This will automatically open your default web browser to:http://localhost:85014. TroubleshootingFFmpeg not found: If MoviePy fails to render, try installing FFmpeg manually or run:pip install imageio-ffmpeg
OpenCV Import Error: If cv2 cannot be imported, try reinstalling it:pip uninstall opencv-python-headless
pip install opencv-python

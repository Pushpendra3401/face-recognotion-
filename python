from flask import Flask, render_template
import subprocess

app = Flask(__name__)

@app.route('/')
def index():
    return render_template('index.html')

@app.route('/start')
def start():
    subprocess.Popen(["python", "face_recognition_script.py"])  # Rename your Python file accordingly
    return "Recognition started. Check your webcam window."

if __name__ == '__main__':
    app.run(debug=True)

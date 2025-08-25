AI Voice Cloning and Talking Avatar
📌 Project Overview

This project develops a complete pipeline that takes a single photo and a 30–60 second voice sample of a person, clones the voice using AI, and generates a talking avatar video where lip movements are synchronized with the cloned voice.

The solution is fully based on open-source tools and runs on Google Colab (free GPU).

🎯 Objective

Clone a person’s voice from a short reference audio.

Generate a talking avatar video from a single photo.

Synchronize lip movements with the cloned voice.

✅ Expected Outcome

By the end of this project, a user can upload a photo + voice sample, type any custom text, and receive a video of the avatar speaking in the cloned voice.

🛠 Tools & Technologies

Python

Google Colab (with free GPU)

Bark – Voice cloning model (open-source)

SadTalker – Face animation model (open-source)

📅 Project Timeline
Week 1 – Research and Setup

Study Bark (voice cloning) and SadTalker (face animation).

Run basic demos for both models on Google Colab.

Deliverable: A working Bark demo generating speech from text.
🔗 https://drive.google.com/file/d/1Qey63Rb-ZR6MwGSALAxg20uP5g2Xpi5O/view?usp=sharing

Week 2 – Voice Cloning Module

Implement a module that takes a 30–60 sec reference voice clip.

Clone the voice to speak any custom text.

Deliverable: Colab script that generates cloned voice from text.

Week 3 – Talking Avatar Module

Implement a module that takes a static photo + audio file.

Generate a video with synchronized lip movement using SadTalker.

Deliverable: Colab script that produces a talking video.
🔗 https://drive.google.com/file/d/1XBlPftLMZLuTdd3xmEM1btowX4KcjKzD/view?usp=sharing

🔗 https://drive.google.com/file/d/1CJ7uIlfVgHO1f5fNHXu3MyDKzSGo3xy7/view?usp=sharing

Week 4 – Integration and Final Output

Integrate Bark + SadTalker into a single pipeline.

Inputs: Photo, Reference Voice, Text

Output: Talking Avatar Video

Deliverables:

Final integrated Colab notebook

At least two demo videos

Documentation of setup & process

🔗 https://drive.google.com/file/d/15SXDIyzqMjIJ77jUtzCuaSB8wZ1VJ8C7/view?usp=sharing

🔗 https://drive.google.com/file/d/1DWFhAjtPAYlXCZv5Jevadn9zlkCi-fU9/view?usp=sharing

🚀 High-Level Steps
1. Setup Bark for Voice Cloning

pip install git+https://github.com/suno-ai/bark.git
python
Copy
Edit
from bark import generate_audio, SAMPLE_RATE
from scipy.io.wavfile import write

audio = generate_audio("Hello, this is AI-generated voice cloning.")
write("voice.wav", SAMPLE_RATE, audio)

2. Setup SadTalker for Lip-Sync Animation

git clone https://github.com/OpenTalker/SadTalker.git
cd SadTalker
pip install -r requirements.txt

Run SadTalker:

python inference.py --driven_audio voice.wav --source_image image.jpg --result_dir results

3. Integration Pipeline

Upload photo + reference voice

Clone voice with Bark

Generate talking avatar with SadTalker

📦 Deliverables at Project Completion

Integrated Google Colab Notebook

Two or more demo videos

Documentation of steps & results

Source code uploaded to GitHub

📊 Evaluation Criteria

End-to-end pipeline functionality

Quality of generated voice & video

Completeness of documentation

Bonus: Any enhancements

📜 License

This project is built entirely with open-source tools and does not use any paid APIs or services.

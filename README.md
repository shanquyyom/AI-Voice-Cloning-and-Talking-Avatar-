# AI Voice Cloning and Talking Avatar 🎙️🧑‍💻

This project integrates **Bark (voice cloning)** and **SadTalker (face animation)** to create a complete AI pipeline that can:

- Clone a person’s voice using a 30–60 second audio sample  
- Generate speech from text with the cloned voice  
- Animate a static image to produce a lip-synced talking avatar video  

---

## 🚀 Project Objective
Develop a pipeline that takes a single photo and a 30–60 second voice sample of a person, clones the voice using AI, and generates a talking video of that person where the lip movements are synchronized with the generated voice.

---

## 📌 Expected Outcome
By the end of this project, you will be able to:
- Upload a photo and a reference voice sample  
- Clone the voice to speak custom text  
- Generate a lip-synced talking video from the photo  

---

## 🛠️ Tools & Technologies
- **Python**  
- **Google Colab (Free GPU)**  
- **[Bark](https://github.com/suno-ai/bark) – Voice Cloning Model**  
- **[SadTalker](https://github.com/OpenTalker/SadTalker) – Face Animation Model**

---

## 📅 Project Timeline

### **Week 1 – Research and Setup**
- Study Bark (voice cloning) and SadTalker (face animation)  
- Run basic demos for both models  
- **Deliverable**: Working Bark demo generating speech from text  
- 🎧 [Demo Audio Link](https://drive.google.com/file/d/1Qey63Rb-ZR6MwGSALAxg20uP5g2Xpi5O/view?usp=sharing)

---

### **Week 2 – Voice Cloning Module**
- Implement a module that takes a 30–60s reference voice clip  
- Clone the voice to speak custom text  
- **Deliverable**: Colab script that generates cloned voice from text  

---

### **Week 3 – Talking Avatar Module**
- Implement a module that takes a static photo and audio file  
- Generate a lip-synced talking video using SadTalker  
- **Deliverable**: Colab script that produces a talking video from an image + audio  
- 🎥 Demo Videos:  
  - [Video 1](https://drive.google.com/file/d/1XBlPftLMZLuTdd3xmEM1btowX4KcjKzD/view?usp=sharing)  
  - [Video 2](https://drive.google.com/file/d/1CJ7uIlfVgHO1f5fNHXu3MyDKzSGo3xy7/view?usp=sharing)

---

### **Week 4 – Integration and Final Output**
- Integrate voice cloning + talking avatar into a single pipeline  
- **Input**: Photo + Reference Voice + Text  
- **Output**: Final Talking Avatar Video  
- **Deliverables**:  
  - Final Colab Notebook  
  - At least **two demo videos**  
  - Documentation of the process  
- 🎥 Demo Videos:  
  - [Video 1](https://drive.google.com/file/d/15SXDIyzqMjIJ77jUtzCuaSB8wZ1VJ8C7/view?usp=sharing)  
  - [Video 2](https://drive.google.com/file/d/1DWFhAjtPAYlXCZv5Jevadn9zlkCi-fU9/view?usp=sharing)

---

## 🔑 High-Level Steps

### 1. Setup Bark (Voice Cloning)
```bash
pip install git+https://github.com/suno-ai/bark.git


Example:
from bark import generate_audio, SAMPLE_RATE
from scipy.io.wavfile import write

audio = generate_audio("Hello, this is AI-generated voice cloning.")
write("voice.wav", SAMPLE_RATE, audio)

2. Setup SadTalker (Lip-Sync Animation)

git clone https://github.com/OpenTalker/SadTalker.git
cd SadTalker
pip install -r requirements.txt


Run SadTalker:
python inference.py --driven_audio voice.wav --source_image image.jpg --result_dir results

3. Integration (Full Pipeline)

Upload Photo + Reference Voice

Generate Cloned Voice from Text

Generate Talking Avatar Video with lip-sync

📦 Deliverables at Project Completion

Working Google Colab notebook with integrated pipeline

At least two demo videos with different inputs

Documentation of process

Source code uploaded to GitHub

📊 Evaluation Criteria

✅ End-to-end pipeline functionality

✅ Quality of cloned voice & generated video

✅ Clarity & completeness of documentation

✅ Additional improvements (if implemented)

⚖️ License

This project is based on open-source tools only and does not use any paid APIs or services.

✨ Author: Shan Quyyoom
📍 Location: Jhang, Pakistan
📧 Email: shanquyyoom5@gmail.com

🔗 LinkedIn


---

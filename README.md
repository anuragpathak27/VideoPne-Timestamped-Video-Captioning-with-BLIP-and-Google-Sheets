# VideoPne

**Automatically generate timestamped captions for videos using the BLIP image captioning model and log results into Google Sheets.**

---

## Features

- ⏱️ Extracts 1 frame per second from any video
- 🧠 Captions each frame using `Salesforce/blip-image-captioning-large`
- 📄 Logs each timestamp + caption to a Google Sheet
- 🧰 Designed for flexible workflows (Python + VS Code, n8n compatible)

## Setup Instructions

### 1. Clone this repository

```bash
git clone https://github.com/anuragpathak27/VideoPne-Timestamped-Video-Captioning-with-BLIP-and-Google-Sheets
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Add your video file

### 4. Google Sheets Integration
 - Go to [Google Cloud Console](https://console.cloud.google.com/).

 - Create a project > Enable Google Drive and Sheets API.

 - Create a Service Account and download the creds.json file.

 - Share your target Google Sheet with the service account email (it looks like xxxx@xxxx.iam.gserviceaccount.com).

### 5. Update the sheet name in main.py:

```bash
sheet = client.open("Video Captions").sheet1
```

### 6. Run the Script
```bash
python main.py
```
## Model Details
 - Hugging Face: Salesforce/blip-image-captioning-large

 - Uses Transformers and OpenCV

#### Anurag Pathak
[Linkedin](www.linkedin.com/in/anurag-pathak-ap27032004)

###  License
This project is licensed under the MIT License.

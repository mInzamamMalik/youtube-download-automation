# youtube video download automation


## Installation 🛠️

1. Download the `install.bat` file to your Windows machine. 📥
2. Right-click on the file and select **Run as administrator**. 👨‍💻

---

## Usage 🎬

1. Open the terminal in the folder where you'd like to download the video. 📂

2. Use the following commands depending on your needs:

### 1. Download the best quality YouTube video: 🎥
```bash
yt-dlp -f "bestvideo+bestaudio/best" -o "%(title)s.%(ext)s" "<YOUTUBE_URL>"
```

### 2. Download the best quality YouTube video with a maximum file size: 📦
```bash
yt-dlp -f "bestvideo+bestaudio/best" --format-sort "filesize" -o "%(title)s.%(ext)s" "<YOUTUBE_URL>"
```

> Note: The video will be downloaded to the same folder where the terminal is opened. 📂













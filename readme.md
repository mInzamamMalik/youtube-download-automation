# youtube video download automation

## Installation 🛠️

1. Download the `install.bat` file to your Windows machine. 📥
2. Right-click on the file and select **Run as administrator**. 👨‍💻

---

## Opening CMD in a Specific Folder

Here are a few ways to open the Command Prompt (cmd) already pointing to a folder:

* **File Explorer → Address Bar**

  1. Open File Explorer and navigate to the folder where you want to run commands.
  2. Click on the address bar, type `cmd`, and press **Enter**.
  3. A Command Prompt window will open, with its working directory set to that folder.

* **Shift + Right‑Click in Folder**

  1. In File Explorer, go to the folder you want.
  2. Hold down **Shift** and right-click inside an empty space (or on the folder background).
  3. Choose **“Open PowerShell window here”** or **“Open command window here”** (depending on your Windows version).
  4. If it opens PowerShell, you can still run `cmd` commands there, or type `cmd` to drop into a classic cmd prompt.

Once opened, the terminal’s current folder will be set to where you want to download the YouTube video.

---

## Usage 🎬

1. Open the terminal (CMD or PowerShell) in the folder where you’d like to download the video. 📂

2. Use the following commands depending on your needs. Below, replace `<YOUTUBE_URL>` with:

### 1. Download the best quality YouTube video: 🎥

```bash
yt-dlp -f "bestvideo+bestaudio/best" -o "%(title)s.%(ext)s" "https://www.youtube.com/watch?v=q0aFOxT6TNw"
```

### 2. Download the best quality YouTube video with a maximum file size: 📦

```bash
yt-dlp -f "bestvideo+bestaudio/best" --format-sort "filesize" -o "%(title)s.%(ext)s" "https://www.youtube.com/watch?v=q0aFOxT6TNw"
```

> Note: The video will be downloaded to the same folder where the terminal is opened. 📂

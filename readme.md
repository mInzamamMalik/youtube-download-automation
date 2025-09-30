# YouTube Video Download Automation

## Installation 🛠️

1. **Download** the `install.bat` file to your Windows machine. 📥
2. **Right-click** on the file and select **Run as administrator**. 👨‍💻

---

## Opening CMD in a Specific Folder

Here are a few ways to open **Command Prompt (CMD)** already pointing to a specific folder:

### 1. **File Explorer → Address Bar**

1. Open **File Explorer** and navigate to the folder where you want to run commands.
2. Click on the **address bar**, type `cmd`, and press **Enter**.
3. A **Command Prompt** window will open, with its working directory set to that folder.

### 2. **Shift + Right-click in Folder**

1. In **File Explorer**, go to the folder you want.
2. Hold down **Shift** and right-click inside an empty space (or on the folder background).
3. Choose **“Open PowerShell window here”** or **“Open command window here”** (depending on your Windows version).
4. If PowerShell opens, you can still run `cmd` commands there or simply type `cmd` to switch to the classic **CMD prompt**.

Once opened, the terminal’s current folder will be set to where you want to download the YouTube video.

---

## Usage 🎬

### 1. Open the terminal (CMD or PowerShell) in the folder where you’d like to download the video. 📂

### 2. Use the following commands based on your needs. Replace `<YOUTUBE_URL>` with your video URL:

#### **1. Download the best quality YouTube video** 🎥

```bash
yt-dlp -f "bestvideo+bestaudio/best" -o "%(title)s.%(ext)s" "https://www.youtube.com/watch?v=q0aFOxT6TNw"
```

#### **2. Download the best quality YouTube video with a maximum file size** 📦

```bash
yt-dlp -f "bestvideo+bestaudio/best" --format-sort "filesize" -o "%(title)s.%(ext)s" "https://www.youtube.com/watch?v=q0aFOxT6TNw"
```

> **Note:** The video will be downloaded to the same folder where the terminal is opened. 📂

---

## Downloading Videos from a Links File 📋

If you have a text file containing multiple YouTube video links, you can download all of them in batch using the following steps:

### 1. **Prepare your links file**

Create a text file (e.g., `links.txt`) containing all the YouTube video URLs you want to download. Make sure each link is on a separate line. Example:

```txt
https://www.youtube.com/watch?v=video1
https://www.youtube.com/watch?v=video2
https://www.youtube.com/watch?v=video3
```

### 2. **Run the download command**

In your terminal (CMD or PowerShell), navigate to the folder where your `links.txt` file is located. Then, use one of the following commands to download all the videos listed in the file:

#### **1. Download the best quality YouTube video using links file** 🎥

```bash
yt-dlp -f "bestvideo+bestaudio/best" -o "%(title)s.%(ext)s" -a links.txt
```

#### **2. Download the best quality YouTube video with a maximum file size using links file** 📦

```bash
yt-dlp -f "bestvideo+bestaudio/best" --format-sort "filesize" -o "%(title)s.%(ext)s" -a links.txt
```

> **Note:** The videos will be downloaded to the same folder where the terminal is opened. 📂

---

# Using the Link Grabber Extension to Download Multiple YouTube or TikTok Videos

You can use the **Link Grabber** Chrome extension to extract all the links from a webpage:
🔗 [Link Grabber Extension](https://chromewebstore.google.com/detail/link-grabber/caodelkhipncidmoebgbbeemedohcdma)

For example, if you visit a page containing multiple YouTube or TikTok videos (e.g., this TikTok profile: [@shugli_loog_officail](https://www.tiktok.com/@shugli_loog_officail)), you can use the extension to collect all video links at once.

### Steps:

1. **Install the Link Grabber extension**
   👉 [Install from Chrome Web Store](https://chromewebstore.google.com/detail/link-grabber/caodelkhipncidmoebgbbeemedohcdma)

2. **Pin the extension** to your Chrome toolbar for easy access.

3. **Open the page** that contains multiple videos, such as:
   [https://www.tiktok.com/@shugli_loog_officail](https://www.tiktok.com/@shugli_loog_officail)

4. **Click the Link Grabber icon** in your toolbar. A new tab will open displaying all the links found on the page.

5. **Copy the relevant video links** and paste them into a file named `links.txt`.

6. **Save `links.txt`** in your desired folder.

7. **Open Command Prompt** in that same folder and run the command as described in the
   **"Downloading Videos from a Links File"** section.

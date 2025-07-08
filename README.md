<p align="center">
  <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/blob/f11f527067f9a37ed0f6fc9123b9f9ce99763c66/img/img_v1.5.7-medio.png" alt="Medio Logo" width="128" />
</p>
<h1 align="center">Medio - Universal Downloader</h1>
<p align="center">
  <b>Effortlessly download videos, extract high-quality audio and save entire playlists from multiple platforms.</b><br>
  <b>Experience a fast, reliable and feature-rich universal downloader optimized for performance.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/Medio-Universal-Downloader/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/Medio-Universal-Downloader?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/Medio-Universal-Downloader/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Commercial-red?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/8.0/runtime"><img src="https://img.shields.io/badge/.NET-8.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/Medio-Universal-Downloader/issues"><img src="https://img.shields.io/badge/Issues-0_open-orange?style=flat-square" alt="Open Issues"></a>
</p>

**Medio** is a user-friendly software for downloading video content from various online platforms. Whether you're looking to save videos, extract audio or download entire playlists, Medio provides an all-in-one tool to meet your needs. Its simple, intuitive interface lets you quickly input a URL, choose your desired quality and filename, and start the download with just a few clicks.

### **Key Features**

- **Video Downloads:** Download videos from various platforms in a variety of formats and qualities, so you can enjoy your favorite content offline whenever you need it.
- **Audio Extraction:** If you only need the audio, Medio makes it easy to extract and download the audio from any supported video.
- **Playlist Downloads:** With Medio, you can download entire playlists at once, saving you time and effort. This is especially helpful for users who want to bulk-download videos for offline viewing.
- **Universal Downloads:** Download videos from numerous platforms and websites, making it a truly universal downloader for your media needs.

### **Supported Formats**

Medio supports a wide range of video and audio formats:

- **Video Formats:** `MP4`, `MKV`, `AVI`, `FLV`, `WMV`, `MOV`
- **Audio Formats:** `MP3`, `OGG`, `WAV`, `M4A`, `AAC`, `WMA`

### **Quality Control**

Medio lets you choose from various video and audio quality options:

- **Video Quality Options:** `4320p`, `2160p`, `1440p`, `1080p`, `720p`, `480p`, `360p`, `240p`, `144p`
- **Audio Quality Options:** `320k`, `256k`, `160k`, `128k`, `96k`, `64k`, `48k`, `32k`
  
Medio uses ffmpeg to recode audio, ensuring the final file matches your selected quality down to `32 kbps` if needed. When your selected quality isn't available on the source platform, Medio **automatically** selects the **highest available** quality for the unavailable option.

**Note on URL Validation:** YouTube URLs are validated quickly, while other platforms may take a few extra seconds to process. This is normal behavior to ensure compatibility with various sources.

## **Table of Contents**

1. [System Requirements](#system-requirements)
   - [Minimum Requirements](#minimum-requirements)
   - [Recommended Requirements](#recommended-requirements)
2. [Third-Party Libraries](#third-party-libraries)
   - [FFmpeg](#ffmpeg)
   - [yt-dlp](#yt-dlp)
   - [Additional Information](#additional-information)
3. [License Options and Benefits](#license-options-and-benefits)
4. [Data Collection and Account Management](#data-collection-and-account-management)
5. [Key Activation and Data Sync](#key-activation-and-data-sync)
6. [Free Trial License Key](#free-trial-license-key)
7. [Getting Started Guide](#getting-started-guide)
   - [Step 1: Configure Your Settings](#step-1-configure-your-settings)
     - [Open the Settings Menu](#step-1-configure-your-settings)
     - [Set Your Preferences](#step-1-configure-your-settings)
   - [Step 2: Download Your Content](#step-2-download-your-content)
     - [Access the Downloader](#step-2-download-your-content)
     - [Select Download Type](#step-2-download-your-content)
     - [Enter the URL](#step-2-download-your-content)
     - [Configure Download Options](#step-2-download-your-content)
     - [Initiate the Download](#step-2-download-your-content)
8. [Download Status Guide](#download-status-guide)
9. [Updating Software](#updating-software)
10. [Running Medio on Linux](#running-medio-on-linux)
    - [Installation Guide](#installation-guide)
11. [Hardware Acceleration](#hardware-acceleration)
12. [Copyright](#copyright)
13. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**
- **Operating System:** Windows 10 (64-bit)
- **Processor:** Intel Core i3 or AMD Ryzen 3
- **RAM:** 4 GB
- **Storage:** 200 MB of free disk space
- **Software:** .NET 8.0 Runtime
  - [Download .NET 8.0 Runtime](https://dotnet.microsoft.com/download/dotnet/8.0/runtime)
- **Internet:** Broadband connection (2 Mbps or faster)

### **Recommended Requirements**
- **Operating System:** Windows 10/11 (64-bit)
- **Processor:** Intel Core i5/i7 or AMD Ryzen 5/7
- **RAM:** 8 GB or higher
- **Storage:** 300 MB of free disk space
- **Software:** .NET 8.0 Runtime
  - [Download .NET 8.0 Runtime](https://dotnet.microsoft.com/download/dotnet/8.0/runtime)
- **Internet:** High-speed broadband connection (10 Mbps or faster)

## Third-Party Libraries

Medio uses two main third-party libraries to handle media processing and downloads: **FFmpeg** and **yt-dlp**.

### FFmpeg

**FFmpeg** is a multimedia framework that handles video, audio, and other media files. It takes care of format conversion and media encoding/decoding. Medio automatically checks for and installs the latest FFmpeg version to ensure everything works smoothly.

- **Website:** [FFmpeg Official Website](https://ffmpeg.org)
- **License:** FFmpeg is licensed under the LGPL or GPL, depending on the configuration and features used.

### yt-dlp

**yt-dlp** is an open-source command-line tool for downloading videos from various platforms. Medio integrates yt-dlp to handle content extraction and downloads from a wide range of sources. This library is automatically updated to stay compatible with the latest website changes.

- **Website:** [yt-dlp GitHub Repository](https://github.com/yt-dlp/yt-dlp)
- **License:** yt-dlp is licensed under the Unlicense, allowing free use, distribution, and modification.

### Additional Information

For more details about FFmpeg and yt-dlp, including their capabilities and licensing, check their official documentation:

- **FFmpeg Documentation:** [FFmpeg Documentation](https://ffmpeg.org/documentation.html)
- **yt-dlp Documentation:** [yt-dlp Documentation](https://github.com/yt-dlp/yt-dlp#readme)

If you have questions or issues related to these libraries, please [open an issue](https://github.com/BerndHagen/Medio-Universal-Downloader/issues) on GitHub.

## **License Options and Benefits**

Medio is **free** for YouTube downloads, allowing unlimited retrieval of video and audio files in multiple formats. Premium licenses unlock features such as **YouTube playlist** downloads, while Ultimate licenses provide support for **additional platforms** beyond YouTube. After purchasing through Stripe's secure payment system, you'll receive your license key via email from Arctisoft-Studio within **5-10 minutes**.

<p align="center">
  <img src="img/img_v1.5.8-medio_licenses.png" alt="Medio Plans" />
</p>

Multiple payment methods are accepted including Card, Klarna, EPS, Bancontact and iDEAL. Since licenses are digital products, refunds are generally **not available** once the key has been delivered. However, if you encounter any issues during the activation process, please don't hesitate to reach out for assistance.

## Data Collection and Account Management

Medio collects account data to improve your experience and sync settings across devices. When you first launch the software, an account is automatically created. The data collected includes:

- Personal settings and preferences
- Selected avatar and profile customizations
- Account creation date and activity metrics
- Experience points and current level
- Total megabytes downloaded
- Total number of audio and video files downloaded
- Download history such as titles and dates
- Remaining downloads for trial license users
- Current license status (Basic, Premium or Ultimate)

**Note:** Your account data is used **solely** for synchronization and feature access. No personal data is shared with third parties.

## Key Activation and Data Sync

Once you purchase and redeem a key in the Settings tab under **Key Activation**, it can always retrieve your latest account data from Medio's database. This includes your complete download history, settings, profile customizations, experience points, statistics and license status, keeping everything synchronized across sessions and devices when using Premium or Ultimate licenses.

- **Basic License** accounts are automatically deleted after **180 days** of inactivity to maintain database efficiency.
- **Premium** and **Ultimate License** users are **exempt from this time limit** and can maintain their accounts indefinitely.

**Note:** Once an account is deleted, it **cannot be restored**. All associated data is permanently removed.

## **Free Trial License Key**

Try selected Premium features with this one-time trial license key. It provides faster download speeds, YouTube playlist downloads and expanded history storage up to 50 entries. The trial is limited to **10** downloads before Premium features are disabled.

**Unlock Medio's Premium Features:**
```yaml
License Key:     PT4O-5TYD-WKTV-0ZZ7
```

Once redeemed, this key becomes invalid and can't be used again. After reaching the download limit, Premium features will no longer be accessible.

## **Getting Started Guide**

Follow these steps to start downloading content:

### **Step 1: Configure Your Settings**

1. **Open the Settings Menu**
   - Launch **Medio** and go to the `Settings` tab.

2. **Set Your Preferences**
   - **Format:** Choose your preferred video or audio format for downloads.
   - **Additional Settings:** Adjust settings like buffer size to suit your needs.

### **Step 2: Download Your Content**

1. **Access the Downloader**
   - Go to the **Downloader** tab in the sidebar.

2. **Select Download Type**
   - Choose whether to download the **video** or extract only the **audio** from your URL.

3. **Enter the URL**
   - Paste the video link into the input field at the top of the **Downloader** page.
   - Note: YouTube URLs validate quickly, while other platforms may take a few extra seconds.

4. **Configure Download Options**

   - **Save Location:**
     - Click the `...` button next to the directory path field to select where files are saved.
     - By default, a folder named `Medio` is created and used for downloads, but you can choose any location you prefer.
     - For playlists, consider creating a dedicated folder to keep files organized.
     
   - **File Name:**
     - Enter a custom name in the `Title your Video` field.
     - For playlists, original video titles are used automatically.
     
   - **Select Quality:**
     - Choose your preferred resolution from the available options. Lower quality means smaller file sizes.

5. **Initiate the Download**
   - Click the `Start Download` button to begin.
   - **Monitor Progress:** Check the progress in the upper-right corner. The process includes:
     - **Loading Tools** – *Medio* is initializing required components
     - **Building Command** – Assembling command arguments for **yt-dlp** and **FFmpeg** based on your settings
     - **Executing** – Running the generated command to download and process the media
     - **Downloading** – Displays live download progress, including speed and segment information
     - **Converting: X%** – Shows conversion progress, including conversion speed and video duration

**Note:** If you enter an unsupported URL, the software will show an `Invalid Link` or `Content Blocked` status. Files with the same name and format in the specified download path will be **automatically skipped**. If the status shows `Network Error`, the download was interrupted due to a lost internet connection. For successful downloads, especially complete playlists, ensure your internet connection is stable.

## **Download Status Guide**

During downloads and conversions, Medio provides detailed status information to keep you informed about what's happening. These status indicators help you understand the current operation and identify any issues.

Below are the status messages you may encounter:

| Status                | Description                                                             |
|------------------------|-------------------------------------------------------------------------|
| `Loading Tools`        | Initializing download components and preparing resources               |
| `Building Command`     | Assembling command arguments for yt-dlp and ffmpeg                     |
| `Executing`            | Running the generated command to process the media                     |
| `Preparing Next`       | Processing the next video in a playlist after successful download      |
| `Invalid Link`         | URL is not recognized or supported                                     |
| `Network Error`        | Connection lost during download or insufficient bandwidth              |
| `Premium Required`     | Feature requires Premium license activation                            |
| `Ultimate Required`    | Feature requires Ultimate license activation                           |
| `Extract Audio`        | Converting video to audio format                                       |
| `Extracting Subtitles` | Downloading and saving subtitle tracks if available                    |
| `Remuxing Video`       | Repackaging video without re-encoding                                  |
| `Getting Thumbnail`    | Downloading the video's thumbnail image                                |
| `Process Stopped`      | Download manually stopped by the user                                  |
| `Converting Format`    | Transforming media to selected format                                  |
| `Merging Files`        | Combining audio and video streams                                      |
| `Adding Metadata`      | Embedding title, artist, and other information                         |
| `Processing Segments`  | Handling individual parts of fragmented content                        |
| `Content Blocked`      | yt-dlp cannot download from this source                                |
| `Copyright Error`      | Content is protected by copyright and cannot be downloaded             |
| `Playlist Error`       | Playlist information could not be gathered from the provided link      |
| `Completed`            | Download and processing successfully finished                          |

If you encounter an `Unknown Error`, this indicates an unexpected issue that hasn't been accounted for. If this error persists, please report it in the [GitHub issue section](https://github.com/BerndHagen/Medio-Universal-Downloader/issues) with details about what you were trying to download and your settings.

## **Updating Software**

Keep Medio updated to ensure it continues working properly. Updates introduce new features and fix bugs that could cause issues like incomplete downloads or conversion errors. Running an outdated version may lead to problems. You can check your current version by looking at the Build Number in the bottom left corner of the application.

**Automatic Update Feature (Available since Version 1.5.4):**

Starting with **version 1.5.4**, Medio includes an automatic update system that handles the update process:

- **Automatic Detection:** The app checks for updates on startup and compares your version with the latest release
- **Smart Download:** If a newer version is available, Medio automatically downloads the update
- **Seamless Installation:** The update installs automatically with minimal user intervention
- **Restart Integration:** After installation, the app restarts with the new version

**Manual Update Process:**

If you prefer to update manually or need to troubleshoot update issues:

1. Download the latest version from the repository and save it to your device.
2. Run the downloaded **MSI** installer to begin installation.
3. Follow the installation wizard to replace old files with updates.
4. Once installation is complete, launch the application.

Make sure the installation path is set to `C:\Users\...\AppData\Local\Arctisoft-Studio\Medio - Universal Downloader` to prevent issues and ensure features aren't blocked due to lack of administrative rights.

## Running Medio on Linux

Starting with **version 1.5.5**, Medio works better on non-Windows systems. While the app is still **primarily** optimized for **Windows**, Linux users can now run Medio through `Wine` with improved stability. However, some features might not work exactly as they do on Windows. Visual elements like the **Verdana** font are **not natively supported** on Linux, resulting in slightly different font rendering.

### Installation Guide

1. Install Wine for your distribution:
```yaml
sudo apt install wine64    # Ubuntu
sudo dnf install wine      # Fedora
sudo pacman -S wine        # Arch Linux
```

2. Download the Medio setup file from GitHub and save it to your Desktop.

3. Navigate to your Desktop:
```yaml
cd ~/Desktop
```

4. Install Medio:
```yaml
wine setup.msi
```

5. After installation, run Medio through Wine:
```yaml
wine "C:\Program Files\Medio\Medio.exe"
```

If you encounter technical issues during installation or usage, please visit our [GitHub issues page](https://github.com/BerndHagen/Medio-Universal-Downloader/issues) for support.

## **Hardware Acceleration**

Medio supports hardware acceleration to optimize video processing performance. This feature uses your system's **GPU** resources for better media handling, resulting in significant **improvements to conversion speeds**. The app automatically detects the best hardware acceleration method through FFmpeg's `-hwaccel auto` parameter, which can use technologies like **NVIDIA NVENC, AMD AMF**, or **Intel QuickSync** depending on your hardware.

### Processing Types and Benefits

1. **CPU Only Processing**
   - Basic processing capability
   - Best for lower resolution content
   - Uses standard system resources

2. **GPU Accelerated Processing**
   - Optimal for high-resolution videos (1440p-4320p)
   - Uses graphics card for better performance
   - Significantly reduces CPU load

3. **Hybrid Processing**
   - Balances workload between CPU and GPU
   - Provides maximum efficiency
   - Automatically adjusts based on content type

Hardware acceleration provides several advantages for media processing:

- **Processing Speed:** GPU acceleration reduces CPU load by up to **75%**, enabling faster video encoding and decoding
- **Quality Management:** Maintains high-quality output while significantly reducing processing time
- **Resource Optimization:** Intelligent distribution of workload between CPU and GPU resources
- **Power Efficiency:** Reduced system resource utilization during intensive operations

**Note:** While hardware acceleration is available on most modern systems, performance benefits may vary **based on your specific hardware configuration** and the **complexity of the media** being processed.

## **Copyright**

This software is the intellectual property of the Author and is protected by international copyright laws. This copyright notice outlines the key terms governing the use, distribution, and modification of the software:

1. **License**: You are granted a revocable, non-exclusive, non-transferable license to download, install, and use the software for personal, non-commercial purposes.

2. **Modifications Prohibited**: Any modification, decompiling, reverse-engineering, or derivative work based on the software is strictly prohibited without the Author's prior written consent.

3. **Attribution**: When redistributing Medio - Universal Downloader, appropriate credit to the Author is required, including a link to the original source when applicable.

4. **Third-Party Libraries**: Medio uses third-party libraries like FFmpeg (LGPL) and yt-dlp (Unlicense) for multimedia processing. Please review and comply with their respective licenses.

5. **Warranty Disclaimer**: Medio is provided *"as is,"* without warranties of any kind, express or implied. The Author assumes no liability for damages resulting from the use of the software.

6. **Limitation of Liability**: The Author is not responsible for any indirect, special, incidental, or consequential damages arising out of the use or inability to use the software.

7. **Termination**: The license to use this software may be terminated if the terms of this notice are violated. Upon termination, all use must cease and copies must be deleted.

By using Medio - Universal Downloader, you agree to these terms and conditions. Failure to comply may result in legal action and revocation of your rights to use the software. For full details on licensing terms and further information, please refer to the [LICENSE](https://github.com/BerndHagen/Medio-Universal-Downloader/blob/main/LICENSE) file.

## **Screenshots**

If you'd like a preview of Medio before downloading, the screenshots below show the application's features. Note that future updates may introduce additional functionality.

<table>
  <tr>
    <th>Medio - Dashboard Page</th>
    <th>Medio - Downloader Page</th>
    <th>Medio - History Page</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_dashboard.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_dashboard.png" alt="Medio Dashboard" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_converter.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_converter.png" alt="Medio Downloader" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_history.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_history.png" alt="Medio History" width="300"></a></td>
  </tr>

  <tr>
    <th>Medio - Premium Page</th>
    <th>Medio - Activation Page</th>
    <th>Medio - Settings Page</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_premium.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_premium.png" alt="Medio Premium" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_redeem.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_redeem.png" alt="Medio Activation" width="300"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_settings.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.8-medio_settings.png" alt="Medio Settings" width="300"></a></td>
  </tr>
</table>
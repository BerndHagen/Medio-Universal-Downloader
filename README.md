<p align="center">
  <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_medio.png" alt="Medio Logo" width="128" />
</p>
<h1 align="center">Medio - Universal Downloader</h1>
<p align="center">
  <b>Effortlessly download videos, extract high-quality audio and save entire playlists from multiple platforms.</b><br>
  <b>Experience a fast, reliable and feature-rich universal downloader optimized for performance.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/Medio-Universal-Downloader/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/Medio-Universal-Downloader?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/Medio-Universal-Downloader/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freemium-red?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/Medio-Universal-Downloader/issues"><img src="https://img.shields.io/badge/Issues-0_open-orange?style=flat-square" alt="Open Issues"></a>
</p>

**Medio** is a user-friendly software for downloading video content from various online platforms. Whether you're looking to save videos, extract audio or download entire playlists, Medio provides an all-in-one tool to meet your needs. Its simple, intuitive interface lets you quickly input a URL, choose your desired quality and filename, and start the download with just a few clicks.

### **Key Features**

- **Video Downloads:** Download videos from various platforms in a variety of formats and qualities, so you can enjoy your favorite content offline whenever you need it.
- **Audio Extraction:** If you only need the audio, Medio makes it easy to extract and download the audio from any supported video.
- **Playlist Downloads:** With Medio, you can download entire playlists at once, saving you time and effort. This is especially helpful for users who want to bulk-download videos for offline viewing.
- **Queue Functionality:** Add multiple videos for sequential automated downloading with improved resilience for protected content.
- **Advanced Customization:** Fine-tune downloads with hardware acceleration GPU selection, download speed limits, audio normalization, metadata embedding, and preferred video codecs.
- **Universal Downloads:** Download videos from numerous platforms and websites, making it a truly universal downloader for your media needs.
- **Taskbar Integration:** View real-time download progress directly in the Windows taskbar for convenient monitoring without switching windows.
- **System Notifications:** Receive desktop notifications when downloads complete, with quick access to open the downloaded file or its folder location.

### **Supported Formats**

Medio supports a wide range of video and audio formats:

- **Video Formats:** `MP4`, `MKV`, `AVI`, `WEBM`, `WMV`, `MOV`
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
4. [Data Collection and Automatic Profile System](#data-collection-and-automatic-profile-system)
   - [How It Works](#how-it-works)
   - [Collected Profile Data](#collected-profile-data)
5. [License Key Activation and Profile Synchronization](#license-key-activation-and-profile-synchronization)
6. [Free Trial License Key](#free-trial-license-key)
7. [Getting Started Guide](#getting-started-guide)
   - [Step 1: Configure Your Settings](#step-1-configure-your-settings)
   - [Step 2: Download Your Content](#step-2-download-your-content)
8. [Advanced Settings](#advanced-settings)
9. [Download Status Guide](#download-status-guide)
   - [Progress Status Messages](#progress-status-messages)
   - [Error Status Messages](#error-status-messages)
10. [Hardware Acceleration](#hardware-acceleration)
    - [Processing Types and Benefits](#processing-types-and-benefits)
11. [Copyright](#copyright)
12. [Screenshots](#screenshots)

## **System Requirements**

### **Minimum Requirements**
- **Operating System:** Windows 10 (64-bit) version 1809 or later
- **Processor:** Intel Core i3-8100 or AMD Ryzen 3 2200G with 4 cores at 3.0 GHz
- **RAM:** 8 GB
- **Graphics:** DirectX 11 compatible graphics card with integrated graphics acceptable
- **Storage:** 500 MB of free disk space plus additional space for downloads
- **Software:** .NET 10.0 Runtime ([Download](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)) - **Not required as application is self-contained**
- **Internet:** Stable broadband connection (5 Mbps or faster)

### **Recommended Requirements**
- **Operating System:** Windows 10/11 (64-bit) version 21H2 or later
- **Processor:** Intel Core i5-10400 or AMD Ryzen 5 3600 with 6 cores, 3.6 GHz or higher
- **RAM:** 16 GB or higher
- **Graphics:** Dedicated GPU with hardware acceleration support
  - **NVIDIA:** GTX 1060 or RTX 2060 or newer with NVENC support
  - **AMD:** RX 580 or RX 6600 or newer with AMF support
  - **Intel:** Arc A380 or newer with QuickSync support, integrated Iris Xe graphics acceptable
- **Storage:** 1 GB of free disk space on SSD plus additional space for downloads
- **Software:** .NET 10.0 Runtime ([Download](https://dotnet.microsoft.com/download/dotnet/10.0/runtime)) - **Not required as application is self-contained**
- **Internet:** High-speed broadband connection (25 Mbps or faster)

**Note:** Medio is designed exclusively for Windows. Linux and macOS are not supported, even through compatibility layers like Wine. The .NET 10.0 Runtime is bundled directly in the installer, allowing Medio to start immediately without requiring separate installation.

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

| Feature                                                                                           | Basic <br> License | Premium<br> License | Ultimate<br> License |
| ------------------------------------------------------------------------------------------------- | :----------------: | :-----------------: | :------------------: |
| Download unlimited videos and audios from YouTube without restrictions                        |          ✔         |          ✔          |           ✔          |
| Optimized hardware-accelerated video conversion using supported GPUs      |          ✔         |          ✔          |           ✔          |
| Automatically embeds full metadata into downloaded video and audio files             |          ✔         |          ✔          |           ✔          |
| Increased download speed for faster downloads and improved performance                           |          ✖         |          ✔          |           ✔          |
| Extended download history with more entries to record your recent activity            |          ✖         |          ✔          |           ✔          |
| Save time by downloading full YouTube playlists with a single click                 |          ✖         |          ✔          |           ✔          |
| Access your download history and profile data from any device anywhere                           |          ✖         |          ✔          |           ✔          |
| Supports high-resolution formats like 2160p and 4320p for sharp quality                     |          ✖         |          ✖          |           ✔          |
| Download content from numerous supported websites outside of YouTube                       |          ✖         |          ✖          |           ✔          |
| **Price**                                                                                        |      **€0.00**     |      **€1.99**      |       **€4.99**      |

Download speed and history limits depend on your license level:  
- **Basic:** Download speed of up to **5 MB/s** and up to **10** download history entries.  
- **Premium:** Download speed of up to **25 MB/s** and up to **50** download history entries.  
- **Ultimate:** Download speed **without limits** and up to **100** download history entries.


Multiple payment methods are accepted including Card, Klarna, EPS, Bancontact and iDEAL. Since licenses are digital products, refunds are generally **not available** once the key has been delivered. However, if you encounter any issues during the activation process, please don't hesitate to reach out for assistance.

## Data Collection and Automatic Profile System

Medio uses an automatic, registration-free profile system to enhance your experience and sync settings across devices. **No manual account creation is required** – everything happens automatically in the background.

### How It Works

**First Launch:**
- When you first start Medio, a unique profile is automatically created
- Your device is securely identified without requiring any personal information
- No usernames, passwords, or email addresses are needed

**Data Storage:**
- Your profile data is securely stored in Medio's cloud database
- This includes settings, preferences, download history, and license status
- All data is protected and linked to your unique profile

**Cross-Device Sync (Premium/Ultimate):**
- When you activate a license key, it becomes linked to your profile
- Enter the same license key on another device to access your complete profile
- This syncs your download history, settings, statistics, and license status seamlessly

### Collected Profile Data

Your profile includes:

- Personal settings and preferences
- Selected avatar and profile customizations
- Profile creation date and activity metrics
- Experience points and current level
- Total megabytes downloaded
- Total number of audio and video files downloaded
- Download history such as titles, dates and links (**only if "Track and save downloads in history" is enabled in Advanced Settings**)
- Remaining downloads for trial license users
- Current license status (Basic, Premium or Ultimate)

**Privacy Note:** Your profile data is used solely for synchronization and feature access. No personal identifying information is collected, and data is not shared with third parties. Individual download history entries can be deleted via the context menu.

## License Key Activation and Profile Synchronization

Your license key serves as both a feature unlock and a profile synchronization tool:

**How License Keys Work:**
- Each license key is permanently linked to your profile upon first activation
- Use the same key on multiple devices to access your synchronized profile data
- Entering your key on a new device instantly retrieves your complete profile
- Includes download history, settings, customizations, and statistics

**Profile Retention Policy:**
- **Basic License:** Profiles inactive for **180 days** are automatically removed to maintain database efficiency
- **Premium/Ultimate License:** Profiles are maintained indefinitely with no time restrictions

**Important:** Deleted profiles cannot be restored. All associated data is permanently removed.

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
   - **Advanced Settings:** Access the Advanced Settings section for GPU selection, download speed limits, audio normalization, metadata embedding, and codec preferences.

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
     - **Downloading** – Displays live download progress, including speed and segment information
     - **Converting** – Shows conversion progress, including conversion speed and video duration

**Note:** If you enter an unsupported URL, the software will show an `Unsupported Link` or `Content Blocked` status. Files with the same name and format in the specified download path will be **automatically skipped**. If the status shows `Network Error`, the download was interrupted due to a lost internet connection. For successful downloads, especially complete playlists, ensure your internet connection is stable.

## **Advanced Settings**

For advanced users, Medio offers an Advanced Settings section accessible from the main navigation, allowing fine-tuned control over download and conversion processes:

- **Hardware Acceleration:** Manually select GPU acceleration (NVIDIA, AMD, Intel) or disable for CPU-only processing, with improved detection for legacy hardware.
- **Download Speed Limit:** Configure maximum download speeds from 1 MB/s to unlimited to manage bandwidth usage.
- **Privacy Mode:** Enable or disable download history logging for privacy-focused usage.
- **Audio Normalization:** Adjust volume levels (Disabled, Light, Medium, Strong, Aggressive) for consistent audio playback quality.
- **Metadata Embedding:** Toggle inclusion of thumbnails and metadata in downloaded files.
- **Video Codec:** Choose preferred codecs (H.264, H.265, VP8, VP9, AV1, MPEG-4) for encoding compatibility.

These settings are synchronized across devices for Premium and Ultimate users.

## **Download Status Guide**

During downloads and conversions, Medio provides detailed status information to keep you informed about what's happening. These status indicators help you understand the current operation and identify any issues.

Below are the status messages you may encounter:

### Progress Status Messages

| Status                  | Description                                                             |
|-------------------------|-------------------------------------------------------------------------|
| `Scanning`              | Validating and analyzing the provided URL                              |
| `Loading Tools`         | Initializing download components and preparing resources               |
| `Building Command`      | Assembling command arguments for yt-dlp and ffmpeg                     |
| `Preparing Next`        | Processing the next video in a playlist/queue after successful download |
| `Downloading: XX%`      | Live download progress with percentage and speed information           |
| `Converting: XX%`       | Video conversion progress with speed and duration information          |
| `Merging Files`         | Combining audio and video streams into final output                    |
| `Extract Audio`         | Extracting and converting audio from video content                     |
| `Extracting Subtitles`  | Downloading and saving subtitle tracks if available                    |
| `Remuxing Video`        | Repackaging video container without re-encoding                        |
| `Getting Thumbnail`     | Downloading the video's thumbnail image for embedding                  |
| `Converting Format`     | Transforming media to selected output format                           |
| `Adding Metadata`       | Embedding title, artist, and other information into file               |
| `Processing Segments`   | Handling individual parts of fragmented or sponsored content           |
| `Cancelling`            | Aborting the download process and cleaning up resources                |
| `Process Stopped`       | Download manually stopped by the user                                  |
| `Completed`             | Download and processing successfully finished                          |

### Error Status Messages

| Status                  | Description                                                             |
|-------------------------|-------------------------------------------------------------------------|
| `Empty Link`            | URL field is empty and requires a valid video link                     |
| `Invalid Link`          | Link does not have a typical URL format or structure                   |
| `Unsupported Link`      | URL is not supported by the download engine                            |
| `Network Error`         | Connection lost during download or insufficient bandwidth              |
| `Content Blocked`       | yt-dlp cannot download from this source due to restrictions            |
| `Copyright Error`       | Content is protected by copyright and cannot be downloaded             |
| `File Exists`           | Content already exists in the directory and will be skipped            |
| `Playlist Error`        | Playlist information could not be gathered from the provided link      |
| `Tools Missing`         | Required tools (yt-dlp or ffmpeg) could not be found                   |
| `Premium Required`      | Feature requires Premium license activation                            |
| `Ultimate Required`     | Feature requires Ultimate license activation                           |

If you encounter an `Unknown Error`, this indicates an unexpected issue that hasn't been accounted for. If this error persists, please report it in the [GitHub issue section](https://github.com/BerndHagen/Medio-Universal-Downloader/issues) with details about what you were trying to download and your settings.

## **Hardware Acceleration**

Medio supports hardware acceleration to optimize video processing performance. This feature uses your system's **GPU** resources for better media handling, resulting in significant **improvements to conversion speeds**. Users can manually select their preferred GPU acceleration method (NVIDIA NVENC, AMD AMF, Intel QuickSync) or disable it entirely for CPU-only processing, with improved detection ensuring compatibility with legacy or unsupported hardware.

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
    <th>Medio - Dashboard</th>
    <th>Medio - Downloader</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_dashboard.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_dashboard.png" alt="Medio Dashboard" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_converter.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_converter.png" alt="Medio Downloader" width="450"></a></td>
  </tr>
  <tr>
    <th>Medio - History</th>
    <th>Medio - Licenses</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_history.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_history.png" alt="Medio History" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_licenses.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_licenses.png" alt="Medio Licenses" width="450"></a></td>
  </tr>
  <tr>
    <th>Medio - Activation</th>
    <th>Medio - Settings</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_redeem.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_redeem.png" alt="Medio Activation" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_settings.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.6.9-medio_settings.png" alt="Medio Settings" width="450"></a></td>
  </tr>
</table>

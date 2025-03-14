<p align="center">
  <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/blob/6ed6fb1aa6f46ef37befbd9c73e4f4cae3d04867/img/img_v1.5.5-medio.png" alt="Medio Logo" width="128" />
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

Medio gives you the flexibility to choose from a wide range of video and audio qualities:

- **Video Quality Options:** `4320p`, `2160p`, `1440p`, `1080p`, `720p`, `480p`, `360p`, `240p`, `144p`
- **Audio Quality Options:** `320k`, `256k`, `160k`, `128k`, `96k`, `64k`, `48k`, `32k`
  
Medio uses the ffmpeg library to recode the audio, ensuring that the final media file matches the user's selected audio quality, even down to `32 kbps` if needed. If the selected audio or video quality isn't available on the source platform, Medio **automatically** selects the **highest available** quality for the one that isn't supported, ensuring the best possible result.

**Note on URL Validation:** While YouTube URL validations are typically processed quickly, validations for other platforms may take a few additional seconds to complete. This is normal and ensures proper compatibility with various sources.

## **Table of Contents**

1. [System Requirements](#system-requirements)
   - [Minimum Requirements](#minimum-requirements)
   - [Recommended Requirements](#recommended-requirements)
2. [Third-Party Libraries](#third-party-libraries)
   - [FFmpeg](#ffmpeg)
   - [yt-dlp](#yt-dlp)
   - [Additional Information](#additional-information)
3. [License Options and Benefits](#license-options-and-benefits)
   - [Premium License](#-premium-license-)
   - [Ultimate License](#-ultimate-license-)
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

Medio leverages several third-party libraries to efficiently process media files and deliver a seamless user experience. The two primary libraries are **FFmpeg** and **yt-dlp**.

### FFmpeg

**FFmpeg** is a robust multimedia framework essential to Medio's functionality. It handles video, audio and other multimedia files and streams, enabling tasks such as format conversion and media encoding/decoding. Medio automatically checks for and installs the latest FFmpeg version to ensure optimal performance and compatibility.

- **Website:** [FFmpeg Official Website](https://ffmpeg.org)
- **License:** FFmpeg is licensed under the LGPL or GPL, depending on the configuration and features used.

### yt-dlp

**yt-dlp** is an open-source command-line tool that enables the downloading of videos from various platforms. Medio integrates yt-dlp to efficiently manage content extraction and downloads, ensuring users can easily access a wide range of sources. This library is automatically updated by Medio to stay compatible with the latest website changes and formats.

- **Website:** [yt-dlp GitHub Repository](https://github.com/yt-dlp/yt-dlp)
- **License:** yt-dlp is licensed under the Unlicense, a public domain equivalent license, allowing free use, distribution, and modification.

### Additional Information

For more details about FFmpeg and yt-dlp, including their capabilities and licensing, refer to their official documentation:

- **FFmpeg Documentation:** [FFmpeg Documentation](https://ffmpeg.org/documentation.html)
- **yt-dlp Documentation:** [yt-dlp Documentation](https://github.com/yt-dlp/yt-dlp#readme)

If you have any questions or issues related to these libraries, please [open an issue](https://github.com/BerndHagen/Medio-Universal-Downloader/issues) on GitHub.

## **License Options and Benefits**

Medio is available for **free**, allowing users to download video and audio files from YouTube in various formats. Premium and Ultimate licenses provide enhanced features and capabilities for a more comprehensive downloading experience. After completing your purchase through Stripe's secure payment gateway, which supports multiple payment methods including credit cards and digital wallets, you will receive an email from Arctisoft-Studio containing your license key and detailed activation instructions within **5-10 minutes**.

### » Premium License «

| **Feature**                     | **Description**                                                        |
|---------------------------------|------------------------------------------------------------------------|
| **Increased Download Speed**    | Experience faster processing with enhanced download speeds             |
| **Extended History**            | Access an expanded download history of up to 50 entries                |
| **Secure Storage**              | Access your download history and account data from any device          |
| **Playlist Downloader**         | Download and process multiple YouTube playlists in batch               |

### » Ultimate License «

| **Feature**                     | **Description**                                                        |
|---------------------------------|------------------------------------------------------------------------|
| **Unlimited Bandwidth**         | Download media files at maximum speeds without any restrictions        |
| **Extended History**            | Access a larger download history, expanded to 100 entries              |
| **Secure Storage**              | Access your download history and account data from any device          |
| **Additional Resolutions**      | Choose from higher video resolutions, including 2160p and 4320p        |
| **Playlist Downloader**         | Download playlists from various video platforms                        |
| **Multi-Platform Support**      | Download from nearly any website with media content                    |

## Data Collection and Account Management

Medio collects account data to enhance your experience and provide seamless synchronization across devices. When you install and launch the application for the first time, an account is automatically created in the database. The data collected includes:

- Personal settings and preferences
- Selected avatar and profile customizations
- Account creation date and activity metrics
- Accumulated experience points and current level
- Total megabytes downloaded
- Total number of audio and video files downloaded
- Comprehensive download history including titles, URLs, and dates
- Number of remaining downloads for trial license users
- Current version status (Basic, Premium, or Ultimate)

## Key Activation and Data Sync

Once a key is purchased and redeemed in the Settings tab under **Key Activation**, it can always be used to retrieve the latest account data from Medio's database. This includes your complete download history, ensuring all your preferences and progress are preserved across sessions and devices when using either a Premium or Ultimate license.

While most account data is backed up and can be restored from the database, certain data, like your **Download History**, is stored locally on your device. **Locally stored data cannot be recovered** if Medio is reinstalled on a different system, which would result in the loss of your Download History.

- Accounts with a **Basic License** will be automatically deleted from the database after **180 days** of inactivity to maintain database efficiency.
- Users with a **Premium** or **Ultimate License** linked to their account are **exempt from this time limit** and can maintain their account indefinitely.

**Note:** Once an account is deleted from the system, it **cannot be restored**. All associated data is permanently removed and cannot be recovered.

## **Free Trial License Key**

Experience selected Premium features with a one-time trial license key. This key provides access to faster download speeds through increased bandwidth, the ability to download YouTube playlists, and expanded history storage of up to 50 entries. The trial is limited to **10** downloads before Premium features are deactivated.

**Unlock Medio's Premium Features:**
```yaml
License Key:     PT4O-5TYD-WKTV-0ZZ7
```

Once the license key has been redeemed, it becomes invalid and can't be used again. After the download limit is reached, the Premium features will no longer be accessible.

## **Getting Started Guide**

Follow these steps to begin downloading content:

### **Step 1: Configure Your Settings**

1. **Open the Settings Menu**
   - Launch **Medio** and navigate to the `Settings` tab.

2. **Set Your Preferences**
   - **Format:** Choose the desired video or audio format for your downloads.
   - **Additional Settings:** Adjust settings like buffer size to suit your needs.

### **Step 2: Download Your Content**

1. **Access the Downloader**
   - Go to the **Downloader** tab in the sidebar.

2. **Select Download Type**
   - Choose whether to download the **video** or extract only the **audio** from your URL.

3. **Enter the URL**
   - Paste the video link into the input field at the top of the **Downloader** page.
   - Note: YouTube URL validations are typically quick, while other platforms may take a few additional seconds to validate.

4. **Configure Download Options**

   - **Save Location:**
     - Click the `...` button next to the directory path field to select your save location.
     - For playlists, it's recommended to create a dedicated folder to keep files organized.
     
   - **File Name:**
     - Enter a custom name in the `Title your Video` field.
     - For playlists, original video titles are used automatically.
     
   - **Select Quality:**
     - Choose your preferred resolution from the available options. If quality isn't your top priority, opting for a lower quality can help reduce the file size.

5. **Initiate the Download**
   - Click the `Start Download` button to begin the process.
   - **Monitor Progress:** Check the progress in the upper-right corner of the app. The `Loading Tools` status means **Medio** is preparing your download, which usually takes a few seconds.

**Medio** processes URLs from various supported platforms. While YouTube links are validated almost instantly, other platforms may require a few additional seconds for validation. If an unrecognized URL is entered, the software will display an `Invalid Link` status. Additionally, if a media file with the same name and format already exists in the specified download path, it will be **automatically skipped** during the download process. If the status changes to `Network Error`, this means the download was interrupted due to a lost Internet connection. To ensure successful downloads, especially when downloading complete playlists, make sure your Internet connection is stable.

## **Download Status Guide**

Throughout the download and conversion process, Medio provides detailed status information to keep you informed about the current operation. These status indicators help you understand exactly what the application is doing at any given moment, from initial preparation to final conversion. The status messages are designed to be clear and informative, helping you track the progress of your downloads and identify any potential issues that may arise.

Below is a comprehensive list of status messages you may encounter while using Medio:

| Status              | Description |
|---------------------|-------------|
| `Loading Tools`     | Initializing download components and preparing resources |
| `Preparing Stream`  | Analyzing media source and configuring download parameters |
| `Invalid Link`      | URL is not recognized or supported |
| `Network Error`     | Connection lost during download or insufficient bandwidth |
| `Premium Required`  | Feature requires Premium license activation |
| `Ultimate Required` | Feature requires Ultimate license activation |
| `Extract Audio`     | Converting video to audio format |
| `Process Stopped`   | Download manually stopped by the user |
| `Converting Format` | Transforming media to selected format |
| `Merging Files`     | Combining audio and video streams |
| `Adding Metadata`   | Embedding title, artist, and other information |
| `Processing Segments` | Handling individual parts of fragmented content |
| `Copyright Error`   | Content is protected by copyright and cannot be downloaded |
| `Completed`         | Download and processing successfully finished |

In rare circumstances, an `Unknown Error` may occur. This status indicates that an unexpected issue has arisen that has not yet been accounted for. If this error persists, please report it in the [GitHub issue section](https://github.com/BerndHagen/Medio-Universal-Downloader/issues), providing details on what you were attempting to download and your selected settings so the issue can be reproduced and addressed.

## **Updating Software**

To ensure Medio continues to perform at its best, it's important to keep it updated. Updates not only introduce new features but also fix bugs that could cause issues, such as incomplete downloads or errors during conversion. Running an outdated version may lead to problems due to outdated files. You can check your current version by locating the Build Number in the bottom left corner of the application, which helps you determine if a newer version is available on the GitHub repository.

To update Medio follow these steps:

1. Download the latest version from the repository and save it to your device.
2. Open the downloaded **ZIP** file and start the setup to begin the installation.
3. Follow the instructions to replace old files with the new updates.
4. Once the installation is complete, launch the application.

Furthermore, make sure the installation path is set to `C:\Users\...\AppData\Local\Arctisoft-Studio\Medio - Universal Downloader`. This prevents any issues and ensures that features aren't blocked due to lack of administrative rights.

## Running Medio on Linux

With the release of **version 1.5.5**, Medio's compatibility with non-Windows operating systems has been significantly improved. While the application remains **primarily** optimized for **Windows**, Linux users can now run Medio through `Wine` with enhanced stability. However, please note that some features might not function exactly as they do on Windows, despite the efforts to ensure cross-platform compatibility. Visual elements like the **Verdana** font are **not natively supported** on Linux, resulting in slightly different font rendering.

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

5. After installation completes, you can run Medio directly through Wine:
```yaml
wine "C:\Program Files\Medio\Medio.exe"
```

If you encounter any technical issues during installation or usage, please visit our [GitHub issues page](https://github.com/BerndHagen/Medio-Universal-Downloader/issues) for support.

## **Hardware Acceleration**

Medio supports advanced hardware acceleration capabilities to optimize video processing performance. This feature uses your system's **GPU** resources for enhanced media handling, resulting in significant **improvements to conversion speeds**. The application automatically detects the best hardware acceleration method through FFmpeg's `-hwaccel auto` parameter, which can utilize technologies like **NVIDIA NVENC, AMD AMF** or **Intel QuickSync** depending on your system's hardware.

### Processing Types and Benefits

1. **CPU Only Processing**
   - Basic processing capability
   - Best suited for lower resolution content
   - Uses standard system resources

2. **GPU Accelerated Processing**
   - Optimal for high-resolution videos (1440p-4320p)
   - Leverages graphics card for enhanced performance
   - Significantly reduces CPU load

3. **Hybrid Processing**
   - Balances workload between CPU and GPU
   - Provides maximum efficiency
   - Automatically adjusts based on content type

### **Performance Specifications**

Hardware acceleration provides several key advantages for media processing:

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

4. **Third-Party Libraries**: Medio leverages third-party libraries like FFmpeg (LGPL) and yt-dlp (Unlicense) for multimedia processing. Please review and comply with their respective licenses.

5. **Warranty Disclaimer**: Medio is provided *"as is,"* without warranties of any kind, express or implied. The Author assumes no liability for damages resulting from the use of the software.

6. **Limitation of Liability**: The Author is not responsible for any indirect, special, incidental, or consequential damages arising out of the use or inability to use the software.

7. **Termination**: The license to use this software may be terminated if the terms of this notice are violated. Upon termination, all use must cease and copies must be deleted.

By using Medio - Universal Downloader, you agree to these terms and conditions. Failure to comply may result in legal action and revocation of your rights to use the software. For full details on licensing terms and further information, please refer to the [LICENSE](https://github.com/BerndHagen/Medio-Universal-Downloader/blob/main/LICENSE) file.

## **Screenshots**

If you'd like a preview of Medio before downloading, the screenshots below offer a clear overview of the application's features. Please note that future updates may introduce additional functionalities.

| Medio - Dashboard Page       | Medio - Downloader Page     | Medio - History Page        |
|------------------------------|-----------------------------|-----------------------------|
| <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.6-medio_dashboard.png" width="300px"> | <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.6-medio_converter.png" width="300px"> | <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.6-medio_history.png" width="300px"> |

| Medio - Premium Page        | Medio - Activation Page     | Medio - Settings Page      |
|-----------------------------|-----------------------------|----------------------------|
| <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.6-medio_premium.png" width="300px"> | <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.6-medio_redeem.png" width="300px"> | <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v1.5.6-medio_settings.png" width="300px"> |

<p align="center">
  <img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_medio.png" alt="Medio Logo" width="128" />
</p>
<h1 align="center">Medio - Universal Downloader</h1>
<p align="center">
  <b>A Windows GUI for yt-dlp and FFmpeg with cloud sync, queue processing, and advanced preprocessing.</b>
</p>
<p align="center">
  <a href="https://github.com/BerndHagen/Medio-Universal-Downloader/releases"><img src="https://img.shields.io/github/v/release/BerndHagen/Medio-Universal-Downloader?include_prereleases&style=flat-square&color=CD853F" alt="Latest Release"></a>&nbsp;&nbsp;<a href="https://github.com/BerndHagen/Medio-Universal-Downloader/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Freemium-red?style=flat-square" alt="License"></a>&nbsp;&nbsp;<a href="https://dotnet.microsoft.com/download/dotnet/10.0/runtime"><img src="https://img.shields.io/badge/.NET-10.0-512BD4?style=flat-square" alt=".NET Version"></a>&nbsp;&nbsp;<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=flat-square" alt="Platform">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Architecture-x64-lightgrey?style=flat-square" alt="Architecture">&nbsp;&nbsp;<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square" alt="Status">&nbsp;&nbsp;<a href="https://github.com/BerndHagen/Medio-Universal-Downloader/issues"><img src="https://img.shields.io/badge/Issues-0_open-orange?style=flat-square" alt="Open Issues"></a>
</p>

**Medio** is a graphical frontend for [yt-dlp](https://github.com/yt-dlp/yt-dlp) and [FFmpeg](https://ffmpeg.org) that wraps these open-source command-line tools in an accessible Windows interface. It handles video downloads, audio extraction, playlist processing, and provides cloud-synced settings, a batch queue, and an audio processing pipeline on top of the core tools.

### **Key Features**

- **Video Downloads:** Download videos in MP4, MKV, AVI, WEBM, WMV, MOV, FLV at resolutions from 144p to 4320p
- **Audio Extraction:** Extract audio as MP3, FLAC, OGG, OPUS, WAV, M4A, AAC, WMA at bitrates from 32k to 320k
- **Playlist Processing:** Batch-download playlists and mixes from supported platforms
- **Queue System:** Sequential automated downloads with configurable concurrency
- **Hardware Acceleration:** GPU encoding via NVIDIA NVENC, AMD AMF, or Intel QuickSync
- **10 Popular Platforms (Basic):** YouTube, Instagram, TikTok, Twitter/X, Facebook, Reddit, Twitch, Vimeo, SoundCloud, Rumble
- **1000+ Platforms (Premium):** All yt-dlp supported platforms
- **Audio Processing (Premium):** Pitch/speed adjustment, reverb, echo, bass boost, 8D audio, vaporwave
- **SponsorBlock (Premium):** Skip or mark sponsored segments in YouTube videos
- **Taskbar Integration:** Real-time progress in the Windows taskbar
- **Cloud Sync:** Settings, statistics, and history sync across devices (cross-device sync is Premium)
- **Privacy Control:** Optionally disable download history tracking

### **Supported Formats**

A wide range of video and audio formats are supported:

- **Video Formats:** `MP4`, `MKV`, `AVI`, `WEBM`, `WMV`, `MOV`, `FLV`
- **Audio Formats:** `MP3`, `FLAC`, `OGG`, `OPUS`, `WAV`, `M4A`, `AAC`, `WMA`

### **Quality Control**

Medio lets you choose from various video and audio quality options:

- **Video Quality Options:** `4320p`, `2160p`, `1440p`, `1080p`, `720p`, `480p`, `360p`, `240p`, `144p`
- **Audio Quality Options:** `320k`, `256k`, `160k`, `128k`, `96k`, `64k`, `48k`, `32k`
  
Medio uses ffmpeg to recode audio, ensuring the final file matches your selected quality down to `32 kbps` if needed. When your selected quality isn't available on the source platform, Medio **automatically** selects the **highest available** quality for the unavailable option.

**Note on URL Validation:** YouTube URLs are validated quickly, while other platforms require a dual-layer validation process combining standard verification with additional media detection, which may take a few extra seconds.

## **Table of Contents**

1. [System Requirements](#system-requirements)
   - [Minimum Requirements](#minimum-requirements)
   - [Recommended Requirements](#recommended-requirements)
2. [Third-Party Libraries](#third-party-libraries)
   - [FFmpeg](#ffmpeg)
   - [yt-dlp](#yt-dlp)
   - [Additional Information](#additional-information)
3. [License Options and Benefits](#license-options-and-benefits)
4. [Privacy and Data Storage](#privacy-and-data-storage)
   - [Cloud-Based Architecture](#cloud-based-architecture)
   - [What Data is Stored](#what-data-is-stored)
   - [Download History Privacy Control](#download-history-privacy-control)
   - [Data Retention and Deletion](#data-retention-and-deletion)
5. [License Key Activation and Profile Synchronization](#license-key-activation-and-profile-synchronization)
6. [Getting Started Guide](#getting-started-guide)
   - [Step 1: Configure Your Settings](#step-1-configure-your-settings)
   - [Step 2: Download Your Content](#step-2-download-your-content)
7. [Advanced Settings](#advanced-settings)
8. [Download Status Guide](#download-status-guide)
   - [Progress Status Messages](#progress-status-messages)
   - [Error Status Messages](#error-status-messages)
9. [Hardware Acceleration](#hardware-acceleration)
    - [Processing Types and Benefits](#processing-types-and-benefits)
10. [Responsible Use](#responsible-use)
11. [Frequently Asked Questions](#frequently-asked-questions)
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

**Note:** Medio is designed exclusively for Windows. While the software may function on Linux through compatibility tools like Bottles, full compatibility is not guaranteed. Visual differences may occur due to missing Windows fonts (e.g., Verdana). The .NET 10.0 Runtime is bundled directly in the installer, allowing Medio to start immediately without requiring separate installation.

## Third-Party Libraries

Medio uses two main third-party libraries to handle media processing and downloads: **FFmpeg** and **yt-dlp**.

### FFmpeg

**FFmpeg** is a multimedia framework that handles video, audio, and other media files. It takes care of format conversion and media encoding/decoding. Medio automatically checks for and installs the latest FFmpeg version to ensure everything works smoothly.

- **Website:** [FFmpeg Official Website](https://ffmpeg.org)
- **License:** FFmpeg is licensed under the LGPL or GPL, depending on the configuration and features used.

### yt-dlp

**yt-dlp** is an open-source command-line tool for downloading videos from various platforms. Medio interfaces with yt-dlp as an external dependency to handle content extraction and downloads from a wide range of sources. Medio does not modify, redistribute, or replace yt-dlp - it simply invokes the tool as a separate process. This library is automatically updated to stay compatible with the latest website changes.

- **Website:** [yt-dlp GitHub Repository](https://github.com/yt-dlp/yt-dlp)
- **License:** yt-dlp is licensed under the Unlicense, allowing free use, distribution, and modification.

### Additional Information

For more details about FFmpeg and yt-dlp, including their capabilities and licensing, check their official documentation:

- **FFmpeg Documentation:** [FFmpeg Documentation](https://ffmpeg.org/documentation.html)
- **yt-dlp Documentation:** [yt-dlp Documentation](https://github.com/yt-dlp/yt-dlp#readme)

If you have questions or issues related to these libraries, please [open an issue](https://github.com/BerndHagen/Medio-Universal-Downloader/issues) on GitHub.

## **License Options and Benefits**

Medio offers two license tiers:

- **Basic (Free):** 10 popular platforms (YouTube, Instagram, TikTok, Twitter/X, Facebook, Reddit, Twitch, Vimeo, SoundCloud, Rumble) with 1440p max resolution, unlimited download speed
- **Premium (€7.99 one-time):** All 1000+ platforms, 4K/8K, audio processing, cross-device sync

License keys are delivered via email within 5-10 minutes after purchase.

| Feature | Basic | Premium |
|---------|:-----:|:-------:|
| **SUPPORTED PLATFORMS** | | |
| YouTube, Instagram, TikTok, Twitter/X, Facebook, Reddit, Twitch, Vimeo, SoundCloud, Rumble | ✔ | ✔ |
| Playlist Support | ✔ | ✔ |
| 1000+ additional platforms | – | ✔ |
| **VIDEO & AUDIO QUALITY** | | |
| Video quality up to 1440p (QHD) | ✔ | ✔ |
| Video quality up to 4K and 8K (4320p) | – | ✔ |
| All audio bitrates (32kbps - 320kbps) | ✔ | ✔ |
| All video formats (MP4, MKV, AVI, WEBM, WMV, MOV, FLV) | ✔ | ✔ |
| All audio formats (MP3, FLAC, OGG, OPUS, WAV, M4A, AAC, WMA) | ✔ | ✔ |
| **DOWNLOAD PERFORMANCE** | | |
| Download speed | Unlimited | Unlimited |
| Simultaneous downloads in queue | Up to 3 | Up to 20 |
| Hardware-accelerated conversion (NVIDIA, AMD, Intel) | ✔ | ✔ |
| **ENCODING OPTIONS** | | |
| Automatic metadata embedding (title, artist, album art) | ✔ | ✔ |
| Audio normalization (5 modes) | ✔ | ✔ |
| Video codec selection (H.264 only / All codecs) | H.264 only | H.264, H.265, VP8, VP9, AV1, MPEG-4 |
| Two-pass encoding for improved quality | – | ✔ |
| **AUDIO PROCESSING** | | |
| Audio pitch adjustment (0.25x - 2.0x) | – | ✔ |
| Audio speed adjustment (0.25x - 2.0x) | – | ✔ |
| Audio enhancement (studio quality processing) | – | ✔ |
| Creative FX (Reverb, Echo, Bass Boost, 8D Audio, Vaporwave) | – | ✔ |
| **ADVANCED FEATURES** | | |
| SponsorBlock ad-skipper for YouTube | – | ✔ |
| Subtitle extraction | ✔ | ✔ |
| Geo-bypass for region-locked content | ✔ | ✔ |
| **CLOUD & PROFILE SYNC** | | |
| Cloud-synced settings | Current device only | All devices |
| Cross-device profile synchronization | – | ✔ |
| Download history | 60 entries (2 pages) | 300 entries (10 pages) |
| Account persistence | Auto-deletion after 365 days inactivity | Permanent |
| **PRICE** | **Free** | **€7.99** (one-time) |

When your history reaches its limit, the **oldest entries are automatically removed** to make room for new downloads. Your most recent downloads are always preserved.

Multiple payment methods are accepted including Card, Klarna, EPS, Bancontact and iDEAL. Since licenses are digital products, refunds are generally **not available** once the key has been delivered. However, if you encounter any issues during the activation process, please don't hesitate to reach out for assistance.

## Privacy and Data Storage

### Cloud-Based Architecture

Medio uses a cloud-first architecture designed for data persistence and seamless synchronization across devices (Premium only). When you first launch the application, a cloud profile is automatically created behind the scenes - no registration, email, or personal information required.

**How It Works:**
- **Automatic Profile Creation:** On first launch, a profile is generated and linked to your device
- **Instant Access:** Each time you launch the application, it automatically connects to your cloud profile and loads your settings
- **Device-Specific (Basic):** Basic license users have their cloud profile tied to their current device only
- **Multi-Device Sync (Premium):** License key holders can access their profile from any device by entering their key

**Why Cloud Storage?**

Since internet connectivity is required for downloads anyway, cloud storage adds valuable benefits without additional overhead:
- **Data Persistence:** Your settings, statistics, and progress are safely stored even if you reinstall Windows
- **Zero Configuration:** No manual backups or exports needed - everything is automatic
- **Cross-Device Sync:** Premium users can seamlessly switch between devices without reconfiguring
- **Gamification:** Track your level, experience points, and ranks persistently

### What Data is Stored

Medio stores the following data in your cloud profile:

**Always Stored (regardless of privacy settings):**
- **Statistics:** Total downloads (video count, audio count), total megabytes processed
- **Progress System:** Experience points (XP), current level, ranks
- **Last Download Title:** Title of your most recent download (for dashboard display)
- **License Status:** Current license type (Basic or Premium)
- **Avatar:** Profile picture if you've uploaded one
- **General Settings:** Buffer size, video/audio format preference, video/audio quality preference
- **Advanced Settings:** Hardware acceleration, download speed limit, download history tracking, audio normalization level, metadata embedding, video codec, video audio codec, two-pass encoding, deinterlace, audio pitch, audio speed, audio enhancement, creative FX, SponsorBlock, geo-bypass, subtitle mode, FFmpeg preset/CRF/threads, concurrent fragments, retries, timeout

**Conditionally Stored (controlled by privacy setting):**
- **Download History:** Complete list of URLs, titles, and dates - only stored when "Track and Save Downloads in History" is **enabled**

**What is NOT Stored:**
- Personal identifying information (name, email, address, phone number)
- Payment details (handled by Stripe, not stored by Medio)
- Downloaded file content (only metadata is tracked)
- Browsing activity outside of Medio
- Device location beyond country-level (used for license management only)

### Download History Privacy Control

You have control over whether Medio tracks detailed download history:

**History Tracking Disabled:**
- New downloads do NOT create history entries
- No URLs or video titles are stored beyond the "last download" field
- The History tab will not populate with new entries
- Statistics (total counts, megabytes) continue to update

**History Tracking Enabled (Default):**
- Each download creates a detailed history entry with URL, title, and timestamp
- View your complete download history in the History tab
- Search and filter past downloads
- Right-click to delete individual entries

**To Disable History Tracking:**
Settings → Advanced → "Track and Save Downloads in History" → Set to **Disabled**

**Note:** Even with history tracking disabled, basic statistics (total downloads, megabytes, XP) are still tracked for the progress system. History tracking specifically controls whether individual download URLs and titles are stored.

### Data Retention and Deletion

**Account Retention:**
- **Basic License:** Inactive accounts (no activity for 365 days) are automatically deleted
- **Premium License:** Accounts are retained indefinitely

**Deleting Your Data:**
- **Individual History Entries:** Right-click any entry in the History tab → Delete
- **Complete Account Deletion:** Navigate to Settings → scroll to "Delete Account" button → confirm twice, or wait 365 days of inactivity for automatic deletion (Basic accounts only)

**What Happens When Deleted:**
- All cloud data is permanently removed
- License keys are not refunded but can be reactivated on a new installation
- Downloaded files on your local device are NOT affected

## License Key Activation and Profile Synchronization

License keys serve two critical purposes: unlocking Premium features and enabling cross-device profile access.

**How Profile Synchronization Works:**

1. **First Device (License Activation):**
   - Enter your license key in the Licenses tab
   - The key permanently links to your current cloud profile
   - All your settings, statistics, history, and progress are now associated with this key

2. **Additional Devices:**
   - Install Medio on a new device (creates a temporary local profile)
   - Go to Licenses tab → Enter the same license key
   - Medio retrieves your existing profile from the cloud, overwriting the temporary local profile
   - All your settings, history, and statistics are now available on the new device

3. **Ongoing Synchronization:**
   - Changes made on any device sync to the cloud automatically
   - Switching between devices always loads your latest profile data
   - Your progress, settings, and history remain consistent across all devices

**Important Notes:**
- **Basic License Limitation:** Basic users cannot sync across devices. If you reinstall Windows or switch computers, you lose access to your profile (automatic deletion after 365 days of inactivity)
- **Premium Benefit:** Your license key is your "passport" to access your profile from any device, anytime
- **Device Security:** License keys can be activated on up to 2 devices simultaneously for security purposes
- **Profile Persistence:** Premium profiles are never automatically deleted - they're retained indefinitely

**What Gets Synchronized:**
- All settings and preferences
- Download statistics (total videos, audios, megabytes)
- Experience points, level, and ranks
- Download history (if tracking is enabled)
- Avatar and customizations

## **Getting Started Guide**

Follow these steps to start downloading content:

### **Step 1: Configure Your Settings**

1. **Open the Settings Menu**
   - Launch **Medio** and go to the `Settings` tab.

2. **Configure Privacy (Optional)**
   - Go to the `Advanced` tab in Settings
   - **Disable History Tracking:** Set "Track and Save Downloads in History" to **Disabled** if you don't want URLs/titles stored
   - **Note:** Statistics (total downloads, MB) are always tracked for the experience system

3. **Set Your Other Preferences**
   - **Format:** Choose your preferred video or audio format for downloads.
   - **Buffer Size:** Adjust buffer settings for optimal performance.
   - **Advanced Settings:** Configure GPU selection, download speed limits, audio normalization, metadata embedding, and codec preferences.

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
     - Click the folder icon (📁) next to the directory path field to select where files are saved.
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

The Advanced Settings panel provides granular control over download and conversion parameters:

**Download Configuration:**
- Quality selection (144p–4320p video, 32k–320k audio) — Basic: up to 1440p, Premium: up to 4K/8K
- Download speed limit (1 MB/s to unlimited)
- Hardware acceleration (NVIDIA NVENC, AMD AMF, Intel QuickSync, CPU-only)
- Network tuning: concurrent fragments (1–16), retries (5–Infinite), timeout (15–300s)
- Buffer size (1024–9216 KB)
- Geo-bypass for region-locked content
- Subtitle extraction (Disabled, English, All Languages)
- Download history tracking toggle

**Encoding Options:**
- Video codec: H.264 (Basic) / H.264, H.265, VP8, VP9, AV1, MPEG-4 (Premium)
- Video audio codec: Auto, AAC, MP3, Opus, Copy
- FFmpeg presets (Ultrafast–Veryslow), CRF quality (18–35 or Auto), thread count
- Two-pass encoding (Premium)
- Deinterlace (Disabled, Auto, Force)
- Metadata embedding (thumbnails, title, artist)
- Audio normalization (5 intensity levels)

**Audio Processing (Premium):**
- Pitch adjustment (0.25x–2.0x)
- Speed adjustment (0.25x–2.0x)
- Audio enhancement (6-stage mastering chain)
- Creative FX (Reverb, Echo, Bass Boost, 8D Audio, Vaporwave)

**Additional:**
- SponsorBlock ad-skipper for YouTube (Premium)

All settings sync automatically across devices for Premium users.

## **Download Status Guide**

Medio displays real-time status information during downloads and conversions.

### Progress Status Messages

| Status                  | Description                                                             |
|-------------------------|-------------------------------------------------------------------------|
| `Scanning`              | Validating and analyzing the provided URL                              |
| `Loading Tools`         | Initializing download components and preparing resources               |
| `Building Command`      | Assembling command arguments for yt-dlp and FFmpeg                     |
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
| `Download Cancelled`    | Download was cancelled before completion                               |
| `Process Stopped`       | Download manually stopped by the user                                  |
| `Completed`             | Download and processing successfully finished                          |

### Error Status Messages

| Status                  | Description                                                             | Solution                                          |
|-------------------------|-------------------------------------------------------------------------|---------------------------------------------------|
| `Empty Link`            | URL field is empty                                                     | Enter a valid video URL                           |
| `Invalid Link`          | URL does not have a recognized format                                  | Check the URL and try again                       |
| `Unsupported Link`      | URL is not supported by yt-dlp                                         | Try a different source or check yt-dlp support    |
| `Network Error`         | Connection lost or insufficient bandwidth                              | Check internet connection and retry               |
| `Content Blocked`       | Platform-side restrictions prevent download                            | Content may be geo-locked or age-restricted       |
| `Copyright Error`       | Platform reports content restrictions                                  | Content is not available for download              |
| `File Exists`           | File already exists in the download directory                          | File is skipped automatically                     |
| `Playlist Error`        | Playlist information could not be gathered                             | Verify the playlist URL is accessible              |
| `Tools Missing`         | yt-dlp or FFmpeg not found                                             | Restart Medio to trigger auto-install              |
| `Premium Required`      | Feature requires Premium license                                       | Activate a Premium license key                    |

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

## **Responsible Use**

Medio is a technical tool designed to provide convenient access to media downloading capabilities. Users must understand and accept their responsibilities when using this software:

**User Responsibilities:**
- **Respect Copyright:** Only download content you have the legal right to access
- **Follow Platform Terms:** Comply with the terms of service of all platforms you download from
- **Age Restrictions:** Verify you meet age requirements for any content you access
- **Local Laws:** Ensure your use of Medio complies with your local jurisdiction's laws

**What Medio Provides:**
- A convenient interface for media downloading tools (yt-dlp, FFmpeg)
- No content filtering or access restrictions (you control what you download)
- Technical functionality without content judgment or monitoring

**What Medio Does NOT Provide:**
- Legal advice or authorization to download copyrighted content
- Circumvention of copyright protection or DRM systems
- Endorsement of any specific platform or content type
- Guarantee of functionality with all platforms (platform changes may affect compatibility)

**Important:** The responsibility for legal compliance rests entirely with you, the user. Medio cannot and does not monitor your download activities or determine what content you are authorized to access. Use this tool responsibly and within the bounds of applicable laws.

If you're unsure whether downloading specific content is legal in your jurisdiction, please consult with a legal professional before proceeding.

## **Frequently Asked Questions**

**Q: Why pay for Medio when yt-dlp and FFmpeg are free?**

A: Medio provides a GUI, cloud sync, queue management, and audio processing on top of yt-dlp/FFmpeg. The Premium tier funds cloud infrastructure and unlocks 1000+ platforms, the audio processing suite, and advanced codec options. The underlying tools remain free and open-source.

**Q: What data does Medio collect?**

A: Settings, statistics (download counts, MB, XP/level), and license status. If history tracking is enabled (default), download URLs and titles are also stored. **No personal identifying information** is collected.

**Q: Why cloud storage instead of local?**

A: Internet connectivity is required for downloads anyway. Cloud storage provides automatic settings backup, persistent progress across reinstalls, and cross-device sync (Premium). You can disable history tracking to minimize stored data.

**Q: Can I use Medio offline?**

A: No. Cloud connectivity is required for profile management. You can disable history tracking to minimize data collection.

**Q: Is it legal to download videos from YouTube?**

A: YouTube's Terms of Service may restrict downloading. Medio is a technical tool — legal responsibility rests with you.

**Q: What happens if I disable history tracking after using it?**

A: New downloads will no longer create history entries. Your existing cloud-stored history remains accessible in the app until you delete individual entries or your account is removed due to inactivity (365 days for Basic accounts).

**Q: Can I transfer my license?**

A: No. License keys are non-transferable and support up to 2 simultaneous device activations. Keys showing suspicious sharing patterns (e.g., activations from multiple countries) may be flagged or deactivated.

**Q: How do I completely delete all my data?**

A: Delete individual history entries via right-click in the History tab. For complete account deletion:
- Navigate to Settings → scroll to "Delete Account" button → confirm twice
- **Basic accounts:** Alternatively, wait 365 days of inactivity for automatic deletion
- **Premium accounts:** Can also use the Delete Account button or contact support via GitHub issue tracker

Your license key remains valid after account deletion and can be used to create a fresh profile on any device.

**Q: What happens to my data if my account is deleted?**

A: Only cloud data (settings, history) is removed. Downloaded files on your device are never affected. License keys remain valid and can be reactivated on a new install.

**Q: What if I reinstall Windows or switch computers (Basic)?**

A: Basic users lose access to their cloud profile on device change. The profile is auto-deleted after 365 days of inactivity. Premium license keys allow retrieving your profile from any device.

**Q: Can I use my license key on multiple devices?**

A: Yes. Enter the same key on a new device to sync your settings, statistics, and history. A maximum of 2 devices can be registered simultaneously — adding a third device automatically removes the oldest one. Basic licenses don't support cross-device sync.

## **Screenshots**

If you'd like a preview of Medio before downloading, the screenshots below show the application's features. Note that future updates may introduce additional functionality.

<table>
  <tr>
    <th>Medio - Dashboard</th>
    <th>Medio - Downloader</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_dashboard.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_dashboard.png" alt="Medio Dashboard" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_downloader.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_downloader.png" alt="Medio Downloader" width="450"></a></td>
  </tr>
  <tr>
    <th>Medio - History</th>
    <th>Medio - Licenses</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_history.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_history.png" alt="Medio History" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_licenses.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_licenses.png" alt="Medio Licenses" width="450"></a></td>
  </tr>
  <tr>
    <th>Medio - Activation</th>
    <th>Medio - Settings</th>
  </tr>
  <tr>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_activation.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_activation.png" alt="Medio Activation" width="450"></a></td>
    <td><a href="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_settings.png" target="_blank" rel="noopener noreferrer"><img src="https://github.com/BerndHagen/Medio-Universal-Downloader/raw/main/img/img_v2.0.3-medio_settings.png" alt="Medio Settings" width="450"></a></td>
  </tr>
</table>

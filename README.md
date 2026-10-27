# FreeConvert_Universel_Grandiose
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gsmagrandi-svg/FreeConvert_Universel_Grandiose/blob/main/FreeConvert_Universel_Grandiose.ipynb)

A universal, all-in-one file converter built with Gradio and Google Colab.
 

FreeConvert_Universel_Grandiose is an open-source, browser-based file conversion tool that supports over 1,500 file conversions across multiple categories: video, audio, images, documents, ebooks, and archives. It automatically detects the uploaded file type, dynamically suggests the best output formats and advanced options (resolution, bitrate, quality), and provides real-time progress feedback with clear, step-by-step instructions.

Whether you need to convert an MP4 to MP3, a DOCX to PDF, a PNG to WEBP, or an EPUB to MOBI, this tool handles it all in one intuitive interface.

✨ Key Features
🔍 Smart Auto-Detection : Automatically identifies the file category and proposes valid output formats and options.

🎛️ Dynamic Options : Offers tailored settings for each format (e.g., 1080p/720p/480p for video, 320/192/128 kbps for audio, DPI for images).

📊 Real-Time Progress : Interactive progress bars with clear status messages for every conversion step.

🛑 Cancellation Support : Stop any conversion mid-process with a dedicated "Stop" button.

💾 Dual Save Modes : Download directly to your PC or save to a designated folder in your Google Drive.

🌐 Cross-Platform : Runs on Windows, macOS, Linux, and mobile devices via any modern web browser.

🎨 Professional UI : Clean, modern Gradio interface with custom CSS styling and a "Grandiose" look.

🛠️ Modular Architecture : Each conversion type is handled by a dedicated function, making it easy to extend and maintain.

🛠️ Technology Stack
Category	Tool / Library
Video & Audio	FFmpeg
Documents	LibreOffice, WeasyPrint
Ebooks	Calibre
Images	Pillow, ImageMagick
Archives	Python standard library (zipfile, tarfile)
Web Interface	Gradio
Environment	Google Colab (with Google Drive integration)
📂 Supported Formats (Examples)
Video : MP4, MKV, AVI, MOV, WEBM, FLV, WMV, M4V

Audio : MP3, WAV, FLAC, AAC, OGG, M4A, WMA

Images : PNG, JPG, JPEG, BMP, WEBP, TIFF, HEIC, SVG

Documents : DOCX, DOC, PPTX, PPT, XLSX, XLS, ODT, TXT, MD, HTML, XML, PY, JS, CSS

Ebooks : EPUB, MOBI, AZW3, FB2, LIT

Archives : ZIP, RAR, 7Z, TAR, GZ

🚀 How to Use
Open the notebook in Google Colab.

Run Cell 2 to mount Google Drive, install system tools (FFmpeg, LibreOffice, Calibre, ImageMagick), and set up Python dependencies.

Run Cells 3 to 7 to load the format dictionary, utility functions, and conversion functions.

Run Cell 7.5 to verify that all components are properly loaded and all system tools are available.

Run Cell 8 to launch the Gradio interface. Click the public link (https://xxxxx.gradio.live) to open the app.

Upload a file, choose the output format and options, select your save location (PC or Google Drive), and click "Lancer la Conversion".

Download the converted file or find it in your Google Drive folder: /content/drive/MyDrive/FreeConvert_Universel_Grandiose/.

📁 Project Structure
text
FreeConvert_Universel_Grandiose/
│
├── FreeConvert_Universel_Grandiose.ipynb   # Main notebook
├── README.md                               # This file
└── (converted files saved here)            # Output directory on Google Drive
⚠️ Important Notes
First Run : The initial setup (installing FFmpeg, LibreOffice, Calibre, ImageMagick) may take several minutes. Subsequent runs are faster thanks to Colab's cache.

Cancellation : The stop button is checked before and after each conversion subprocess. For very large files, cancellation may take a few seconds to take effect.

Session Persistence : Google Colab sessions are ephemeral. After a runtime restart, you must re-execute all cells (2 → 3 → 4 → 5 → 6 → 7 → 7.5 → 8) to reload the environment.

Google Drive Path : Converted files saved to Drive are stored in /content/drive/MyDrive/FreeConvert_Universel_Grandiose/.

🔮 Future Improvements
Add support for more formats (e.g., pandoc for advanced document conversion, HandBrake for video presets).

Integrate direct cloud storage providers (Dropbox, OneDrive) via OAuth.

Deploy as a permanent web app on Hugging Face Spaces.

Add batch conversion support (multiple files at once).

Implement a file history and conversion log.

📄 License
This project is open-source and available under the MIT License. Feel free to use, modify, and distribute it as you see fit.

🙏 Acknowledgements
Gradio for the intuitive web interface.

FFmpeg, LibreOffice, Calibre, and ImageMagick for their powerful conversion engines.

Google Colab for providing a free, accessible development environment.

Made with ❤️ for the open-source community.


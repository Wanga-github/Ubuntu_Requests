# Ubuntu Image Fetcher

A Python tool that downloads images from URLs and organizes them locally. Built with the Ubuntu philosophy of community, respect, sharing, and practicality.

## Features

- Downloads images from direct URLs or HTML pages
- Automatically extracts images from web pages (Unsplash, etc.)
- Creates organized directory structure
- Handles errors gracefully
- Auto-detects correct file extensions

## Requirements

- Python 3.6+
- requests library

## Installation

Install dependencies:
```bash
pip install requests
```

Optional - make executable on Linux/macOS:
```bash
chmod +x ubuntu_image_fetcher.py
```

## Usage

Run the script:
```bash
python3 ubuntu_image_fetcher.py
```

Or on Linux/macOS if executable:
```bash
./ubuntu_image_fetcher.py
```

Enter an image URL when prompted. The script will download it to the `Fetched_Images/` directory.

## Supported URLs

- Direct image URLs: `https://example.com/image.jpg`
- Unsplash photo pages: `https://unsplash.com/photos/photo-id`
- Any page with Open Graph or Twitter card images

## Troubleshooting

**403 Forbidden Error**
Try using the direct image URL instead of the page URL. Right-click the image and select "Copy Image Address".

**Connection Timeout**
Check your internet connection and try again.

**Image Not Found**
Verify the URL is correct and the image exists.

## How It Works

The script sends proper browser headers to avoid being blocked, detects whether a URL is an image or HTML page, extracts the actual image URL if needed, and downloads the image with appropriate error handling.

## License

Open source and available for educational and personal use.

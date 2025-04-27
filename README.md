# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps

## OUTPUT:
Extracted Metadata, Timeline Events, and Hidden Data Detection Results

## ✅ A. Using ExifTool – for file metadata

## 📦 Install:

sudo apt update
sudo apt install exiftool -y

## 📂 Extract metadata from a file:

exiftool image.jpg

## 📁 Batch process a folder:

exiftool -r /path/to/folder

## 📌 Useful flags:
-G: Show metadata group

-time:all: Show only timestamps

-GPSLatitude -GPSLongitude: Extract GPS data

![image](https://github.com/user-attachments/assets/42916ff2-a4d6-469c-8805-b6e360aab17d)

## install log2timeline

sudo apt install plaso -y

sudo apt install steghide -y

Embed data

steghide embed -cf /home/kali/Downloads/wallpaper.jpg -ef /home/kali/Downloads/secret.txt

![image](https://github.com/user-attachments/assets/e5244d76-6acc-4a25-84ef-a080433319ad)

Extract hidden data:

steghide extract -sf hidden.jpg

![image](https://github.com/user-attachments/assets/dc045712-2109-4ac2-9d01-1594b3a237ee)

## Using binwalk – for file analysis

sudo apt install binwalk -y

binwalk suspicious.jpg

binwalk /home/kali/Downloads/wallpaper.jpg

![image](https://github.com/user-attachments/assets/dba743ad-ba4a-4019-85c8-4dacb5b5dce7)



## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.


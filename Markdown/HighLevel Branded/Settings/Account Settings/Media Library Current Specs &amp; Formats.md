**Date Updated:** 2025-07-29T01:29:04.000Z

The Media Library stores assets like images and videos. Different products have different limitations on the files that can be used in them.

---

**TABLE OF CONTENTS**

* [What is a File and Why a Media Library?](#What-is-a-File-and-Why-a-Media-Library?)  
   * [Media Library Details](#Media-Library-Details)  
   * [Per-product File Limits](#Per-product-File-Limits)

---

# **What is a File and Why a Media Library?**

  
Files are data sets that are formatted in a special way and given a specific file extension (ex: **.png or .pdf or .txt**). Any product that can use a file will have a limit on the **types** of files it knows how to read and the **size** of the files it can read.

  
A webpage builder might know how to use a .png file but not an .svg and it might be able to process a 1MB file but not a 1GB file. The file extension is usually easy to see, but the file size is sometimes hard to see.

  
Additionally, even if the product can incorporate the file, there might be design reasons to limit the file's **display size**. For example, a logo displayed at 50px by 200px fits into a header well, but a logo displayed at 500px by 500px is way too big. 

  
On top of that, the file's native resolution might not be a good fit for the display size, like if the file is only 16px by 16px (an icon) and the webpage is trying to display it at 500px by 500px. It will look very pixelated, not sharp. Unless it's a .svg, in which case it doesn't have a native resolution (because it's drawn with math instead of pixels) so it can be displayed at any size.

  
As if that wasn't enough, when a file is displayed its dimensions might not be a perfect fit for the area it's put into. In that case there are style options to make it justified left, right, or center, and there are settings to address the whitespace like stretching it, tiling it, cropping it, etc. These are not part of the file itself, they're style settings that modify how the file is displayed, but different file details work better with different display options. 

  
This is why HighLevel has a Media Library; once you start managing file assets you have to deal with a significant amount of complexity. 

---

## **Media Library Details**

  
Get to the Media Library and preview files by navigating to **Media Storage > Folder/File**.

  
* **Filename**: This is the string that identifies the file. This has to be different from all other filenames.
* **File Extension**: This is the shorter string at the end of the filename (ex: .png). This identifies how the data is encoded so that products can read the file.
* **Publication Date**: The date the file was added to the Media Library.
* **File Size**: This is how much memory the file takes up. You will often see kb (kilobytes), mb (megabytes, and gb (gigabytes). Each is a thousand (1,000x) times bigger than the last.
* **Dimensions**: This is the number of pixels high and wide the file is natively. This tells you how much of the screen the file will take up if you don't squish or stretch it.

  
![](https://s3.amazonaws.com/cdn.freshdesk.com/data/helpdesk/attachments/production/155049689085/original/6APZtw8HUlC4A5PJp14VPaXlVf7QqpRaHQ.png?1752198820)

---

## **Per-product File Limits**

  
Files can be uploaded through Forms by creating a Custom Value of type File Upload.

  
| File Type                                                                                                                                                                      | Media Library | Social Planner | Sites & Funnels | Courses | CV File Upload |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------- | -------------- | --------------- | ------- | -------------- |
| **Images**                                                                                                                                                                     |               |                |                 |         |                |
| PNG (.png)                                                                                                                                                                     | 100MB         | 10MB           | 100MB           | 50MB    | 50MB           |
| JPEG (.jpg, .jpeg, .jfif, .pjpeg, .pjp)                                                                                                                                        | 100MB         | 10MB           | 100MB           | 50MB    | 50MB           |
| GIF (.gif)                                                                                                                                                                     | 100MB         | 10MB           | 100MB           | 50MB    | 50MB           |
| TIFF (.tif, .tiff, x-tiff)                                                                                                                                                     | 100MB         | 10MB           | 100MB           | 50MB    | 50MB           |
| WEBP (.webp)                                                                                                                                                                   | 100MB         | 10MB           | 100MB           | 50MB    | 50MB           |
| SVG (.svg)                                                                                                                                                                     | 100MB         | 10MB           | 100MB           | 50MB    | 50MB           |
| ICON (.ico, .cur, x-icon)                                                                                                                                                      | 100MB         | 10MB           | 100MB           | 50MB    | 50MB           |
| **Videos**                                                                                                                                                                     |               |                |                 |         |                |
| AVI (.avi, x-troff-msvideo)                                                                                                                                                    | 4GB           | 1GB            | 4GB             | 5GB     | 50MB           |
| QuickTime (.qt, .qtc, .mov, .moov, .moov)                                                                                                                                      | 4GB           | 1GB            | 4GB             | 5GB     | 50MB           |
| MP4 (.mp4)                                                                                                                                                                     | 4GB           | 1GB            | 4GB             | 5GB     | 50MB           |
| MPEG (.mpg)                                                                                                                                                                    | 4GB           | 1GB            | 4GB             | 5GB     | 50MB           |
| Ogg Video (.ogv)                                                                                                                                                               | 4GB           | 1GB            | 4GB             | 5GB     | 50MB           |
| Windows Media (.wmv, .asf)                                                                                                                                                     | 4GB           | 1GB            | 4GB             | 5GB     | 50MB           |
| WebM (.webm)                                                                                                                                                                   | 4GB           | 1GB            | 4GB             | 5GB     | 50MB           |
| **Audio**                                                                                                                                                                      |               |                |                 |         |                |
| AIF (.aif, .aiff, .aifc)                                                                                                                                                       | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| MIDI (.midi, .mid)                                                                                                                                                             | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Windows Audio (.wav)                                                                                                                                                           | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Ogg Audio (.oga)                                                                                                                                                               | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| WebM Audio (.weba)                                                                                                                                                             | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| MPEG (.mpeg)                                                                                                                                                                   | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| m4a (.m4a)                                                                                                                                                                     | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| **Application**                                                                                                                                                                |               |                |                 |         |                |
| PDF (.pdf)                                                                                                                                                                     | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Word (.doc, .docx, ms-doc, msword, vnd.openxmlformats-officedocument.wordprocessingml.document)                                                                                | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Excel (excel, .xls, xlsx, .xlsm, vnd.ms-excel, x-excel, x-msexcel, vnd.openxmlformats-officedocument.spreadsheetml.sheet)                                                      | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| PowerPoint (.ppt, .pptx. .pptm, mspowerpoint, powerpoint, vnd.ms-powerpoint, x-mspowerpoint, vnd.ms-powerpoint, vnd.openxmlformats-officedocument.presentationml.presentation) | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Apple Numbers (x-iwork-numbers-sffnumbers,                                                                                                                                     | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Google Sheet (vnd.google-apps.spreadsheet)                                                                                                                                     | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Google Doc (vnd.google-apps.document)                                                                                                                                          | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Google Slides (vnd.google-apps.presentation)                                                                                                                                   | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Text (.rtf, .txt)                                                                                                                                                              | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| ZIP (.zip, x-zip, z-zip-compressed, x-compress, x-compressed                                                                                                                   | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| CSV (.csv)                                                                                                                                                                     | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| **Font**                                                                                                                                                                       |               |                |                 |         |                |
| TrueType TTF (.ttf)                                                                                                                                                            | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| OpenType OTF (.otf)                                                                                                                                                            | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| Web Open Font Format WOFF, WOFF2 (.woff)                                                                                                                                       | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |
| **Contact**                                                                                                                                                                    |               |                |                 |         |                |
| vCard (.vcf)                                                                                                                                                                   | 100MB         | 100MB          | 100MB           | 50MB    | 50MB           |

  
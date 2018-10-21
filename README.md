# WordPress-Pen-Testing-Lab

# Exploit 1
WordPress 3.6.0-4.7.2 - Authenticated Cross-Site Scripting (XSS) via Media File Metadata (CVE-2017-6814)
To exploit this vulnerability, I used the following steps:
  1. Download an arbitrary MP3 file. (I prefer something by Rick Astley)
  2. In order to make our newly downloaded file malicious, we must edit the metadata of the file.
  3. I used the software 'kid3' to change the title of the song in the file metadata to include my XSS code.
  4. Log into the vicitm WordPress page and upload this malicious file.
  5. Once the file is uploaded, all it takes is viewing file to execute the XSS.
  ![](Exploit1.gif)

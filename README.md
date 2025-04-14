# CTF Tools and Usage Reference

This document includes commonly used tools and their basic usage in Capture The Flag (CTF) competitions. 

---

## Reverse Engineering

### **apktool**

- Decompile Android APK files.

```
apktool d app.apk
```

### **dnSpy**

- Analyze .NET binaries.
- Usage: Load EXE or DLL files to reverse engineer source code.

---

## Binary / General Analysis

### **xxd / hexedit**

- View files in hexadecimal format.

```
xxd file.gif | grep "21 FE"
```

### **strings**

- Extracts readable strings from files.

```
strings file.png | grep -i flag
```

### **file**

- Analyzes the file type.

```
file file.abc
```

### **grep**

- Extracts specific patterns from files.

```
grep -aE "flag\{.*\}" file.png
```

---

## Steganography / Forensics

### **steghide**

- For steganography (hiding/extracting data within files).

```
steghide extract -sf file.jpg
```

### **binwalk**

- Scans files for embedded data.

```
binwalk -e file.gif
```

### **exiftool**

- View metadata of a file.

```
exiftool file.jpg
```

### **identify (ImageMagick)**

- Displays detailed image file information.

```
identify -verbose image.gif
```

---

## Multimedia Analysis

### **sonic visualizer**

- GUI-based program to generate spectrograms of audio files.

### **ffmpeg**

- Convert and analyze video/audio files.

```
ffmpeg -i video.mp4
```

```
ffmpeg -i input.mp4 -c copy -bsf:v noise output.mp4
```

---

## Hashing

### **md5sum**

- Calculates the MD5 hash value for a file.

```
md5sum file.mp4
```

---

## Compression / Extraction

### **unzip**

- Extracts ZIP compressed files.

```
unzip file.xyz
```

---

## Online Tools

### **dcode.fr**

- Web-based cipher decoder.
- URL: [https://www.dcode.fr](https://www.dcode.fr)

### **morscode.world**

- Web-based Morse code translator.
- URL: [https://morscode.world](https://morscode.world)

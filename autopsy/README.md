# Ex No. 06 – Use Sleuth Kit to Analyze Digital Evidence

## Aim
To use The Sleuth Kit (TSK) command-line tools to analyze a disk image and recover digital evidence.

## Procedure
Sleuth Kit is used in digital forensics to analyze disk images and recover crucial evidence. It allows the examination of file systems, listing of files and partitions, recovery of deleted files, extraction of metadata, and timeline analysis to understand file activity. Findings can be compiled into a digital forensic report for secure storage.

## Step 1: Install Sleuth Kit
### Download Sleuth Kit
- Visit the official Sleuth Kit website or a provided Google Drive link.
- Download the latest version compatible with Windows.

### Install Sleuth Kit
- Run the downloaded installer.
- Follow the on-screen instructions to complete installation.

## Step 2: Acquire the Disk Image
A disk image is required before analysis. This can be a copy of a hard disk, pen drive, memory card, etc.

### Create Disk Image
Use a tool like FTK Imager or dd to create a bit-by-bit copy of the storage device.

Supported formats:
- .dd
- .raw
- .img
- .E01

### Example Evidence Files
- 4Dell Latitude CPi.E01
- 4Dell Latitude CPi.E02
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4a8b9abf-8ccf-47e7-a967-abc493c7f61e" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c04e373e-391b-4f3b-864a-55c5e7c0f1ff" />

## Step 3: Mount the Disk Image (Optional)
Mounting helps in navigating the file system manually.

### Mount Using OSFMount
- Use OSFMount to mount the .E01 image as a virtual drive.

## Step 4: Analyze the File System Using Sleuth Kit
Open Command Prompt and navigate to the Sleuth Kit installation folder.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/477f7ead-8edf-4f77-b9f1-e1fb76c83cd0" />

```<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4915d425-61e6-459f-94cf-e67a1a224351" />

### Identify File System Type – fsstat
```
fsstat "4Dell Latitude CPi.E01" > filesystem_info.txt
```

### List Partitions – mmls
```
mmls "4Dell Latitude CPi.E01" > partitions.txt

### List All Files – fls
```
fls -r "4Dell Latitude CPi.E01" > file_list.txt
```

### Recover Deleted Files – icat
```
icat "4Dell Latitude CPi.E01" [inode number] > [output file]
```

## Step 5: Analyze File Metadata
### View Metadata – istat
```
istat "4Dell Latitude CPi.E01" [inode number] > metadata_info.txt
```

## Step 6: Timeline Analysis (Optional)
### Generate Body File
```
fls -m / -r "4Dell Latitude CPi.E01" > body.txt
```

### Create Timeline – mactime
```
mactime -b body.txt > timeline.txt
```

## Result
Using The Sleuth Kit on Windows, you can examine disk images, retrieve file information, recover deleted files, extract metadata, and create activity timelines—helping to analyze and preserve digital evidence effectively.

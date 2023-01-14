# 👋Welcome to Container File👋
Container File is a project developed to host all files in a single file. To avoid file clutter, your files are stored in a single file in an "**uncompressed**" format.

## 🤔Why are files stored without compression?🤨
It is planned to avoid the long waiting times that large files spend on compression and extraction.

## 😎How will the files be stored in a single file?🧐
The container file is actually an xml file. The file structure is specified as follows.
```xml
<?xml version="1.0"?>
<ContainerFile xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
	<FileNames>
		<string>File Name.ext</string>
		<string>Filename without extension</string>
	</FileNames>
	<FileBytes>
		<base64Binary>...</base64Binary>
		<base64Binary>...</base64Binary>
	</FileBytes>
</ContainerFile>
```

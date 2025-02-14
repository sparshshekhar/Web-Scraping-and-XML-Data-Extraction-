# Web Scraping XML Data with Python 

## Introduction  
This project is a simple Python script that extracts and processes XML data using the `xml.etree.ElementTree` module. It parses XML content containing metadata about stored files and extracts key details such as filenames, last modified timestamps, sizes, and storage classes.  

## Features 
- Parses XML data efficiently using Python's `ElementTree`.  
- Extracts important metadata from XML files, including:  
  - **File name** (`Key`)  
  - **Last modified timestamp** (`LastModified`)  
  - **File size** (`Size`)  
  - **Storage class** (`StorageClass`)  
- Can be extended to process real-time XML feeds.  

## Requirements  
- Python 3.10 or above  

## Code Structure  

### 1. web_scrapping.py  
This script contains the logic for parsing XML data and extracting required information.  

#### Implementation Details:  
- Loads XML data into memory.  
- Parses and extracts relevant file details using `ElementTree`.  
- Prints extracted data in a readable format.  

### Example XML Input:  
```xml
<Root>
    <Contents>
        <Key>example-file.jpg</Key>
        <LastModified>2023-01-01T12:00:00.000Z</LastModified>
        <Size>12345</Size>
        <StorageClass>STANDARD</StorageClass>
    </Contents>
</Root>
```  

### Extracted Output Format:  
```
Filename: example-file.jpg  
Last Modified: 2023-01-01T12:00:00.000Z  
Size: 12345 bytes  
Storage Class: STANDARD  
```  

## Setup Instruction  

### 1. Clone the Repository  
```bash
git clone https://github.com/yourusername/web-scraping-xml.git  
cd web-scraping-xml
```

### 2. Run the Script  
```bash
python web_scrapping.py
```

## Future Improvements  
- Extend script to fetch XML from live APIs.  
- Store extracted data in a database or CSV file.  
- Implement error handling for missing or malformed XML elements.  

## Conclusion  
This project demonstrates XML data parsing in Python, extracting essential metadata for further processing. The script can be enhanced for real-world applications, such as automated file tracking and data analysis.  

---

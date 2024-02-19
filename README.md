Iannis Bardakos 2018

# Zotero Storage PDF Management Tool

## Overview
This tool is designed to streamline the management of PDF files like the ones in a Zotero Reference manager storage directories. It focuses on flattening the directory hierarchy by moving all PDFs to the root folder, identifying and removing duplicate files, and maintaining a clean, organized structure. The utility embodies a minimalist approach, leveraging Python's capabilities for file manipulation and employing a simple graphical user interface for user interactions.

## Features
- PDF Hierarchy Flattening: Transforms nested folder structures by moving all PDFs to the specified root folder, thereby simplifying access and management.
- Duplicate Detection and Removal: Employs SHA-1 hashing to identify duplicate files, considering both file size and content, with a preference for retaining files with more recent modification timestamps or shorter names.
- Graphical User Interface: Offers a straightforward interface for selecting directories and executing the flattening process, enhancing user experience.

## Prerequisites
- Python 3.x: Ensure Python 3 and above is installed on your system.
- Tkinter: The GUI framework, typically included with Python installations.

## Usage
1. Clone or download the repository to your local system.
2. Navigate to the directory containing the script.
3. Launch the script using a Python interpreter:
    ```bash
    python3 zotero_pdf_manager.py
    ```
4. Use the GUI to select the root folder where PDF files are stored. The script will then flatten the hierarchy and clean duplicates within this directory.

## Technical Insights
- The tool traverses directory structures recursively, identifying PDF files based on their extensions.
- Flattening involves moving files to the root directory and removing empty subdirectories.
- Duplicate detection is a two-step process: a preliminary check using a hash of the first 1KB of each file to quickly identify potential duplicates, followed by a full file hash comparison for confirmation.

## Contributing
Contributions to enhance functionality or improve efficiency are welcome. Please adhere to standard coding practices and document changes adequately.

## License
This project is open-source, available under [GNU General Public License v3.0], promoting free information and expression in alignment with anti-capitalist and communal principles.

## Acknowledgements
Gratitude to the global community of developers and researchers, whose collaborative spirit and shared knowledge make such tools possible.

---

This README aims to encapsulate the essence and functionality of your tool while reflecting the values and principles you uphold, Dr. Bardakos.

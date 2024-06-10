# Smart-Files
# Smart Files Documentation

## Overview
Smart Files is a Python application that simplifies file management through a graphical user interface (GUI) built with Tkinter. The tool provides functionalities to browse directories, rename files based on their type and timestamp, organize files into folders by their extensions, and compress files older than a specified age. The application leverages batch scripts and PowerShell commands to perform these operations.

## Features
- **Browse Directory**: Select a directory for file operations.
- **Rename Files**: Automatically rename files based on their type and timestamp.
- **Organize Files**: Sort files into folders by their extensions.
- **Compress Files**: Compress files older than a specified age into a zip archive.

## Usage
1. Run the `Smart Files` executable.
2. Use the GUI to select the desired directory and operation.

### GUI Components
- **Main Frame**: Allows directory selection and navigation to different functionalities.
- **Options Frame**: Presents the choices to rename, organize, or compress files.
- **Rename Files Frame**: Enables file renaming based on predefined rules.
- **Organize Files Frame**: Facilitates sorting files into folders by extension.
- **Compress Files Frame**: Compresses old files into a zip archive.

### Directory Browsing
- **Browse Button**: Opens a file dialog to select a directory.
- **Directory Entry**: Displays the selected directory path with placeholder text support.

### Renaming Files
Files are renamed based on their type with a timestamp appended. Supported file types include:
- Images (png, jpg, jpeg, gif)
- PDFs
- Documents (doc, docx, etc.)
- Spreadsheets (xls, xlsx, etc.)
- Presentations (ppt, pptx, etc.)
- Text files (txt, ini, cfg, etc.)
- Audio files (mp3, wav, etc.)
- Video files (mp4, mov, etc.)

### Organizing Files
Files are moved into folders named after their extensions, excluding certain script and batch files to prevent conflicts.

### Compressing Files
Files older than a specified number of days are moved to an "Old Files" folder, compressed into a zip archive, and the folder is deleted after compression.

## Code Overview
The application is structured into several key functions:

- **browse_directory**: Opens a directory selection dialog.
- **on_focus_in**: Clears placeholder text when the entry gains focus.
- **on_focus_out**: Restores placeholder text if the entry is empty.
- **show_options_frame**: Displays the options frame for further actions.
- **draw_gradient**: Draws a gradient background on a canvas.
- **show_main_frame**: Returns to the main frame.
- **show_next_section**: Navigates to the selected operation frame.
- **Rename_Excute**: Executes the batch script for renaming files.
- **Orginize_Excute**: Executes the batch script for organizing files.
- **Compress_Excute**: Executes PowerShell commands to compress old files.
- **Run_command**: Determines which operation to run based on the selected option.

## Running the Application
To run the application, execute the compiled executable (.exe).


## GUI Navigation
- **Main Frame**: Browse directory and navigate to options.
- **Options Frame**: Choose to rename, organize, or compress files.
- **Rename Files Frame**: Apply renaming rules to the selected directory.
- **Organize Files Frame**: Sort files into extension-based folders.
- **Compress Files Frame**: Compress old files in the selected directory.

## Error Handling
Output labels in each operation frame display success or error messages based on the operation's result.

## Conclusion
Smart Files offers an intuitive GUI for managing file operations, enhancing productivity and organization. Follow the usage instructions to utilize its capabilities effectively. For any issues or contributions, refer to the GitHub repository.

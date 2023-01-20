# PPTX VT Remover
This is a Python script that can remove vertical tab-line tabulation from PPTX files. The script iterates through each slide in the PPTX file and checks for VT, and when found either replaces it with a space (if none is found before or after) or deletes it (if a space is found before or after).

## Requirements
- Python 3 installed on your system
- python-pptx library installed. You can install it using pip by running the command: 
```bash
pip install python-pptx==0.6.18
```
- The PPTX file that you want to remove VT from should be accessible on your system and you should have the correct path to it 
- The script should have write access to the directory where you want to save the log file and the modified PPTX file

## How to use

- Clone the repository to your local machine
- Navigate to the cloned folder 
- Run the script by providing the path of the PPTX file as an argument:
```bash
python pptx_vt_remover.py path/to/pptx/file
```
- The script will create a log file called "removed_vts.txt" in the same directory as the script, which will contain the logs of all the VTs removed, including the slide and the text where it was removed.

Please note that it is always a good practice to create and use virtual environment to avoid any library version conflicts with the other existing projects.

- If you have an empty file now in your folder called removed_vts.txt and its empty, it means that there were no VTs found in the PPTX file that you provided. Make sure that you have provided the correct path to the file and that you have the read permissions for the file.

This readme gives an overview of the project, the requirements, and how to use it. It also includes a troubleshooting section to help users with common issues they might face while using the script. The script is well commented so that you can understand the logic behind the code.
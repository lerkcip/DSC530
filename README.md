# DSC530

How to Uncompress Files After Downloading
After downloading the compressed file from this repository, follow the instructions below to uncompress it on your system.

For Windows Users:
Using the Built-in Extract Tool:

Locate the downloaded compressed file (e.g., city_market_tracker.zip).
Right-click on the file and select "Extract All..." from the context menu.
Choose the destination folder where you want to extract the files.
Click "Extract" to uncompress the file.
Using a Script (Optional):

Download the uncompress.bat script from the repository.
Place the script in the same directory as the compressed file.
Double-click uncompress.bat to automatically uncompress the file.
uncompress.bat:

batch
Copy code
@echo off
echo Uncompressing the file...

REM Uncompress the file (for .zip files)
powershell -Command "Expand-Archive -Path city_market_tracker.zip -DestinationPath ."

REM For .tar.gz files, you would use:
REM tar -xvzf city_market_tracker.tar.gz

echo Uncompression complete.
pause
For macOS Users:
Using the Built-in Archive Utility:

Locate the downloaded compressed file (e.g., city_market_tracker.zip).
Double-click on the file. The file will automatically uncompress to the same directory.
Using a Shell Script (Optional):

Download the uncompress.sh script from the repository.
Place the script in the same directory as the compressed file.
Open Terminal and navigate to the directory containing the files.
Run the following command to uncompress:
bash
Copy code
sh uncompress.sh
uncompress.sh:

bash
Copy code
#!/bin/bash
echo "Uncompressing the file..."

# Uncompress .zip file
unzip city_market_tracker.zip

# For .tar.gz files, use:
# tar -xzvf city_market_tracker.tar.gz

echo "Uncompression complete."
Additional Notes:
Ensure that the compressed file and the script (if using) are in the same directory.
If the compressed file has a different format (e.g., .tar.gz), the same steps can be followed, but make sure to modify the script or extraction process accordingly.

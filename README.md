# ShareX Linux Script

This script allows you to take a screenshot using Flameshot and upload it to a XBackbone ShareX server. Before using the script, you need to replace the placeholder values with your actual XBackbone ShareX server URL and authentication token.

## Installation
1. Clone the GitHub repository to your local machine using the following command:
```bash
git clone https://github.com/GeorgeV220/ShareX-Linux-Script.git
```
2. Move to the cloned repository directory:
```bash
cd ShareX-Linux-Script
```
3. Now, let's install the script by moving it to /usr/bin, which requires administrative privileges. Use the following command:
```bash
sudo mv upload_screenshot.sh /usr/bin/upload_screenshot
```
4. Make the script executable:
```bash
sudo chmod +x /usr/bin/upload_screenshot
```

## Dependencies
### Debian
Before running the script, ensure that the required dependencies are installed on your Debian system:
1. Flameshot: A powerful screenshot tool.
2. curl: A command-line tool for transferring data with URLs.
3. jq: A lightweight and flexible command-line JSON processor.
You can install these dependencies using the following command:
```bash
sudo apt-get update
sudo apt-get install flameshot curl jq
```

### Arch
Before running the script, ensure that the required dependencies are installed on your Arch system:
1. Flameshot: A powerful screenshot tool.
2. curl: A command-line tool for transferring data with URLs.
3. jq: A lightweight and flexible command-line JSON processor.
You can install these dependencies using the following command:
```bash
sudo pacman -Syu flameshot curl jq
```

## Usage
To use the script, open a terminal and run the following command:
```bash
upload_screenshot
```
The script will take a screenshot using Flameshot, upload it to the specified XBackbone ShareX server, and provide you with the URL. The URL will also be copied to your clipboard for easy sharing.

Note: Make sure you have set up your XBackbone ShareX server URL and obtained an authentication token before running the script. Replace the server_url and auth_token variables in the script with your actual values.

If the screenshot upload is successful, you will receive a notification with the URL. In case of an error, an appropriate error message will be displayed.

Please ensure you have an active internet connection before running the script, as it requires internet access to upload the screenshot to the XBackbone ShareX server.

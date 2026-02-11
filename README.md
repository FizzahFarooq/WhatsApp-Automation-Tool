# WhatsApp-Automation-Tool

A Java-based WhatsApp automation system that allows users to send **bulk text messages, multimedia files, and scheduled automated messages** through WhatsApp Web using Selenium. The project also includes a GUI built with Java Swing for ease of use.

## Features
- Scan QR code to log in to WhatsApp Web
- Load and display WhatsApp contacts dynamically
- Send instant text messages
- Send multimedia files (images, documents, etc.)
- Send **bulk messages** to multiple contacts
- Schedule automated messages with custom time intervals
- User-friendly desktop GUI (Java Swing)

## Technologies Used
- Java
- Selenium WebDriver
- Java Swing (GUI)
- ChromeDriver
- WhatsApp Web

## Project Structure
- **WhatsAppAutomationGUI** – Main GUI application for user interaction  
- **WhatsAppAutomation** – Handles WebDriver setup and WhatsApp Web login  
- **ContactManager** – Fetches and manages WhatsApp contacts  
- **MessageSender (Abstract Class)** – Base structure for message sending  
- **TextMessageSender** – Sends text, bulk, and automated messages  
- **MultimediaMessageSender** – Sends media files (images/documents)  

## How It Works
1. Launch the application and scan the WhatsApp Web QR code.  
2. Load contacts from WhatsApp Web into the GUI.  
3. Select one or multiple contacts from the list.  
4. Choose to send:
   - A single text message  
   - Multimedia files  
   - **Bulk messages** to multiple contacts  
   - Automated messages with a defined interval and count  
5. Selenium WebDriver interacts with WhatsApp Web in real time to send messages.  

## Setup Instructions
1. Install Google Chrome.  
2. Download ChromeDriver compatible with your Chrome version.  
3. Download Selenium Java library from the [official site](https://www.selenium.dev/downloads/).  
4. Add Selenium JAR files to your project:  
   - `selenium-server-<version>.jar`  
   - All JARs inside the `libs` folder of the download  
5. Update the ChromeDriver path in the code:
   ```java
   System.setProperty("webdriver.chrome.driver", "path_to_chromedriver");
6.Run WhatsAppAutomationGUI.java.

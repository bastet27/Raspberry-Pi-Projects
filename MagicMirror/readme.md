# My Mini MagicMirror for Desktop 📆

## Overview
I wanted a compact and functional way to keep track of my **to-do lists**, **calendar events**, and other daily tasks right on my desktop. Using a Raspberry Pi, I built a **Mini MagicMirror** that does exactly that. This project combines my love for tinkering with technology and my need to stay organized.

## Hardware I Used
- **Raspberry Pi 3 Model B**
- **7" Screen**
- **HDMI Cables**
- **16GB MicroSD Card**

## Software Setup

### 1. Installing Raspberry Pi OS
First, I downloaded and installed the Raspberry Pi OS (Full version) onto my 16GB MicroSD card using the Raspberry Pi Imager tool.

### 2. Setting Up MagicMirror²
I followed the [official MagicMirror installation guide](https://docs.magicmirror.builders/getting-started/installation.html#manual-installation). Here’s the step-by-step process I used:

1. **Installing Node.js**  
   I made sure to download and install a compatible version of Node.js for my Raspberry Pi. You can find versions for:
   - [Linux Distributions](https://nodejs.org)
   - [Other Platforms](https://nodejs.org)

2. **Checking for Git**  
   I checked if Git was already installed by running:
   ```
   git
   ```
   If it wasn’t installed, I ran:
   ```
   sudo apt install git
   ```

3. **Cloning the MagicMirror Repository**  
   Next, I cloned the MagicMirror repository with:
   ```
   git clone https://github.com/MagicMirrorOrg/MagicMirror
   ```

4. **Navigating to the Repository**  
   I navigated into the cloned repository folder:
   ```
   cd MagicMirror
   ```

5. **Installing MagicMirror**  
   To install everything MagicMirror needed, I ran:
   ```
   npm run install-mm
   ```

   > **Note:** This step took a while (about 10 minutes on my RPi3), so I grabbed a coffee and let it finish.

6. **Configuring MagicMirror**  
   I copied the sample configuration file to set up my MagicMirror:
   ```
   cp config/config.js.sample config/config.js
   ```

7. **Starting MagicMirror**  
   Finally, I started the MagicMirror application with:
   ```
   npm run start
   ```

   Alternatively, for **Server Only** mode, I could have used:
   ```
   npm run server
   ```

## Next Steps
Now that I’ve got the MagicMirror up and running, I’m customizing it with modules to make it truly mine. Some features I’m planning to add include:
- **Google Calendar Integration**: Syncing my events and reminders.
- **To-Do List**: Using the `MMM-Todoist` module to keep track of tasks.
- **Weather Updates**: Adding a weather module for daily forecasts.

This setup is already making my workspace more productive and organized. If you’re interested in building something similar, feel free to ask questions or share your ideas!

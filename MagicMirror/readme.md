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

## Modules I Use
I’ve customized my MagicMirror setup with the following modules:
- **Clock**: Displays the current time and includes moon phase settings phase percentage, rise, and set.
- **Weather**: Provides daily weather updates.
- **Calendar**: Syncs with my iCloud calendar for upcoming events.  
  I followed the guide from [this forum post](https://forum.magicmirror.builders/topic/5327/sync-private-icloud-calendar-with-magicmirror?page=1) to sync private iCloud calendars with MagicMirror.

## Customizations
1. **Wallpaper**: I created a custom CSS file (`custom.css`) to add a static wallpaper as the background. The wallpaper is a beautiful image that enhances the overall aesthetic.
2. **Module Layout**: Arranged the modules to maximize visibility and functionality for my workflow.
3. **Moon Phase Settings**: Added moon phase display in the clock module, which shows sunrise, sunset, moonrise, and moonset times.

## Next Steps
While my MagicMirror is already functional and tailored to my needs, I’m considering adding more modules and features, such as:
- **To-Do List Integration**: Syncing my tasks with MagicMirror.

This setup has improved my productivity and brought a modern touch to my workspace. If you’re planning a similar project or have suggestions, feel free to share them!

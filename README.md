# Smart Train Station Automation

## 1. Project Goals and Motivation
The goal of this project is to improve train traffic management in stations using both automatic and manual control to reduce delays caused by:
Track congestion.
Inability to enter the station due to an occupied track.
The system allows manual or automatic control on Raspberry Pi 3.
It can display real-time updates on a local GUI, and users can also access the information remotely through an HTML web interface hosted on GitHub Pages.
Additionally, the system sends updates to a JSON file on GitHub Gist, which the web interface reads to reflect changes in real-time.

## 2. System Diagram

<img width="1536" height="1024" alt="project diagram" src="https://github.com/user-attachments/assets/c2a8f0d6-4954-4de4-b410-168739f4ba05" />

- Trains move along the tracks.
- Raspberry Pi controls switches and reads sensors.
- Updates are sent to JSON on GitHub Gist.
- Web interface displays the current status in real-time.

## 3. Target Build System
- **Buildroot** for running the system on the Raspberry Pi.

## 4. Hardware Platform
- Raspberry Pi 3
- Touchscreen display
- Electric switches to control train movement
- Sensors to detect track occupancy

## 5. Open Source Projects / Packages
- Python GPIO library for controlling switches
- Python for backend and Frontend
- HTML / CSS for frontend remotly
- GitHub Gist API to send real-time updates

## 6. Previous Assignment Content
- Buildroot setup
- Running an application on startup

## 7. New Content Beyond Course
- Smart scheduling algorithm for train management
- Automatic JSON updates when track status changes
- HTML and GUI interface displaying real-time track status

## 8. Source Code Organization
- `main-repo`: Buildroot setup + backend scripts + frontend code + scheduling logic
- Everything is managed in a **single repository** with clear folders:
  - `/backend` → Python scripts for GPIO and JSON updates
  - `/frontend` → HTML/JS/CSS for web interface
  - `/docs` → Diagrams and documentation

## 9. References
- [Buildroot Raspberry Pi Support](https://buildroot.org/downloads/manual/manual.html#raspberrypi)
- GitHub Gist API documentation

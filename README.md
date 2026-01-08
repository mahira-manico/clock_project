# ⏰ Clock Project

A simple command-line clock application with customizable time and alarm functionality.

## 📋 Features

- **Real-time clock** that runs continuously in the background
- **Change time** manually to any hour, minute, and second
- **Set alarms** that ring when the specified time is reached
- **Reset time** to system time instantly
- **Input validation** to prevent errors
- **Clean terminal interface** with hidden cursor for smooth display

## 🚀 Installation

### Prerequisites

- Python 3.6 or higher
- pip (Python package manager)

### Clone the repository

```bash
git clone https://github.com/mahira-manico/Clock-project.git
cd Clock-project
```

### Install dependencies

```bash
pip install keyboard
```

## 💻 Usage

Run the program:

```bash
python clock.py
```

### Menu Options

- **Press A** - Change the current time
- **Press B** - Set an alarm
- **Press C** - Reset time to system time

### Setting the Time

1. Press `A` in the menu
2. Enter the hour (0-23)
3. Enter the minutes (0-59)
4. Enter the seconds (0-59)

### Setting an Alarm

1. Press `B` in the menu
2. Enter the alarm hour (0-23)
3. Enter the alarm minutes (0-59)
4. Enter the alarm seconds (0-59)
5. The alarm will ring when the current time matches the set time

## 🛠️ Technical Details

### Technologies Used

- **Python 3**
- **threading** - For running the clock in the background
- **datetime** - For time manipulation
- **keyboard** - For key press detection

### How It Works

1. A background thread (`running_hour()`) continuously increments the time every second
2. The main menu displays the current time and checks for alarm triggers
3. ANSI escape codes are used for terminal control (cursor hiding, screen clearing)
4. Input validation ensures only valid time values are accepted

## ⚠️ Known Limitations

- Terminal must support ANSI escape codes

## 🔧 Troubleshooting

### Keyboard library not working

Make sure you've installed it correctly:
```bash
pip install keyboard 
```

## 📝 Future Improvements
- [ ] Add a feature to stop time
- [ ] Add a 12h format
- [ ] Add multiple alarm support
- [ ] Save alarms to a file
- [ ] Add sound notification for alarms
- [ ] GUI version with tkinter

## 👤 Author

**Mahira Manico**

- GitHub: [@mahira-manico](https://github.com/mahira-manico)

## 🙏 Acknowledgments

Built as a learning project to practice:
- Threading in Python
- Terminal control with ANSI codes
- User input validation
- Time manipulation with datetime

---

⭐ If you found this project helpful, consider giving it a star on GitHub!

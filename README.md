# 🚀 Swoosh - Hand Gesture Desktop Control

**The Ultimate Hand Gesture Control for Your Desktop!** 

Switch between virtual desktops and applications with simple hand gestures - it's like flipping through pages in a book! 📖✋

![Swoosh Demo](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## ✨ Features

- **🖐️ Intuitive Hand Gestures**: Control your desktop naturally with hand movements
- **🎥 Real-time Camera Feed**: See exactly what the AI sees with live overlay
- **🔊 Sound Effects**: Satisfying audio feedback for every gesture
- **⚙️ Customizable Settings**: Adjust sensitivity, actions, and visual effects
- **🎨 Beautiful UI**: Modern, translucent overlay with smooth animations
- **💻 Cross-Platform**: Works on Windows, macOS, and Linux
- **🎯 System Tray Integration**: Always accessible from your system tray

## 🎮 How to Use

### Hand Gestures

| Gesture | Action |
|---------|--------|
| 🖐️ **Open Hand + Left Swipe** | Previous Virtual Desktop |
| 🖐️ **Open Hand + Right Swipe** | Next Virtual Desktop |
| ✊ **Closed Fist + Left Swipe** | Previous Window (Alt+Shift+Tab) |
| ✊ **Closed Fist + Right Swipe** | Next Window (Alt+Tab) |

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+Shift+A` | Toggle camera overlay |

### System Tray

Right-click the Swoosh icon in your system tray for quick access to:
- Show/Hide Overlay
- Settings
- Sound Controls
- About & Help

## 🛠️ Installation

### Quick Setup

1. **Clone or download this repository**
   ```bash
   git clone https://github.com/your-username/swoosh.git
   cd swoosh
   ```

2. **Run the setup script**
   ```bash
   python setup.py
   ```

3. **Start Swoosh**
   ```bash
   python main.py
   ```

### Manual Installation

1. **Install Python 3.8+** (if not already installed)

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run Swoosh**
   ```bash
   python main.py
   ```

## 📋 Requirements

### System Requirements
- **Python**: 3.8 or higher
- **Camera**: Any USB webcam or built-in camera
- **OS**: Windows 10/11, macOS 10.14+, or Linux (Ubuntu 18.04+)
- **RAM**: 4GB minimum (8GB recommended)

### Python Dependencies
- PyQt6 (GUI framework)
- OpenCV (computer vision)
- MediaPipe (hand detection)
- PyAutoGUI (system control)
- Pygame (sound effects)
- pynput (global hotkeys)

## ⚙️ Configuration

### Settings Tabs

#### 📹 Input
- **Camera Selection**: Choose your preferred camera
- **Sensitivity**: Adjust gesture detection sensitivity
- **Detection Confidence**: Fine-tune hand detection accuracy
- **Gesture Cooldown**: Set delay between gesture recognitions

#### ⚡ Actions
- **Enable/Disable Actions**: Toggle window switching and desktop switching
- **Control Mode**: Choose between fist/open hand modes

#### 🔊 Audio
- **Sound Effects**: Enable/disable audio feedback
- **Volume Control**: Adjust sound effect volume
- **Test Sounds**: Preview all sound effects

#### 🎨 Display
- **Visual Effects**: Toggle gesture trails and text feedback
- **Overlay Opacity**: Adjust transparency of camera overlay
- **Animation Settings**: Control visual feedback intensity

## 🎯 Tips for Best Performance

### Camera Setup
- 💡 **Good Lighting**: Ensure your hand is well-lit for better detection
- 📐 **Proper Distance**: Keep your hand 1-3 feet from the camera
- 🖐️ **Clear Background**: Avoid cluttered backgrounds behind your hand
- 📱 **Camera Position**: Position camera at chest/shoulder height

### Gesture Tips
- ✋ **Deliberate Movements**: Make clear, intentional swipes
- ⏱️ **Consistent Speed**: Don't move too fast or too slow
- 🎯 **Practice**: Try the gestures a few times to get the feel
- 🔄 **Cooldown**: Wait for the gesture cooldown before next gesture

### Performance Optimization
- 🔧 **Adjust Sensitivity**: Lower sensitivity if gestures trigger too easily
- 📺 **Single Monitor**: Works best with one camera and monitor setup
- 💻 **Close Unnecessary Apps**: Free up system resources
- 🔋 **Power Settings**: Use high-performance mode for best results

## 🐛 Troubleshooting

### Common Issues

#### Camera Not Working
- ✅ Check if camera is connected and working in other apps
- ✅ Try different camera index in settings
- ✅ Restart Swoosh after changing cameras
- ✅ Check camera permissions (especially on macOS)

#### Gestures Not Detected
- ✅ Improve lighting conditions
- ✅ Increase sensitivity in settings
- ✅ Check hand distance from camera
- ✅ Ensure hand is clearly visible

#### Performance Issues
- ✅ Close other camera applications
- ✅ Lower detection confidence slightly
- ✅ Disable visual effects if needed
- ✅ Check system resources (CPU/RAM usage)

#### Sound Problems
- ✅ Check system volume settings
- ✅ Test sounds in Swoosh settings
- ✅ Restart application if sounds don't work
- ✅ Check audio drivers

### Platform-Specific Notes

#### Windows
- Works best with Windows 10/11
- May need to allow camera access in Privacy settings
- Some antivirus software may flag the global hotkey feature

#### macOS
- Camera permission required on first run
- Accessibility permissions may be needed for hotkeys
- Command key used instead of Ctrl for window switching

#### Linux
- May need additional packages: `sudo apt-get install python3-dev libgl1-mesa-glx`
- Camera access permissions may vary by distribution
- Test with different camera backends if issues occur

## 🔧 Advanced Configuration

### Custom Hotkeys
You can modify the global hotkey in the code:
```python
shortcut_str = '<ctrl>+<shift>+a'  # Change this line in setup_hotkey_listener()
```

### Custom Actions
Add your own actions by modifying the `handleGesture` method in the `OverlayWindow` class.

### Sound Customization
Replace sound files in the `sounds/` directory or modify the `SoundManager` class to use your own audio effects.

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **🐛 Bug Reports**: Open an issue with detailed steps to reproduce
2. **💡 Feature Requests**: Suggest new features or improvements
3. **🔧 Code Contributions**: Fork, make changes, and submit a pull request
4. **📚 Documentation**: Help improve this README or add code comments
5. **🧪 Testing**: Test on different platforms and report compatibility

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **MediaPipe**: For excellent hand tracking capabilities
- **OpenCV**: For computer vision functionality
- **PyQt6**: For the beautiful GUI framework
- **The Open Source Community**: For all the amazing libraries that made this possible

## 📞 Support

Having issues? Need help?

- 📖 **Check this README** for troubleshooting tips
- 🐛 **Open an Issue** on GitHub with detailed information
- 💬 **Join Discussions** for community support
- ⭐ **Star this repo** if Swoosh helped you!

---

**Made with ❤️ for a more intuitive desktop experience**

*Swoosh - Because your hands deserve better than keyboard shortcuts!* 🚀✋

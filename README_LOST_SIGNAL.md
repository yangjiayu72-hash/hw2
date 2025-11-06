# Lost Signal - Interactive Story

An interactive web-based story experience where your choices determine the fate of a mysterious transmission.

## How to Run

Simply open `index.html` in any modern web browser (Chrome, Firefox, Safari, Edge).

```bash
# Option 1: Double-click the file
# Option 2: From command line
firefox index.html
# or
google-chrome index.html
```

## Story Overview

You receive a mysterious transmission that is breaking apart. The signal is degrading, and you must decide how to respond. Each choice you make will affect the signal strength and ultimately determine the ending of the story.

## Features

### Visual Effects
- **Flickering CRT-style display** with scanlines
- **Dynamic noise effects** that change based on signal strength
- **Glitching text** when signal is weak
- **Transmission line animations** when forwarding messages
- **Signal strength indicator** that updates in real-time

### Interactive Elements

#### 1. **REPLY Button**
- Opens an input box for you to type a message
- **Effect**: Strengthens the signal (+15%)
- **Sound**: Gentle electronic beep
- **Feedback**: Your reply is displayed in the communication window

#### 2. **IGNORE Button**
- Dismisses the current transmission
- **Effect**: Weakens the signal (-20%)
- **Sound**: Low-pitched distortion buzz
- **Feedback**: Message becomes noisier and starts fading

#### 3. **FORWARD Button**
- Opens a submenu with three options:
  - **Send to Friend**: Share with someone else (+5% signal)
  - **Send to Archive**: Preserve in memory (+10% signal)
  - **Send to Self**: Loop back to yourself (-5% signal)
- **Effect**: Varies by destination
- **Sound**: Triple beeping transmission sound
- **Animation**: Transmission line shoots across the screen

### Three Possible Endings

After **at least 3 actions**, you'll reach one of these conclusions:

#### 🔄 **TIME LOOP**
- **Triggered by**: Forwarding the message to yourself
- **Revelation**: You discover you've been both the sender and receiver all along, caught in an endless temporal loop

#### 🌟 **NEW TIMELINE (Branch)**
- **Triggered by**: Replying frequently (2+ replies)
- **Revelation**: Your engagement creates a stable connection, forming a new branching timeline where contact is successfully made

#### 💀 **SIGNAL LOST (Dissolve)**
- **Triggered by**: Ignoring the message too often (2+ ignores)
- **Revelation**: The signal completely dissolves into noise, lost forever in the void

#### ❓ **UNCERTAIN RESOLUTION**
- **Triggered by**: Mixed actions with no clear pattern
- **Revelation**: The signal exists in an indeterminate quantum state, neither fully connected nor completely lost

## Technical Details

### Technologies Used
- **HTML5** for structure
- **CSS3** for animations and visual effects
  - CRT scanline effect
  - Dynamic noise overlay
  - Flickering animations
  - Signal strength visualization
- **Vanilla JavaScript** for interaction logic
- **Web Audio API** for procedural sound generation

### Key Interactions Tracked
- Number of replies sent
- Number of times message was ignored
- Number of forwards and their destinations
- Signal strength (0-100%)
- User's actual reply text
- Total actions performed

### Sound Effects
All sounds are generated procedurally using the Web Audio API:
- **Reply**: Sine wave at 800Hz (gentle electronic tone)
- **Ignore**: Sawtooth wave at 120Hz (harsh buzz)
- **Forward**: Three square wave beeps at 1200Hz

## Gameplay Tips

- Watch the **signal strength bar** - it affects the visual noise level
- Your replies are preserved and shown in the final statistics
- Try different strategies to see all three main endings
- Each playthrough takes about 1-2 minutes
- The story is designed to be replayed to explore different paths

## Design Philosophy

Lost Signal explores themes of:
- **Connection vs. Isolation**: The choice to engage or disconnect
- **Time and Causality**: Especially in the Time Loop ending
- **Consequence**: How small decisions compound into major outcomes
- **Communication**: The importance (or futility) of reaching out

## Credits

Created as an interactive narrative experiment combining:
- Retro terminal aesthetics
- Branching narrative design
- Real-time feedback systems
- Procedural audio generation

---

**Enjoy your journey through the signal!**

*Remember: Every transmission is a chance to connect. What will you choose?*

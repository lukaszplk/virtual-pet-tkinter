# Virtual Pet (Tkinter)

An interactive virtual pet application built with Python and Tkinter. A cute animated creature that responds to your mouse interactions.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Tkinter](https://img.shields.io/badge/GUI-Tkinter-green)

## Features

| Interaction | Pet Response |
|-------------|--------------|
| Hover mouse over pet | Smiles + pink cheeks appear (happy) |
| Move mouse away | Returns to neutral expression |
| Double-click | Crosses eyes + sticks tongue out (cheeky) |
| Leave alone ~50 sec | Gets sad |
| Watch | Blinks automatically every 3 seconds |

## Demo

The pet is a light blue creature with:
- Oval body with pointy ears
- Expressive eyes that blink and can cross
- Mouth that changes between happy/neutral/sad
- Pink cheeks when happy
- Red tongue for cheeky mode

## Requirements

- Python 3.x
- Tkinter (included with Python)

## Run

```bash
python main.py
```

Or run the Jupyter notebook:
```bash
jupyter notebook main.ipynb
```

## How It Works

### Canvas Drawing
Uses `tkinter.Canvas` to draw shapes:
- `create_oval()` - body, eyes, cheeks, feet
- `create_polygon()` - ears
- `create_line()` - mouth expressions
- `create_rectangle()` - tongue

### Event Handling
- `<Motion>` - detect mouse hover
- `<Leave>` - detect mouse exit
- `<Double-1>` - detect double-click

### Animations
Uses `root.after(ms, callback)` for timed events:
- Blinking every 3 seconds
- Happiness decay every 5 seconds
- Tongue/eye reset after 1 second

## Project Structure

```
virtual-pet-tkinter/
├── main.py          # Main application
├── main.ipynb       # Jupyter notebook version
├── LICENSE
└── README.md
```

## Learning Concepts

This project demonstrates:
- Tkinter Canvas widget
- Drawing shapes programmatically
- Mouse event bindings
- State management in GUI
- Timed callbacks with `after()`

## License

MIT License

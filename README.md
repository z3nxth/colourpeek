# colourpeek

Instantly preview an image and print its dominant colours to the terminal.

![Colourpeek Screenshot](Screenshot%202025-06-03%20at%2000.25.01.png)

---

## Features

- Creates nice, aesthetic colour palette through `colourthief` to grab colours.
- Uses `climage` for a preview of the image in-terminal.
- Lightweight & fast.

---

## Installation (Global)

### Linux / macOS:

```bash
git clone https://github.com/niftyifty/colourpeek.git
cd colourpeek

pip install . --user
```
### Windows (Command Prompt or PowerShell):
```
git clone https://github.com/niftyifty/colourpeek.git
cd colourpeek

pip install . --user
```

---


## Usage

`colourpeek path/to/image.jpg`

Example:

`colourpeek ~/Pictures/sunset.png`

Uninstall (_not that you'd ever need to_) 
`pip uninstall colourpeek`

---

## Flags

Flag	Description
-n, --num	Number of dominant colours to extract (default: 8)
--truecolor	Manually set terminal colour mode: yes, no, or ask
--remember	Save your answer to the truecolor prompt
--forget	Ignore saved config and ask again
-h, --help	Show help message

---

## Dependencies
- colorthief – For palette extraction
- climage – For image preview in ANSI
- argparse – For CLI parsing (built-in)

---

### Configuration

Settings like truecolor preference are saved in:

~/.colourpeek_config.json

To reset, run with --forget.

---

## credits 
Terminal image rendering by climage
Colour extraction powered by Color Thief


---

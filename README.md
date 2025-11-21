# Analog Clock

A simple, lightweight analog clock application written in C/C++ designed to display the current system time in a classic analog format. This project is ideal for learning graphics rendering, system time handling, and basic event loop programming.

---

## Overview

The Analog Clock project renders a real-time analog clock with hour, minute, and second hands. It demonstrates:

* Reading system time
* 2D graphics rendering (ticks, hands, labels)
* Smooth animation using a render loop
* Basic user-configurable settings (colors, sizes)

This repository includes a Code::Blocks project file for easy opening and building.

---

## Key Features

* Real-time hour, minute, and second hands
* Smooth animation and anti-aliased rendering (depends on graphics lib)
* Configurable clock size and hand lengths
* Simple, commented C/C++ source suitable for learning

---

## Project Structure

```
Analog Clock/
├── Analog Clock.cbp       # Code::Blocks project file (use this to open in Code::Blocks)
├── src/                  # Source code files (e.g., main.cpp, clock.cpp, clock.h)
├── assets/               # Optional images or resources (icons, fonts)
├── README.md             # This file
└── LICENSE               # Project license (MIT recommended)
```

> **Note:** The included Code::Blocks project file is available at: `/mnt/data/Analog Clock.cbp`.

---

## Technologies & Libraries

* **Language:** C / C++
* **Possible Graphics Libraries:** WinBGI, SDL2, SFML, OpenGL, or platform-native GDI (depending on your implementation)
* **IDE:** Code::Blocks (project file included)

---

## Requirements

* A C/C++ compiler (MinGW for Windows or GCC/Clang for Linux)
* Code::Blocks recommended for opening the `.cbp` project file
* If using an external graphics library (SDL2, SFML), install the corresponding development packages

---

## Build & Run (Using Code::Blocks)

1. Open Code::Blocks.
2. Go to **File → Open** and select the project file: `/mnt/data/Analog Clock.cbp`.
3. Build the project (Build → Build).
4. Run the project (Build → Run or press `F9`).

### Build manually (command-line example)

If the project uses a single `main.cpp` and no external libs, you can compile with:

```bash
g++ src/main.cpp -o analog_clock
./analog_clock
```

If using SDL2 or SFML, add the appropriate compiler/linker flags.

---

## Configuration & Customization

You can modify constants in the source code to change:

* Clock radius and window size
* Hand lengths and thickness
* Colors for background, ticks, and hands
* Tick mark styles (numbers, dots, or lines)

Search for clearly labeled `// CONFIG` or `// SETTINGS` sections in the source files.

---

## Troubleshooting

* **Blank window / no rendering:** Ensure the graphics library is initialized correctly and the render loop is running.
* **Compilation errors:** Check include paths and linked libraries if using third-party graphics packages.
* **Time incorrect:** Verify your system time or the time-fetching function used (localtime vs gmtime).

---

## License

This project is released under the **MIT License**. See the `LICENSE` file for details.

---

## Contributing

Contributions are welcome! Typical contributions:

* Improve rendering or add smoothing/anti-aliasing
* Add settings UI to change clock appearance at runtime
* Port to other graphics libraries or platforms

Please open an issue or submit a pull request.

---

## Author

Developed by **Harsh Arora**

---


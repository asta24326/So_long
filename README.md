*This project has been created as part of the 42 curriculum by asharafe.*

# 🎮 So Long

### ✅ Result: 122/100

## 📄 Description
So Long is a small 2D game developed using the MiniLibX library. The goal is to create a simple top-down puzzle game where a player collects all items on a map and reaches an exit while avoiding obstacles (or enemies in the bonus part). This project serves as an introduction to basic graphics programming, window management, event handling (keyboard and mouse), and working with textures and sprites.



---

## 🎯 Acquired Skills
* **Graphics Programming**: Rendering images and managing windows using the MiniLibX library.
* **Event Handling**: Capturing and processing user input (key presses and window closing events).
* **Game Logic**: Implementing movement, collision detection, and win/loss conditions.
* **Map Parsing**: Reading and validating map files (`.ber`) to ensure they meet specific requirements.
* **Asset Management**: Working with XPM textures and sprite sheets.

---

## 🛠 Contents
The project includes the following components:
1. **Mandatory Part**: A functional game with movement, collectibles, an exit, and a movement counter displayed in the terminal.
2. **Map Validation**: Ensuring the map is rectangular, surrounded by walls, and has a valid path to all objectives.
3. **Bonus Part**: Additional features such as sprite animations, an on-screen move counter, and patroling enemies that end the game on contact.

---

## ⚙️ Compilation
The project includes a `Makefile` that compiles the source files and links the MiniLibX library.

To compile the mandatory part:
```bash
make

```

To compile the bonus part:

```bash
make bonus

```

To clean the project:

```bash
make fclean

```

---

## 🧪 How to Use

The program takes a map file with the `.ber` extension as an argument.

1. **Run the game**:

```bash
./so_long maps/map.ber

```

2. **Controls**:

* **W/A/S/D or Arrow Keys**: Move the character.
* **ESC**: Close the game.
* **Click on the 'X'**: Close the game window.

3. **Map Rules**:

* `1`: Wall
* `0`: Empty space
* `C`: Collectible
* `E`: Exit
* `P`: Player starting position

---

## 💡 AI Usage

AI tools were used during the development of this project for:

* **Documentation**: Structuring the README to maintain the established gold standard for 42 projects.
* **Optimization**: Improving the flood-fill algorithm used to verify that the map has a valid path.
* **Bug Squashing**: Identifying memory leaks related to image destruction and window cleanup.
* *Note: All core gameplay mechanics and map parsing logic were implemented manually.*

---

## 🔗 Resources

* 42 Project Subject: So Long.
* [MiniLibX Documentation](https://harm-smits.github.io/42docs/libs/minilibx).
* [2D Game Development Basics](https://en.wikipedia.org/wiki/2D_computer_graphics).
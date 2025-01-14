# Whack-a-Mole Verilog Project

## 📚 Project Description
This is a **FPGA-based Whack-a-Mole game** implemented in Verilog. The project includes features such as:
- **Dot Matrix Display**: Shows the current score.
- **7-Segment Display**: Acts as a countdown timer.
- **VGA Display**: Provides the main game interface for players.

---

## 🛠️ Features
1. **Dot Matrix**: Displays player's hit score in real-time.
2. **7-Segment Display**: Countdown timer with adjustable time intervals.
3. **VGA Display**: Provides a dynamic and visually appealing game interface.
4. **Modular Design**: Each component (Dot Matrix, VGA driver, Timer, etc.) is designed independently for easy testing and integration.

---

## 📋 To-Do List
- [x] Design a timer for the game:
  - [x] Implement a countdown timer that starts from a configurable initial value (e.g., 30 seconds).
  - [x] Stop the game when the timer reaches 0 by triggering a `stop` signal.
  - [x] Allow the game to reset and start a new session when the `reset` signal is activated.

- [ ] Resolve the issue where `keypadBuf` retains its previous value when no button is pressed:
  - [ ] Ensure that `hit` is not triggered unless a new button press updates the `keypadBuf`.
  - [ ] Implement logic to detect "no input" scenarios and handle them appropriately.
  - [ ] Test with various cases, such as no button pressed, multiple buttons pressed, and valid inputs.

---

## ⚙ Settings

1. [Pin Assignment](https://github.com/DennisLee03/Whack-A-Mole/blob/main/top.qsf) - The Board is DE10-Lite
2. [Module Structure](https://github.com/DennisLee03/Whack-A-Mole/blob/main/module-design.pdf) - Generated by Quartus Prime Lite Edition

---

## 🎥 Demo

- [Video Here!](https://www.youtube.com/watch?v=aqGkdmAqu8M)

---
## 📖 References
1. [VGA Basic 1](https://www.youtube.com/watch?v=mR-eo7a4n5Q&t=101s) - To know basic VGA signals
2. [VGA Basic 2](https://www.cnblogs.com/liujinggang/p/9690504.html) - To know basic VGA signals
3. [Whack A Mole idea](https://blog.csdn.net/qq_43499622/article/details/100742468)

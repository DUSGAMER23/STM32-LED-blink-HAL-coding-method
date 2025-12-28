# STM32 LED Blink — HAL Coding Method

This repository contains a **beginner-friendly STM32CubeIDE project** that blinks an LED on an STM32F446RET6 microcontroller using the **STM32 HAL (Hardware Abstraction Layer)**.  
It’s a simple embedded firmware example — perfect as a first STM32 project or for learning how to use CubeMX and HAL GPIO toggling.

---

## 🚀 What This Project Does

- Configures a GPIO pin connected to an onboard LED.
- Toggles the LED on/off in a loop with a delay.
- Built using **STM32CubeIDE** with HAL drivers (no low-level register code).  
This makes it easy to understand and modify for beginners.

---

## 📦 Repository Structure

```

STM32-LED-blink-HAL-coding-method/
├── Core/                  → Source (`Src/`) and Header (`Inc/`) files
├── Drivers/               → HAL and CMSIS drivers
├── Startup/               → Startup assembly and linker scripts
├── STM32F446RETX_FLASH.ld → Linker script
├── STM32F446RETX_RAM.ld   → RAM layout
├── LED_blink_HAL_project.ioc → CubeMX configuration
├── .project               → IDE project metadata
├── .cproject              → Toolchain config
├── .gitignore             → Ignore build outputs

````

## 🛠️ How to Build & Run

### 1. Clone the repository
```bash
git clone https://github.com/DanielRajChristeen/STM32-LED-blink-HAL-coding-method.git
cd STM32-LED-blink-HAL-coding-method
````

### 2. Open in STM32CubeIDE

* Launch **STM32CubeIDE**
* Go to **File → Import → Existing Projects into Workspace**
* Select this folder

### 3. Build the project

* Click the **Build** button in STM32CubeIDE
* Confirm there are no compile errors

### 4. Flash to your board

* Connect your STM32F446RET6 board via ST-Link
* Use **Run → Debug** or **Run → Run**
  The LED should start blinking!

---

## 🧠 What You Learn Here

This project teaches:

* How to configure GPIO using CubeMX
* How HAL functions (`HAL_GPIO_TogglePin`) work
* How the build & debug process flows in STM32CubeIDE

Perfect for beginners stepping into embedded firmware development. ([STMicroelectronics][2])

---

## 📌 Notes & Tips

* The HAL library **simplifies peripheral access** compared to low-level register programming.
* You can modify the LED blink speed in `main.c`.
* Make sure the correct board/MCU is selected when opening in CubeIDE.

---

## 📜 License

This project is open-source. Use it, learn from it, and adapt it!

---

## ❤️ Acknowledgements

Inspired by embedded learning resources and STM32 community examples.

Happy hacking! 💡

---

# VimMouse

Control the cursor with your hands on the keyboard’s home row — even if you don’t have a ThinkPad.

🎯 This project is based on [EsportToys/TPMouse](https://github.com/EsportToys/TPMouse.git).  
**Many thanks to the original author for their great work!**

## Improvements in This Version

- ✅ Keybindings optimized for **Vim users**.
- ✅ Tweaked cursor and scroll speed for smoother control.
- ✅ **Grid mode** now supports **multi-monitor environments** for precise positioning across screens.

---

## Inertia Mode

![image](https://user-images.githubusercontent.com/98432183/197381484-b4e669f0-c5bd-42af-a469-f21f5191a6a3.png)

1. **Activate** with <code>\`I</code> (Backtick + I).
2. Move the cursor using `H` / `J` / `K` / `L`:
   - `H`: Left
   - `J`: Down
   - `K`: Up
   - `L`: Right
3. Hold `S` to brake for more precise movement.  
   Hold `Space` to scroll horizontally/vertically.
4. Click with:
   - `A`: Left Click
   - `D`: Right Click
   - `W`: Middle Click
5. **Exit** with <code>\`O</code> (Backtick + O) or `Esc`.

---

## Grid Mode

![image](https://user-images.githubusercontent.com/98432183/197323322-09607efb-c940-4add-95e8-660c94c18306.png)

1. **Activate** with <code>\`P</code> (Backtick + P).
2. A red grid overlay will appear. Use `H`/`J`/`K`/`L` to narrow down the search area.
3. Click with `A` (left), `D` (right), or `W` (middle).
4. **Exit** with <code>\`O</code> or `Esc`.

🆕 **Multi-monitor support**: Use number keys (`0`–`9`) to quickly switch and target grid mode on a specific screen. The grid will automatically snap to that monitor.

---

## Demo Videos

### Inertia Mode

https://user-images.githubusercontent.com/98432183/198895264-45823df6-8e8e-4135-9e7d-4ea9c5408c43.mp4

### Grid Mode

https://user-images.githubusercontent.com/98432183/198895269-4a5b7266-f662-491c-810e-5a2d87ddfc47.mp4

---

## Configuration: `options.ini`

You can customize keybindings and inertia parameters via the `options.ini` file. If the file is missing, the script falls back to these defaults:

```ini
[Inertia]
DampingCoef=15
BrakingCoef=90
NormalSensitivity=1
ScrollSensitivity=1

[Bindings]
up=VK_K
left=VK_H
down=VK_J
right=VK_L
mb1=VK_A
mb2=VK_D
mb3=VK_W
brake=VK_S
scroll=VK_SPACE


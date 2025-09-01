# VimMouse

Control the cursor while keeping your hands on the home row — no need for a ThinkPad.

🔧 This project is a customized version of [EsportToys/TPMouse](https://github.com/EsportToys/TPMouse.git).  
**Credit to the original author!**

## What's Improved in This Version

- ✅ Key bindings are redesigned for **Vim enthusiasts** — using familiar `HJKL` navigation.
- ✅ Cursor and scroll speeds are adjusted for smoother control.
- ✅ **Grid Mode** now supports **multi-monitor** environments, allowing precise cross-screen cursor placement.

---

## Inertia Mode

![image](https://user-images.githubusercontent.com/98432183/197381484-b4e669f0-c5bd-42af-a469-f21f5191a6a3.png)

1. Activate with `CapsLk + C` or `LShift + RShift + C`.  
   Your main cursor will change to a crosshair.
2. Move the cursor using `K`/`H`/`J`/`L`.
   - Hold `S` to brake and slow movement for precise aiming.
   - Hold `Space` to scroll both vertically and horizontally.
3. Click with:
   - `A`: Left Click
   - `D`: Right Click
   - `W`: Middle Click
4. Quit using `CapsLk + Q`, `LShift + RShift + Q`, or just `Esc`.

---

## Grid Mode

![image](https://user-images.githubusercontent.com/98432183/197323322-09607efb-c940-4add-95e8-660c94c18306.png)

1. Activate with `CapsLk + G` or `LShift + RShift + G`.
   - A red frame will appear around your screen.
2. Use `K`/`H`/`J`/`L` to shrink the selection area.
3. Click with:
   - `A`: Left Click
   - `D`: Right Click
   - `W`: Middle Click
4. Quit using `CapsLk + Q`, `LShift + RShift + Q`, or just `Esc`.

🆕 **Multi-Monitor Support**:  
You can now press a number key (`0`–`9`) to quickly switch the red frame to a different monitor for seamless multi-screen navigation.

---

## Demo

### Inertia Mode

https://user-images.githubusercontent.com/98432183/198895264-45823df6-8e8e-4135-9e7d-4ea9c5408c43.mp4

### Grid Mode

https://user-images.githubusercontent.com/98432183/198895269-4a5b7266-f662-491c-810e-5a2d87ddfc47.mp4

---

## Configuration: `options.ini`

You can customize inertia behavior and key bindings by editing the `options.ini` file.  
If the file doesn't exist, the following default values are used:

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




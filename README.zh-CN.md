# VimMouse
📘 English version: [README.md](./README.md)

Control the cursor with your hand staying on the keyboard's homerow — even if you don't have a ThinkPad.

🎯 本项目是基于原项目 [EsportToys/TPMouse](https://github.com/EsportToys/TPMouse.git) 魔改后的。**感谢原作者的贡献！**

## 本版本改进说明

- ✅ 键位布局更符合 **Vim 爱好者** 的操作习惯。
- ✅ 调整了光标和滚轮的移动速度，操作更顺畅。
- ✅ **Grid 模式** 现已支持 **多屏幕 / 多显示器** 精准定位，方便多屏用户快速定位。

## 🔧 运行环境要求

要运行 **VimMouse**，你需要先安装以下组件：

- [AutoIt3](https://www.autoitscript.com/site/autoit/downloads/)
- [SciTE4AutoIt3](https://www.autoitscript.com/site/autoit-script-editor/downloads/)

这两个工具用于运行、编译和调试 `.au3` 脚本，是 VimMouse 的运行基础。


---

## Inertia 模式

![image](https://user-images.githubusercontent.com/98432183/197381484-b4e669f0-c5bd-42af-a469-f21f5191a6a3.png)

1. **激活方式**：<code>\`I</code>（反引号 + I）
2. 使用 `H`/`J`/`K`/`L` 控制光标方向：
   - `H`：向左
   - `J`：向下
   - `K`：向上
   - `L`：向右
3. 按住 `S` 可刹车以进行更精确的移动；按住 `Space` 可滚动页面。
4. 使用 `A`/`D`/`W` 分别进行左键 / 右键 / 中键点击。
5. **退出方式**：<code>\`O</code>（反引号 + O）或按 `Esc`。

---

## Grid 模式

![image](https://user-images.githubusercontent.com/98432183/197323322-09607efb-c940-4add-95e8-660c94c18306.png)

1. **激活方式**：<code>\`P</code>（反引号 + P）
2. 屏幕上会出现红框，使用 `H`/`J`/`K`/`L` 缩小定位范围。
3. 使用 `A`/`D`/`W` 进行点击（左/右/中键）。
4. 退出方式同上。

🆕 **多屏支持**：你可以使用数字键（0–9）快速切换到不同显示器上的 Grid 模式，边框会自动定位到对应屏幕区域。

---

## 演示视频

### Inertia Mode

https://user-images.githubusercontent.com/98432183/198895264-45823df6-8e8e-4135-9e7d-4ea9c5408c43.mp4

### Grid Mode

https://user-images.githubusercontent.com/98432183/198895269-4a5b7266-f662-491c-810e-5a2d87ddfc47.mp4

---

## 配置文件：`options.ini`

你可以通过编辑 `options.ini` 文件来自定义惯性参数或按键绑定。如果文件不存在，脚本会使用以下默认配置：

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


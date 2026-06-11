# DMU-Sim-online

A modified simulator of FFXIV Dancing Mad (Ultimate) phase 2 towers, forked from [WCGH/Waju-Sims DMU SIM beta v1.9](https://github.com/WCGH/Waju-Sims/releases/tag/dmu-0.1.x).

## ✨ Features

- **Localized UI** – Most settings and texts are translated into Chinese (Simplified).
- **P2P Networking (Module 1)** – Built with Godot's ENet. Requires one host with a public IP to relay positions and markers.  
  *Recommended: Use Tailscale / ZeroTier / Radmin to create a private virtual network.*
- **P2P Networking (Module 2)** – Uses Steam Remote Play Together. After the host creates a lobby, friends accept the invitation via Steam, then click "Join" inside the simulator.  
  *Please use within reasonable limits to avoid violating the EULA.*
- **Skill Simulation** – Practice ability usage (GCDs, oGCDs) during the tower mechanic to simulate real‑fight rotations and resource management.
- **Priority Markers** – Customizable markers for assigning priority, improving communication and reaction.

## ⚠️ Notes

- Bugs may exist. No further updates are planned as our static group has already cleared the phase. Feel free to fork and fix.
- For any modifications, please comply with the GPL-3.0 license.

---

# DMU-Sim-online

基于 [WCGH/Waju-Sims DMU SIM beta v1.9](https://github.com/WCGH/Waju-Sims/releases/tag/dmu-0.1.x) 的最终幻想14 绝龙诗P2塔模拟器修改版。

## ✨ 功能

- **本地化** – 大部分设置和文本已翻译为简体中文。
- **联机模块1** – 使用 Godot 的 ENet 实现 P2P 联机。需要一位有公网 IP 的玩家作为主机，收发客户端的位置与标点信息。  
  *建议搭配 Tailscale / ZeroTier / Radmin 等工具构建私有网络使用。*
- **联机模块2** – 使用 Steam 远程同乐。主机创建大厅后，好友在 Steam 内接受邀请，然后在模拟器中点击“加入”即可连线。  
  *请在合理范围内使用，避免违反 EULA。*
- **技能模拟** – 在塔机制过程中模拟技能使用（GCD、能力技等），帮助练习实战循环。
- **优先级标记** – 可自定义标点，用于分配优先级，提升沟通与反应效率。


## ⚠️ 注意

- 可能存在未知错误。由于我们固定队已通关此阶段，暂时无后续开发计划，有能力者可自行修改。
- 二次开发请遵守 GPL-3.0 协议。

---

# Waju-Sims

Download links:

DMU: https://github.com/WCGH/Waju-Sims/releases/tag/dmu-0.2.x

FRU: https://github.com/WCGH/FRU-Sim/releases/tag/v1.8

DSR: https://github.com/WCGH/Dragonsong-Sim/releases/tag/v1.1

Discord: https://discord.gg/P9adFHADrX

## Note on renderer compatability issues and running on Linux:

If the sim fails to launch or consistently crashes, it is usually a rendering issue. The sim by default runs on DX12 but you can run it on Vulkan through cmd line arguments.

For Windows users: Shift+Right click anywhere inside the folder containing dmu-sim.exe > Open PowerShell window here > Enter `./dmu-sim.exe --rendering-driver vulkan`

The same arguments should also work for Linux users running it through Wine.

Alternative for Linux Users: you can download the Linux version of the Godot engine (any 4.7 version should work). Extract the `godot_..._linux.x86_64` file and rename it to `dmu-sim` and run it in the dmu-sim folder.

If you're on a laptop with integrated GPU and neither DX12 or Vulkan works, you can also try replacing `vulkan` with `opengl3`, though you will see a big drop in performance.


If you have any questions or feedback let me know on discord.

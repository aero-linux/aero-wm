# 🦀 aero-wm — High-Performance Rust Wayland Compositor

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0b0e,100:00f2fe&height=200&section=header&text=aero--wm&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Ground-Up%20Rust%20Wayland%20Compositor%20%26%20Dynamic%20Tiler&descAlignY=62&descAlign=50" width="100%"/>

<br/>

[![Roadmap](https://img.shields.io/badge/Milestone-v2.0_Singularity-0891b2?style=for-the-badge&logo=rust&logoColor=white)](https://github.com/aero-linux/aero-wm)
[![Memory Target](https://img.shields.io/badge/RAM_Target-%3C_150_MB-3178C6?style=for-the-badge&logo=speedtest&logoColor=white)](https://github.com/aero-linux/aero-wm)
[![Smithay](https://img.shields.io/badge/Compositor-Smithay-orange?style=for-the-badge&logo=wayland&logoColor=white)](https://smithay.github.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-4EAA25?style=for-the-badge)](LICENSE)

</div>

---

### 🚀 Overview
**`aero-wm`** is the next-generation Wayland compositor being engineered for **Aero Linux v2.0 (Singularity)**. Written purely in Rust on top of the **Smithay** compositor framework, it targets an uncompromising memory footprint (< 150 MB total RAM), hardware-accelerated Direct Scanout via DRM/KMS, zero-latency frame presentation, and seamless dynamic window tiling.

### ⚡ Architectural Goals

1. **Sub-150MB Total RAM:** Zero Electron or heavy web-engine overhead in the compositor loop.
2. **Smithay & DRM/KMS Backend:** Direct render-node communication with modern AMDGPU, Intel Iris, and NVIDIA Open Kernel modules.
3. **Dynamic Tiling Engine:** Flexible binary-space-partitioning (BSP) and floating workspace management.
4. **IPC Protocol:** Unix domain socket IPC for 1-millisecond response to desktop widgets, keybinds, and CLI tools.
5. **IPC Zero-Flicker Animations:** 60/120/144Hz tear-free rendering using Vulkan / OpenGL ES 3.

---

### 🛠️ Building & Contributing

```bash
# Build the prototype (Rust toolchain required)
cargo build --release

# Run in nested Wayland session (for testing)
cargo run -- --nested
```

---

<div align="center">
  <p>Maintained by the <b><a href="https://github.com/aero-linux">Aero Linux Project</a></b> & <b><a href="https://github.com/ronitgupta138">@ronitgupta138</a></b></p>
</div>

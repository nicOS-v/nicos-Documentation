## nicos Mesa 编译文档



### 1.拉取Mesa



`git clone https://github.com/nicOS-v/mesa`

`cd mesa`



### 2.安装依赖



`apt install pkg-config build-essential meson ninja-build python3 pkg-config libdrm-dev libexpat1-dev libx11-dev libxext-dev libxdamage-dev libxfixes-dev libxshmfence-dev libxcb1-dev libxrandr-dev libudev-dev libelf-dev llvm libvulkan-dev libwayland-dev libgbm-dev libdrm-dev libdrm-amdgpu1 libelf-dev elfutils-libelf-devel byacc flex wayland-protocols libwayland-egl-backend-dev libwayland-dev libegl1-mesa-dev libxcb-glx0-dev libxcb-shm0-dev libx11-xcb-dev libxcb-dri2-0-dev libxcb-dri3-dev libxxf86vm-dev libxcb*`



### 3.编译安装

`meson setup builddir`

`cd builddir`

`ninja`

`ninja install`





备注：


这些程序包在构建和编译 Mesa 或类似的复杂图形软件包时起到关键作用。以下是每个包的作用简析：

1. **build-essential**: 包含编译软件所需的基本编译工具，如 GCC 编译器、make 工具等。
2. **meson**: 一种现代化的构建系统，用于配置、编译和安装软件。
3. **ninja-build**: 一个小型的构建系统，通常与 Meson 配合使用，用于执行构建命令。
4. **python3**: Python 编程语言的最新版本，用于执行一些构建脚本和工具。
5. **pkg-config**: 一个帮助程序，用于在编译过程中定位和配置软件包的元数据。
6. **libdrm-dev**: Direct Rendering Manager (DRM) 的开发文件，用于底层图形操作。
7. **libexpat1-dev**: Expat XML 解析库的开发文件。
8. **libx11-dev**: X11 客户端库的开发文件，用于基本的 X Window 系统交互。
9. **libxext-dev**: X11 扩展库的开发文件。
10. **libxdamage-dev**: X 服务器的 Damage 扩展库的开发文件。
11. **libxfixes-dev**: X 服务器的修复扩展库的开发文件。
12. **libxshmfence-dev**: 用于 X 服务器的共享内存围栏的开发文件。
13. **libxcb1-dev**: X11 的 C 语言接口库 XCB 的开发文件。
14. **libxrandr-dev**: X11 RandR 扩展库的开发文件，用于屏幕大小、方向和反射的设置。
15. **libudev-dev**: udev 库的开发文件，用于 Linux 的设备管理。
16. **libelf-dev**: 用于处理 ELF (Executable and Linkable Format) 文件的开发文件。
17. **llvm**: 编译器和工具链技术的集合，用于构建 Mesa 的某些部分。
18. **libvulkan-dev**: Vulkan 图形和计算 API 的开发文件。
19. **libwayland-dev**: Wayland 协议的开发文件，用于现代图形堆栈。
20. **libgbm-dev**: 通用缓冲管理器 (GBM) 的开发文件。
21. **libdrm-amdgpu1**: AMD GPU 的 DRM 库，用于 AMD 图形硬件。
22. **elfutils-libelf-devel**: 用于处理 ELF 文件的工具和库，特别是在 Fedora、Red Hat 或 CentOS 上。
23. **byacc**: Berkeley Yacc，用于生成解析器。
24. **flex**: 快速词法分析器生成器，用于生成扫描器。
25. **wayland-protocols**: Wayland 协议的规范和扩展。
26. **libwayland-egl-backend-dev**: Wayland EGL 后端的开发文件。
27. **libegl1-mesa-dev**: Mesa EGL 库的开发文件。
28. **libxcb-glx0-dev**: XCB 的 GLX 扩展的开发文件。
29. **libxcb-shm0-dev**: XCB 的共享内存扩展的开发文件。
30. **libx11-xcb-dev**: X11 和 XCB 之间的接口库的开发文件。
31. **libxcb-dri2-0-dev**: XCB 的 DRI2 扩展的开发文件。
32. **libxcb-dri3-dev**: XCB 的 DRI3 扩展的开发文件。
33. **libxxf86vm-dev**: XFree86-VidModeExtension 库的开发文件，用于视频模式设置。
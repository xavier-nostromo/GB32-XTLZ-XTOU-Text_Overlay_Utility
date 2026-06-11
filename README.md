# XTOOL Type Overlay Util (RichEdit Native PopUp Version)

An advanced, hardware-accelerated style on-screen display (OSD) text overlay utility built for **GFA-BASIC 32 (GB32)**. It features strict window transparency masking, dynamic sizing, and selection-based text alignment control powered by native Win32 API hooking and GB32's built-in context menus.

---

## 🚀 Features

* **Native Rich Text Rendering:** Leverages an OCX RichEdit control for high-fidelity text presentation using customizable typography (`Cyberverse`).
* **Dual-Layer Translucency:** Utilizes layered window composition to render an interactive, vibrant text layer perfectly over a dim, transparent base background.
* **Context-Driven Text Alignment:** Features an integrated native context menu (`PopUp`) triggered on right-click to instantly shift text layouts (`Left`, `Center`, `Right`).
* **Global Message Hooking:** Captures precise hardware input events—such as real-time text scaling via the mouse wheel (`WM_MOUSEWHEEL`)—without intercepting the foreground focus chain.
* **Safe Windows Subclassing:** Fully custom Window Procedures (`WndProc`) that bypass traditional activation patterns to keep the interface non-intrusive yet responsive.

---

## 🛠️ Controls & Hotkeys

| Action | Control Shortcut | Behavior |
| :--- | :--- | :--- |
| **Align Left** | `Ctrl + L` / Right-Click Menu | Align selected text to the left margin. |
| **Align Center** | `Ctrl + E` / Right-Click Menu | Horizontally center selected text. |
| **Align Right** | `Ctrl + R` / Right-Click Menu | Align selected text to the right margin. |
| **Scale Font Size** | `Mouse Wheel Up / Down` | Dynamically scale font size between `8pt` and `200pt`. |
| **Graceful Exit** | `Escape` or `Ctrl + Break` | Unhooks hooks, un-subclasses windows, and exits safely. |

---


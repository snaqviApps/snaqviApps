## Sayyid A. Naqvi

<!--
**snaqviApps/snaqviApps** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

-->

<br>



## 🛠 Technical Ecosystem

| Category | Stack |
| :--- | :--- |
| **Languages** | Kotlin, Java, C++, Python |
| **Frameworks** | Jetpack Compose, Compose Multiplatform, KMP SDK |
| **Architecture** | MVVM, Clean Architecture, Nav3 |
| **DI & Networking** | Constructor Injection, OkHttp, Retrofit, Ktor |
| **Storage/Cloud** | Firebase, Firestore, Room |
<br>
<br>

## 🚀 Featured Projects

### <img width="35" height="32" alt="PCI Monitor Icon" src="https://github.com/user-attachments/assets/9df66119-ce5b-4eb7-a46a-8618df504759" align="absmiddle" style="vertical-align: middle; margin-right: 8px;" /> PCI Monitor

* **`PCI_Monitor`**: Master umbrella repository coordinating a real-time PCIe hardware telemetry and diagnostics architecture.
* **`pci-diagnostics` (Backend)**: Native C++ core that queries Linux `sysfs` registers and exports optimized interop functions compiled into a shared `.so` library.
* **`KMP-FrontEnd` (UI)**: Kotlin Multiplatform client utilizing JNA and Jetpack Compose to render live multi-device telemetry tables across Desktop and Android environments.

  [View Repository](https://github.com/snaqviApps/PCI_Monitor.git)
<br>
<br>

### 🖼️ SharedVault: Multi-User Gallery (KMP)
*A secure, cross-platform image sharing solution for private groups.*

*   **Tech:** Kotlin Multiplatform (KMP), Firebase Storage, Firestore
*   **Secure Auth:** Implements a **Custom OkHttp Authenticator** to handle JWT 401/403 error flows and automated token refresh logic.
*   **Networking:** Utilizes Ktor for multiplatform API requests and shared business logic across Android and iOS.
*   **Storage:** To handle ~25 concurrent users with real-time Firestore synchronization and Firebase Storage access rules.
<br>

### 🎬 Custom Android NDK Video Engine (C++ / JNI / ExoPlayer)
* Engineered a high-performance, zero-copy video decoding pipeline bridging AndroidX Media3 (ExoPlayer) with native C++ hardware decoders*

*  **Zero-Copy GPU Rendering:** Bound native AMediaCodec instances directly to Android Surface (ANativeWindow) components via JNI, achieving 60fps
   playback with zero CPU overhead for YUV-to-RGB pixel conversion.
   
*  **Precision Synchronization:** Implemented strict 8-byte memory alignment in C++ to extract and pass 64-bit hardware
   timestamps (presentationTimeUs) up to Kotlin, locking native frame rendering perfectly to ExoPlayer's master audio clock.
   
*  **Dynamic Playback Control:** Bridged ExoPlayer's internal buffer states to native C++ commands, executing real-time hardware memory
   flushes for zero-latency timeline scrubbing and instant seek recovery.

*  **Resilient Memory Management:** Designed a robust C++ buffer recycling architecture that securely manages ExoPlayer's 16-frame
   maximum memory pool, preventing hardware starvation, memory leaks, and MediaServer double-free corruptions.

     
   [View Project](https://github.com/snaqviApps/MoviesApp)




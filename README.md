# Godot NVDA Integration

As of 2024, the latest package for integrating NVDA support into Godot seems to be https://github.com/lightsoutgames/godot-tts. However, from speaking to the author on Discord, I understood that this is no longer going to be maintained.

Ergo, as a sighted developer, I need a quick-and-easy way to integrate NVDA with Godot, so that I can send NVDA texts to read; this provides the best-case for usability for blind users and users who depend on screen readers.

The current code is based on a hastily-thrown-together example from @bruvzg, circa 2023, which you can find here: https://github.com/godotengine/godot-proposals/discussions/6757#discussioncomment-5722559

I attempted to adapt and maintain the code for Godot 4.2.1 in 2024, and going forward.

# Development Instructions

Same as https://github.com/godotengine/godot-cpp; namely:

- Install Scons (`pip install scons`)
- Install MSYS2
- Install MinGW-w64
- Install the toolchain

See [Getting Started with C++ And MingW-64 in Visual Studio Code](https://code.visualstudio.com/docs/cpp/config-mingw#_installing-the-mingww64-toolchain) for detailed, up-to-date instructions

Once that's done:

- Build `godot-cpp`
- Move this directory so it's a subdirectory of `godot-cpp`
- From the root directory of this project, run `scons`
- Wait. A long, long time.
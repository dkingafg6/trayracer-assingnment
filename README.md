# Trayracer Assignment

This project is based on the [trayracer](https://github.com/fLindahl/trayracer) repository.  
It is modified and optimized for a university assignment involving profiling, optimization, and multithreaded rendering.

## 🛠 Features Implemented

- **Single-frame render** without OpenGL or user interface.
- **Command-line arguments** for customizable rendering:
  - Image width
  - Image height
  - Rays per pixel
  - Number of spheres
- **Custom random number generator** implemented (xorshift).
- **Performance measurement**:
  - Time taken to render
  - Total rays traced
  - MRays/s (Million Rays per second)
- **Memory leak fixes** and **compiler warnings** cleaned.
- **Multithreaded rendering** (CPU parallelization).
- **Optimization** through profiling and memory improvements.
- **LaTeX report** documenting all profiling and optimization steps.

## 🧩 Build Instructions

Requires:
- GCC 9+ or Clang 10+
- CMake 3.15+
- Ninja
- OpenGL & X11 libraries (for compilation only)

Build with:

```bash
cd ~/raytracer
mkdir -p build
cd build
cmake -G Ninja ..
ninja

# Change Log

## v0.2.3 (20-03-2019)
  - fixed vertex format mapping
  - fixed building with "empty" backend on Windows
  - bumped the default descriptor pool size
  - fixed host mapping aligments
  - validating the uniform buffer offset

## v0.2 (06-03-2019)
  - Platforms: iOS/Metal, D3D11
  - Crates:
    - `wgpu-remote`: remoting layer for the cross-process boundary
    - `gfx-examples`: selected gfx pre-ll examples ported over
  - Features:
    - native example for compute
    - "gfx-cube" and "gfx-shadow" examples
    - copies between buffers and textures
    - separate object identity for the remote client
    - texture view tracking
    - native swapchain resize support
    - buffer mapping
    - object index epochs
    - comprehensive list of vertex and texture formats
    - validation of pipeline compatibility with the pass
  - Fixes
    - fixed resource destruction

## v0.1 (24-01-2019)
  - Platforms: Linux/Vulkan, Windows/Vulkan, D3D12, macOS/Metal
  - Crates:
    - `wgpu-native`: C API implementation of WebGPU, based on gfx-hal
    - `wgpu-bindings`: auto-generated C headers
    - `wgpu`: idiomatic Rust wrapper
    - `examples`: native C examples
  -  Features:
    - native examples for triangle rendering
    - basic native swapchain integration
    - concept of the storage hub
    - basic recording of passes and command buffers
    - submission-based lifetime tracking and command buffer recycling
    - automatic resource transitions

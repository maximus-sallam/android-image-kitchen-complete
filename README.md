# Android Image Kitchen - Complete Kernel/Recovery Image Toolkit

This repository is a comprehensive toolkit for Android developers, combining the functionality of AIK-Linux v3.8 with Android-Image-Kitchen. It provides a robust set of tools for unpacking and repacking Android kernel and recovery images, along with the ramdisks. This merge restores essential files removed in previous versions, ensuring compatibility and enhancing the utility of Android-Image-Kitchen.

## Contents
- `README.md`: Documentation for using the toolkit.
- `bin/`: Executable binaries and scripts supporting various platforms including Linux, macOS, and utilities for handling boot and recovery images.
- `cleanup.sh`: Script to clean up the working directory.
- `repackimg.sh`: Script to repack the image after modifications.
- `unpackimg.sh`: Script to unpack the image for modification.

### Bin Directory Structure
- `androidbootimg.magic`, `avb/`, `boot_signer.jar`, `chromeos/`, `linux/`, `macos/`, `magic`: Core components and utilities for image processing.
- `avb/`: Contains keys and certificates for Android Verified Boot (AVB).
- `chromeos/`: Tools and keys for Chrome OS image signing.
- `linux/`, `macos/`: Platform-specific binaries for image manipulation, including tools for packing, unpacking, and modifying boot images.

#### Platform-specific Binaries
- **Linux**: Supports `i686` and `x86_64` architectures, including utilities like `mkbootimg`, `unpackbootimg`, `lz4`, and more for image processing.
- **macOS**: Supports `i386` and `x86_64` architectures, equipped with macOS-specific versions of the tools available for Linux, in addition to macOS-specific utilities like `cpio`, `dd`, `file`, and more.

## Usage
To begin using the toolkit:
1. Clone this repository to your local machine.
2. Ensure executable permissions are set for the scripts in the `bin/` directory.
3. Use `unpackimg.sh` to unpack an image, then modify it as needed.
4. After modifications, use `repackimg.sh` to repack the image.
5. Use `cleanup.sh` to clean up your working directory post-processing.

This toolkit is designed to streamline the workflow for Android kernel and recovery image developers, providing a versatile and powerful set of tools for image processing. For detailed usage of each script and tool, refer to the script comments or execute them with the `--help` flag for usage instructions.

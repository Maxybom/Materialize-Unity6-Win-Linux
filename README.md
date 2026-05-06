# Materialize - Unity 6 Port (Windows & Linux)

Materialize port for Unity 6 - Compatible with Windows and Linux. Full FreeImage support included.

## Acknowledgments
This is a port of the original **Materialize** project created by **Bounding Box Software**. All core features, UI, and original concepts belong to them. 
* **Original Repository:** [BoundingBoxSoftware/Materialize](https://github.com/BoundingBoxSoftware/Materialize/releases)
* **Official Website:** [Bounding Box Software](https://boundingboxsoftware.com/materialize/)

## Features & Fixes in this Port
* **Unity 6 Upgraded:** Project fully migrated and tested on Unity 6 (6000.3.12f1).
* **Cross-Platform:** Native support for both Windows and Linux environments. Natively tested on Ubuntu and Arch Linux, while the Windows version was successfully tested via Lutris/Wine.
* **FreeImage Stability:** Unlike other Linux ports that completely remove FreeImage to bypass compatibility bugs, this version retains full library support. We implemented specific fixes to handle .tif/.tiff metadata issues that previously caused Segmentation Faults on Linux, ensuring absolute stability without sacrificing the original features.

## Requirements and Tested Systems
* **Unity Engine:** Version 6000.3.12f1 or compatible version.
* **OS:** Windows 10/11 (64-bit) or Linux (Ubuntu/Arch).

## Getting Started
1. Clone or download this repository.
2. Open **Unity Hub**.
3. Click on **Add** -> **Add project from disk** and select the downloaded folder.
4. Open the Main scene (if not loaded automatically) and press Play.

## Known Issues
* **.TIF Previews:** Due to internal library limitations in the Unity 6 port, .tif files do not display a visual preview in the UI.
* **Memory Management (.tif):** When processing .tif files, you may notice a memory leak. This is a deliberate stability workaround implemented to prevent the application from crashing during heavy texture processing.
    * **Note:** If you are working with a large number of .tif files, it is recommended to restart the application periodically to clear the memory.

## License
This project is licensed under the **GNU General Public License v3.0 (GPL-3.0)**, strictly inheriting the original project's license constraints. See the LICENSE file for more details.

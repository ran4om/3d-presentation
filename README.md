# 3D presentation

[Download the presentation package](https://github.com/ran4om/3d-presentation/releases/latest)


An animated accounting presentation about low-value assets and fixed assets, with 26 content slides and 50 embedded camera-transition clips.

## Download and open

Extract the ZIP completely. Open 3D_Presentation.pptx in desktop Microsoft PowerPoint for Windows and start the slide show with F5. The videos are embedded in the presentation.

## Navigate the 3D tour

The main deck uses a custom phone remote to select sections and play the camera transitions. Ordinary next/previous slide clicks do not follow the intended tour order.

1. Install Python 3.11 or 3.12 with the Windows Python launcher, and install Tailscale on the presenting PC and phone.
2. Connect both devices to your own Tailscale network.
3. Start the PowerPoint slide show, then run remote/start-tailscale-windows.bat. The first launch creates a Python environment and installs the dependencies listed in remote/requirements.txt.
4. Open the newly generated phone link or scan the newly generated QR code. Each launch creates a fresh pairing key.
5. Keep the remote running while presenting. Closing it stops its Tailscale Serve session. The launcher stops if it detects a conflicting Serve setup on HTTPS port 443.

To browse the content manually, use the PowerPoint slide navigator to select slides 1 through 26. Transition clips occupy slides 27 through 76. See slide_map.md for the mapping. Browser previews and other presentation apps may not reproduce the animations and controls.

## Public copy

This package contains the main 3D deck only. It excludes the linear/clicker version, saved pairing QR codes, local Python environments, caches, and temporary Office files. Document author metadata, printer settings, the document preview thumbnail, and hidden PNG source-path/render metadata have been removed. Slide content, animations, and embedded videos are preserved.

## Credits

3D: Blender. Models: Poly Haven (CC0), "VW Passat Variant B5" by KrStolorz and "Tesla M3 model" by wintrez (Sketchfab, CC BY). Original on-slide credits remain in the presentation.

# nkwine

nkwine is a launcher that runs NinjaKernel, the Roblox executor, on Linux.

NinjaKernel only ships for Windows. nkwine builds a wine prefix, works around the wine
bugs that stop it running, installs NinjaKernel from its own installer, and launches it.
Clipboard, mouse lock and native file dialogs work in-app.

## Install

    curl -fsSL https://raw.githubusercontent.com/Ring0lw/nkwine/main/install.sh | sh

Or download the AppImage from the releases page and chmod +x it.

## Use

Put NinjaKernel Setup.exe in ~/Downloads (get it from https://ninjakernel.dev), then:

    nkwine

The first run downloads Proton, builds the prefix and unpacks NinjaKernel, so give it a
minute. After that it goes straight to launching.

    nkwine status      what is set up and what is running
    nkwine kill        close NinjaKernel and Roblox
    nkwine uninstall   remove the prefix

## Needs

A Vulkan GPU, python3, and about 7 GB free. Uses GE-Proton from Steam if it is there,
downloads its own otherwise.

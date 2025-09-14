# Info

- 2025.09.14 Update Electron v38.1.0

# Requirements
- node.js
- npm

# Build instructions
```
npm install
npm install @electron/packager --save-dev
npx @electron/packager --overwrite . ctbrec-minimal-browser
```
This builds the browser for your current OS. If you want to build for other platforms you can use additional switches. Available platforms are
linux, win32, darwin. For example macos 64bit:
```
npx @electron/packager --overwrite . ctbrec-minimal-browser --platform=win32 --arch=x64 --icon=icon.png
npx @electron-packager --overwrite . ctbrec-minimal-browser --platform=linux --arch=x64 --icon=icon.png
npx @electron-packager --overwrite . ctbrec-minimal-browser --platform=darwin --arch=x64 --icon=icon.icns
```
<img width="195" alt="ef_m_dk" src="https://github.com/user-attachments/assets/022cc324-97a9-4243-9207-a897c58055ff" />


# EF CubeSat Ground Terminal V1

A desktop application for CubeSat ground station control and monitoring, built with Electron.js.

## Description

EF CubeSat Ground Terminal is a comprehensive desktop application designed for controlling and monitoring CubeSat ground stations. The application provides a modern interface for satellite tracking, data visualization, and serial communication with ground station hardware.

## Features

- Real-time satellite tracking and visualization using Three.js
- Serial port communication for ground station hardware control
- WebSocket-based real-time data updates
- Cross-platform support (Windows, Linux)
- Modern and intuitive user interface

## Prerequisites

Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14.0.0 or higher)
- npm (usually comes with Node.js)
- Git

## Installation

1. Clone the repository:
```bash
git clone https://github.com/edgeflyte/CubeSat-Ground-Station-Software-v1.git
cd CS-Ground-Terminal
```

2. Install dependencies:
```bash
npm install
```

## Development

To run the application in development mode:
```bash
npm start
```

## Building the Application

### For all platforms:
```bash
npm run make
```

### For specific platform builds:
```bash
npm run build
```

The built applications will be available in the `out` directory.

## Project Structure

```
CS-Ground-Terminal/
├── dist/               # Distribution files
├── build/             # Build resources
├── css/               # Stylesheets
├── js/                # JavaScript modules
├── img/               # Image assets
├── models/            # 3D models
├── index.js           # Main electron process
├── main.html         # Main application window
└── preload.js        # Electron preload script
```

## Dependencies

### Main Dependencies
- electron: Desktop application framework
- three.js: 3D visualization
- socket.io: Real-time communication
- serialport: Hardware communication
- express: Web server framework

### Dev Dependencies
- @electron-forge/cli: Build tooling
- @electron-forge/maker-deb: Linux .deb packaging
- @electron-forge/maker-rpm: Linux .rpm packaging
- @electron-forge/maker-squirrel: Windows installer
- @electron-forge/maker-zip: ZIP packaging

## Scripts

- `npm start`: Run the application in development mode
- `npm run package`: Package the application
- `npm run make`: Build the application for distribution
- `npm run build`: Build using electron-builder

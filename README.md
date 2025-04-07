# HBC WebGL - Homebrew Channel Banner Animation

A pixel-perfect recreation of the Nintendo Wii Homebrew Channel banner animation using WebGL and modern web technologies.

![HBC WebGL Banner](hbc-webgl-screenshot.png)

## Overview

This project recreates the iconic banner animation and audio from the Homebrew Channel (HBC) - one of the most famous custom channels for the Nintendo Wii. It faithfully reproduces all visual elements, including:

- The flowing water effect
- Particle bubbles with authentic generation patterns
- Wave animations with precise timing
- The signature flash effect
- Original HBC logo and transitions

The animation is rendered using WebGL shaders that mirror the same rendering techniques used in the original Wii implementation.

## Motivation

I was always obsessed with the clean animation and signature soundtrack of the Homebrew Channel. The animation combined simple visual elements into a cohesive, calming experience that perfectly matched the channel's aesthetic. Porting it to the web was a fun challenge that allowed me to both preserve this piece of Wii homebrew history and learn more about how the original animations were created.

## Features

- **Authentic Animation**: Directly based on the original banner generation code from the HBC source
- **Precise Audio Synchronization**: The music is accurately synchronized with animation keyframes
- **Interactive Controls**: Play, pause, reset, and jump to specific animation points
- **Frame-Perfect Loop**: Seamless animation looping matching the original
- **Bubble System**: Accurate recreation of the bubble generation system with the same seeded random function

## Technical Implementation

The animation system is a complete translation of the original HBC banner generation code from Python/OpenGL to JavaScript/WebGL:

- Hermite spline interpolation for smooth animations
- Material system with custom texture wrapping modes
- Texture coordinate transformations matching the original
- WebGL shaders that replicate the original rendering pipeline
- Precise frame timing at 60fps to match the Wii's display rate

## Usage

1. Run a web server in the project's root directory and navigate to the local address in a modern browser (e.g., using `python -m http.server` or any other web server of your choice)
2. Use the controls to interact with the animation:
   - **Play**: Start the animation and audio
   - **Pause**: Freeze the animation and stop audio
   - **Reset**: Return to the beginning
   - **Jump to Bubbles**: Skip to the bubble burst effect

Keyboard shortcuts:
- **Space**: Toggle play/pause
- **R**: Reset animation

## Requirements

- A browser with WebGL support
- Audio capability for the full experience

## Asset Credits

This project uses the following assets from the original Homebrew Channel:
- Animation timing and layout from the `mkbanner.py` script
- Audio extracted from the original Homebrew Channel
- Rendering techniques took from the `Alameda.py` script

## Original Homebrew Channel Credits

The Homebrew Channel was developed by Team Twiizers (later known as fail0verflow). All original design and asset credits belong to them.

Original repository: https://github.com/fail0verflow/hbc

## License

This project is provided for educational and historical preservation purposes. All original Homebrew Channel assets and designs remain under their original licenses.
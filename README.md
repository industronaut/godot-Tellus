# Tellus

A Godot 4.4+ plugin for creating procedural tiled 3D maps.

## Overview

Tellus is a GDExtension plugin that provides tools for generating procedural 3D tiled maps in Godot. Whether you're building dungeon crawlers, strategy games, or open-world environments, Tellus helps you create dynamic and interesting 3D terrain using tile-based generation.

## Features

- **Procedural Generation**: Create diverse 3D maps using algorithmic generation
- **Tile-Based System**: Build maps using modular tile components
- **Godot 4.4+ Compatible**: Built as a native GDExtension for optimal performance
- **Cross-Platform**: Supports Linux, Windows, macOS, and Web platforms

## Requirements

- Godot 4.4 or later
- Compatible with Linux, Windows, macOS, and Web platforms

## Installation

### From Releases

1. Download the latest release from the [Releases](https://github.com/industronaut/godot-Tellus/releases) page
2. Extract the contents to your project's `addons/` folder
3. Enable the plugin in your project settings

### Building from Source

1. Clone the repository with submodules:

   ```bash
   git clone --recursive https://github.com/industronaut/godot-Tellus.git
   cd godot-Tellus
   ```

2. Build the extension:

   ```bash
   scons target=template_debug
   ```

3. Copy the built extension to your project:
   ```bash
   cp -r demo/addons/tellus /path/to/your/project/addons/
   ```

## Usage

1. Enable the Tellus plugin in your project settings
2. Add a Tellus node to your scene
3. Configure the generation parameters
4. Generate your procedural 3D map

## Development

### Building

This project uses SCons for building. The build system supports multiple platforms and configurations:

```bash
# Debug build for current platform
scons target=template_debug

# Release build
scons target=template_release

# Editor build
scons target=editor

# Specify platform and architecture
scons target=template_debug platform=linux arch=x86_64
```

### Supported Platforms

- Linux (x86_64)
- Windows (x86_64)
- macOS (Universal)
- Web (WebAssembly)

### Code Style

This project uses pre-commit hooks for code formatting and quality checks. Install and set up pre-commit:

```bash
pip install pre-commit
pre-commit install
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. Make sure to:

- Follow the existing code style
- Run pre-commit hooks before submitting
- Test your changes across different platforms when possible

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with [godot-cpp](https://github.com/godotengine/godot-cpp)
- Inspired by the Godot community's need for better procedural generation tools

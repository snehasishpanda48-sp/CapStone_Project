# File Explorer Application

A comprehensive console-based file explorer application in C++ that provides file management, navigation, and file operations for Linux systems.

## Features

### Core Functionality
- **Directory Listing**: View files and directories with detailed information (permissions, size, type, modification time). Toggle hidden files view with `hidden`.
- **Navigation**: Advanced navigation with history (`back`, `forward`), bookmarks (`bookmark`, `goto`, `unmark`), and quick navigation commands.
- **File Operations**: Copy (`cp`), move (`mv`), delete (`rm`), create files (`touch`) and directories (`mkdir`).
- **Disk Usage**: View disk space usage with `du`.
- **Interactive Interface**: User-friendly command-line interface with a built-in help system.

### Available Commands

#### Navigation Commands
- `ls`, `list` - List current directory contents
- `cd [path]` - Change directory (`cd ..` to go up, `cd ~` for home, `cd -` for previous)
- `back` - Go back in navigation history
- `forward` - Go forward in navigation history
- `pwd` - Print current directory path

#### Bookmark System
- `bookmark [name]` - Bookmark current directory
- `goto [name]` - Go to bookmarked directory
- `unmark [name]` - Remove bookmark
- `bookmarks` - Show all bookmarks
- `history` - Show navigation history

#### File Operations
- `cp [source] [destination]` - Copy files/directories
- `mv [source] [destination]` - Move/rename files/directories
- `rm [path]` - Delete files/directories
- `mkdir [path]` - Create a new directory
- `touch [file]` - Create an empty file
- `du [path]` - Show disk usage of a path or current directory

#### Display Options
- `hidden` - Toggle hidden files display
- `help`, `?` - Show available commands
- `exit`, `quit` - Exit application

## Building the Application

### Prerequisites
- C++17 compatible compiler (GCC, Clang)
- CMake 3.10 or higher
- Linux operating system (or WSL on Windows)

### Build Instructions

```bash
# Clone or download the project
cd Wipro_Capstone_Project_4

# Create build directory
mkdir build
cd build

# Configure with CMake
cmake ..

# Build the project
make

# Run the application
./bin/file_explorer
```

## Usage Examples

### Basic Navigation
```
File Explorer> ls                    # List current directory
File Explorer> cd Documents          # Change to Documents directory
File Explorer> cd ..                 # Go to parent directory
File Explorer> bookmark docs         # Bookmark current directory as "docs"
File Explorer> goto docs             # Go to bookmarked directory
```

### File Operations
```
File Explorer> cp file.txt backup/   # Copy file to backup directory
File Explorer> mv old.txt new.txt    # Rename file
File Explorer> mkdir new_folder      # Create new directory
File Explorer> touch new_file.txt    # Create empty file
File Explorer> du .                  # Show disk usage of current directory
```

## System Requirements

- **Operating System**: Linux (Ubuntu 18.04+, CentOS 7+, etc.) or Windows with WSL
- **Compiler**: GCC 7+ or Clang 6+ with C++17 support
- **Permissions**: Read access to directories you want to explore, write access for file operations

## License

This project is part of a Wipro capstone project and is intended for educational purposes.

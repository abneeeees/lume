# Lume

A lightweight, terminal-based peer-to-peer (P2P) chat application written in C.

## Features

- **P2P Communication**: Direct messaging between peers using TCP/IP.
- **Automatic Discovery**: Local network peer discovery via UDP beacons.
- **Terminal UI**: Interactive interface built with `ncurses`.
- **File Transfer**: Support for sending and receiving files over the network.

## Requirements

- GCC
- Make
- ncurses library
- pthread library

## Installation

### Quick Install (Debian/Ubuntu)

1. Download the latest `lume.deb` package from the [Releases](https://github.com/jorgegarcia33/lume/releases) section.
2. Install the package using:
   ```bash
   sudo apt install ./lume.deb
   ```
3. Launch the application:
   ```bash
   lume <username> <port>
   ```

### Build from Source

If you prefer to build the project manually:

```bash
make
sudo make install
```

## Usage

```bash
lume <username> <port>
```

### Controls & Commands

Once inside the application, you can use the following controls:

- **Arrow Keys (Up/Down)**: Cycle through the list of discovered peers in the network.
- **Type & Enter**: Send a text message to the currently selected peer.
- **`/file <path>`**: Send a file to the selected peer (e.g., `/file ./document.txt`).
- **ESC**: Exit the application.

## Project Structure

- `src/`: Source code files (`.c`).
- `include/`: Header files (`.h`).
- `bin/`: Compiled executable.
- `obj/`: Object files.

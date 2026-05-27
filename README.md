# Multi-Threaded Server-Client Tic-Tac-Toe

An end-to-end network programming project utilizing Python sockets and multi-threading to facilitate concurrent multiplayer Tic-Tac-Toe matches.

## Overview
This project explores networked game development by implementing a centralized server that acts as a hub for game logic and player coordination. It manages the state of the game board, enforces rules, and handles the initiation of games by connecting pairs of clients into single matches. By combining a multi-threaded server architecture with dual client interfaces (CLI and GUI), it demonstrates a scalable and responsive approach to real-time client-server communication.

## Project Structure
- `ttt_server.py`: The multi-threaded TCP/IP server script managing connections, player matching, and game states.
- `ttt_client.py`: The lightweight command-line interface client for terminal-based gameplay.
- `ttt_client_gui.py`: The graphical user interface client built with Tkinter.
- `ttt_server.log`: Server execution and event logs tracking connections and game terminations.
- `ttt-service.conf`: Upstart configuration file for deploying the server as a background service.
- `Tic-tac-toe game with server-client architecture.pdf`: Academic project specifications and requirements.

## Key Phases
1. **Server Development:** Engineered a multi-threaded server using the `socket` and `threading` libraries to accept simultaneous incoming connections and match players asynchronously without bottlenecking the main process.
2. **Game Logic Integration:** Centralized the Tic-Tac-Toe rules engine on the server to validate moves, track board states, and accurately transmit each move to the appropriate opponent.
3. **Client Interface Design:** Developed a user-friendly graphical user interface (GUI) alongside a command-line interface (CLI) to capture player moves, render the board, and handle network communications smoothly.

## Key Technologies
- **Python:** Core programming language for logic and network implementation.
- **Sockets:** TCP/IP networking interface for client-server data transmission.
- **Threading:** Multi-threaded concurrency for handling multiple game sessions simultaneously.
- **Tkinter:** Native Python GUI development for interactive client rendering.
- **Upstart:** Linux service management for background execution.

## Metrics & Findings
| Metric | Value |
| :--- | :--- |
| **Architecture** | Multi-threaded Client-Server |
| **Protocol** | TCP/IP Sockets |
| **Concurrency Model** | Thread-per-Client |
| **GUI Framework** | Tkinter |

## Author
**Sepehr Barekati**

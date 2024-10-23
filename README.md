# RemoteIT System

RemoteIT System is a multithreaded remote desktop application that allows clients to authenticate, control the desktop, chat, and transfer files, all implemented using TCP sockets without any networking libraries.

## Features

- **Authentication**: Random password generated for each session.
- **Remote Desktop Control**: View and control the desktop with mouse and keyboard.
- **Chat**: Real-time chat between client and remote machine.
- **File Transfer**: Transfer files between systems (In progress).
- **Multiple Connection Options**: Connect using LAN, WAN, or via ngrok.
- **Event Logs**: Track connection status and user actions.
- **Performance Optimization**: In-memory operation, screen compression, and background optimization.

## Tech Stack

- **Backend**: Python 3.7
- **GUI**: Tkinter

## Getting Started

### Prerequisites
- Python 3.8+
- Virtual Environment (optional but recommended)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/adarshsingh26/RemoteITSystem.git
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv myenv
    myenv\Scripts\activate  # Windows
    ```

3. Install required modules:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the server or client:
    - For server:
      ```bash
      python server.py
      ```
    - For client:
      ```bash
      python client.py
      ```

## How It Works

- **Server**: Listens for connections, streams the desktop, and simulates mouse/keyboard events.
- **Client**: Authenticates with the server, views the remote desktop, and sends mouse/keyboard inputs.

## To-Do

- Complete file transfer feature.
- Add UPnP support.
- Add custom file manager UI.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

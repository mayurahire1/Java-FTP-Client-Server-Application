# 🚀 Java FTP Client-Server Application

A Java-based FTP-style file transfer application developed using **Socket Programming**. It follows a client-server architecture and allows users to transfer and manage files over a network.

## 📌 Project Overview

This project implements a client-server file transfer system using Java TCP Socket Programming.

The server listens for incoming client connections on port **9000**. Clients can connect to the server and perform different file management operations, such as uploading, downloading, renaming, deleting, and viewing files.

The server uses **Multithreading** to handle multiple client connections simultaneously.

## ✨ Features

- **LIST** – Display all files available on the server.
- **EXISTS** – Check whether a file exists on the server.
- **INFO** – Display file information, including name, size, readability, and writability.
- **SIZE** – Get the size of a file in bytes.
- **GET** – Download files from the server to the client.
- **PUT** – Upload files from the client to the server.
- **RENAME** – Rename an existing file on the server.
- **DELETE** – Delete a file from the server.
- **QUIT** – Disconnect from the server.

## 🛠️ Technologies Used

- Java
- Java Socket Programming
- TCP Networking
- ServerSocket and Socket
- DataInputStream and DataOutputStream
- FileInputStream and FileOutputStream
- Multithreading
- Java I/O

## 🏗️ Project Architecture

```text
             FTP CLIENT
             (Client.java)
                  |
                  |
           Socket Connection
              Port: 9000
                  |
                  |
             FTP SERVER
             (Server.java)
                  |
                  |
            File Management
                  |
                  |
             Server Storage
```

## 📂 Project Structure

```text
Java-FTP-Client-Server/
│
├── Client.java       # FTP Client
├── Server.java       # FTP Server
│
└── README.md
```

## ⚙️ Installation and Setup

### Prerequisites

- JDK 17 or later
- Terminal / Command Prompt
- Basic knowledge of Java

### Step 1: Clone the Repository

```bash
git clone https://github.com/mayurahire1/Java-FTP-Client-Server.git
```

### Step 2: Navigate to the Project Directory

```bash
cd Java-FTP-Client-Server
```

### Step 3: Compile the Java Programs

```bash
javac Server.java Client.java
```

### Step 4: Start the FTP Server

Open the first terminal:

```bash
java Server
```

The server will start listening on port `9000`.

### Step 5: Start the FTP Client

Open another terminal:

```bash
java Client
```

The client will connect to the server.

## 💻 Available FTP Commands

| Command | Description |
|---|---|
| `LIST` | Display server files |
| `EXISTS Demo.txt` | Check file existence |
| `INFO Demo.txt` | Display file information |
| `SIZE Demo.txt` | Display file size |
| `GET Demo.txt` | Download a file |
| `PUT Demo.txt` | Upload a file |
| `RENAME Demo.txt DemoNew.txt` | Rename a file |
| `DELETE Demo.txt` | Delete a file |
| `QUIT` | Disconnect from server |

## 📥 File Transfer Examples

### Download a File

```text
GET Demo.txt
```

The downloaded file will be saved on the client as:

```text
Download_Demo.txt
```

### Upload a File

```text
PUT Sample.txt
```

The file will be transferred from the client to the server.

## 🧠 Concepts Learned

- Client-Server Architecture
- TCP Socket Communication
- Java Networking
- File Handling and File Transfer
- Multithreading
- Input/Output Streams
- Exception Handling
- Network Communication

## 🔮 Future Enhancements

- Add user authentication.
- Implement secure file transfer.
- Add a graphical user interface (GUI).
- Support directory management.
- Display file transfer progress.
- Add file transfer error recovery.

## 👨‍💻 Author

**Mayur Kishor Ahire**

- GitHub: [mayurahire1](https://github.com/mayurahire1)
- LinkedIn: [Mayur Ahire](https://www.linkedin.com/in/mayur-ahire1/)

## 📜 License

This project is intended for educational and learning purposes.
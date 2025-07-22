# 💬 JavaFX Chat App with Multi-Client Support (Sockets)

This is a simple **real-time chat application** built with **JavaFX** for the UI and **Java sockets** for networking. It allows multiple clients to connect to a server and exchange messages in real time.

---

## 📌 Features

- JavaFX client GUI with message bubbles
- Multi-client support using threads
- System messages when users join/leave
- Timestamp for each message
- Scrollable chat with smart alignment (left/right)
- Also includes a basic CLI client

---

## 🏗️ Project Structure


- 🔌 Communication via `Socket` et `BufferedReader/Writer`.


## 📁 Structure du projet
```
src/net/example/chatappwebsockets/app/
├── Chat2.java # JavaFX GUI client
├── Client.java # Simple console-based client
├── Server.java # Basic one-client console server
├── ServerMultiThread.java# Multi-client socket server
└── SocketThread.java # Handles one client in a separate thread
```

---

## 🚀 Getting Started

### ✅ Requirements

- Java 11 or higher
- JavaFX SDK (for GUI client)
- IDE (like IntelliJ, Eclipse, or VS Code)

---

### 🔧 Compile & Run

#### 1. Start the multi-client server

```bash
# Compile
javac ServerMultiThread.java SocketThread.java
# Run
java net.example.chatappwebsockets.app.ServerMultiThread
```
## 2. Run the GUI client (JavaFX)
- Make sure JavaFX SDK is correctly configured in your IDE or use VM options:
```bash
# VM options example
--module-path /path/to/javafx-sdk/lib --add-modules javafx.controls,javafx.fxml
```
```bash
# Run the Chat2 class
java net.example.chatappwebsockets.app.Chat2
```
## 3. (Optional) Run CLI Client
```bash
javac Client.java
java net.example.chatappwebsockets.app.Client
```
---

## 🖼️ Screenshots

Interface utilisateur simple et responsive avec bulles de messages personnalisées.

![Chat UI Screenshot](./screenshots/screen.PNG)

---

## 🔌 Port Information

| Component    | Port |
|--------------|------|
| Server       | 9093 |
| GUI Client   | 9093 |
| CLI Client   | 9093 |

> ⚠️ Assurez-vous que le serveur est lancé **avant** tout client.

---

## 👤 Author

**Abdelkarim El Hajbi**  
📧 [LinkedIn](https://www.linkedin.com/in/abdelkarim-el-hajbi)  
💻 [GitHub](https://github.com/abdelkarimelhajbi)

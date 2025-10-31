# Assigment-04-Simple-Chatroom_Mohamed_mejahed

💬 Go RPC Chat Application

A simple and lightweight real-time chat system built with Go (Golang) using the net/rpc package.
This project demonstrates how to implement client-server communication, message broadcasting, and concurrency in Go.

🚀 Features

Multi-user chat over RPC

Colored terminal output for users and system messages

In-memory message history

Thread-safe message handling

Simple console interface

🧩 Project Structure
go-chat/
├── server.go   # Chat server handling users and broadcasting
├── client.go   # Chat client for sending and receiving messages
└── README.md   # Documentation
|__ Video       # https://drive.google.com/file/d/1oC5ayvjC_Zjc5uErskf5w06HGa1K-aaj/view?usp=sharing

⚙️ Requirements

Go 1.18 or newer

Two or more terminals (for server and clients)

🏗️ How to Run
1️⃣ Start the Server
go run server.go


Or set a custom port:

export CHAT_PORT=8080
go run server.go

2️⃣ Start a Client
go run client.go


If the server is remote:

export CHAT_SERVER=192.168.1.10:1234
go run client.go

💡 Usage

Type messages and press Enter to send

Type quit to leave the chat

Color legend:

Color	Meaning
🟡 Yellow	Your messages
🔴 Red	Other users
🩵 Cyan	System info
🧠 Notes

Chat messages are stored in memory only (not persistent).

Uses sync.Mutex for thread-safe access.

Simple console I/O — easy to extend or customize.

🔧 Possible Improvements

Add message saving (to file or DB)

Add private messaging

Add user authentication

Upgrade to gRPC or WebSocket

👨‍💻 Author

Developed by Mohamed Ahmed Mejahed

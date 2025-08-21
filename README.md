# 💬 Real-Time Chat Application

A **real-time chat application** built with **Spring Boot, WebSockets, STOMP, and SockJS** for the backend, and **HTML, CSS, and JavaScript** for the frontend.  
It supports instant two-way communication, user join/leave notifications, and a responsive chat UI.

---

## 🚀 Features
- Real-time communication using **WebSocket + STOMP protocol**  
- User join/leave system with broadcast notifications  
- Dynamic chat messages with **color-coded avatars**  
- Responsive chat UI built with **HTML, CSS, JavaScript**  
- **SockJS fallback** for reliable WebSocket connections  
- Cross-browser compatibility  

---

## 🛠 Tech Stack
**Backend:**
- Java 17  
- Spring Boot 3.x  
- Spring WebSocket (STOMP)  

**Frontend:**
- HTML5, CSS3, JavaScript  
- SockJS, STOMP.js  

---

## 📂 Project Structure
chat-application/
│
├── src/main/java/com/shrey/chat/
│ ├── ChatApplication.java # Spring Boot main class
│ ├── WebSocketConfig.java # WebSocket + STOMP configuration
│ ├── ChatController.java # Handles incoming/outgoing chat messages
│ ├── ChatMessage.java # Chat message model (sender, content, type)
│ ├── MessageType.java # Enum for CHAT, JOIN, LEAVE
│ └── WebSocketEventListener.java # Tracks user connect/disconnect events
│
├── src/main/resources/static/
│ ├── index.html # Chat UI
│ ├── main.js # Frontend WebSocket + UI logic
│ └── main.css # Styling for chat UI
│
└── pom.xml # Maven dependencies

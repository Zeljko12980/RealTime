# 🔨 Real-Time Chat App with Video Calls  

A real-time chat application with WebRTC-based video calling, built using **React, SignalR, ASP.NET Core, and WebRTC**.  

---

## 🚀 Features  
👉 **Real-time text chat** using SignalR  
👉 **Peer-to-peer video calls** using WebRTC  
👉 **User authentication** (optional)  
👉 **Light/Dark mode support**  

---

## 🛠 Technologies Used  
- **Frontend**: React, Material UI, SignalR client  
- **Backend**: ASP.NET Core, SignalR  
- **Real-time communication**: SignalR & WebRTC  

---

## 📺 Project Structure  

```
📆 realtime-chat-app
├── 📺 api          # ASP.NET Core backend
│   ├── Controllers/    # API Controllers
│   ├── Hubs/           # SignalR Hubs
│   ├── Models/         # Database models
│   ├── appsettings.json
│   ├── Program.cs
│   ├── Startup.cs
├── 📺 react-view         # React frontend
│   ├── src/
│   │   ├── components/ # UI Components
│   │   ├── App.js      # Main app component
│   │   ├── VideoCall.js # WebRTC Video Calling
│   │   ├── ChatRoom.js  # Chat interface
│   ├── package.json
│   ├── .env
└── README.md
```

---

## 🛠 Installation & Setup  

### **1⃣ Clone the Repository**  
```sh
git clone https://github.com/yourusername/realtime.git
cd realtime-chat-app
```

### **2⃣ Backend Setup**  

1. Navigate to the backend directory  
   ```sh
   cd backend
   ```
2. Install dependencies  
   ```sh
   dotnet restore
   ```
3. Run the backend server  
   ```sh
   dotnet run
   ```
4. The backend will start on **`http://localhost:5255`**  

---

### **3⃣ Frontend Setup**  

1. Navigate to the frontend directory  
   ```sh
   cd ../frontend
   ```
2. Install dependencies  
   ```sh
   npm install
   ```
3. Start the React application  
   ```sh
   npm start
   ```
4. The frontend will be available at **`http://localhost:3000`**  

---

## 🖥️ Usage  

### **Join a Chat Room**
1. Open the app in your browser  
2. Enter a **username** and select a **chatroom**  
3. Start chatting in real time!  

### **Start a Video Call**  
1. Click on the **"Start Call"** button  
2. Grant camera & microphone permissions  
3. Invite another user to join the call  

---

## ⚙️ Configuration  

To change the **backend URL**, update the **SignalR connection URL** in `frontend/src/App.js`:

```js
const conn = new HubConnectionBuilder()
  .withUrl("http://localhost:5255/chat")
  .build();
```

---

## 🔥 Future Improvements  
👉 User authentication (JWT)  
👉 File sharing support  
👉 Group video calls  

---

## 🤝 Contributing  
Want to contribute? Fork the repository and submit a pull request!  

---

## 🐝 License  
This project is licensed under the **MIT License**.  

---

## ✨ Credits  
- Developed by **Željko Ikanović** 🚀  
- GitHub: https://github.com/Zeljko12980
- Email: ikanoviczeljko095@gmail.com

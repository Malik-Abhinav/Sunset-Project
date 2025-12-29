> This project was originally developed as part of a university course and later published as an independent public repository for portfolio purposes.

# 💬 Discord Clone Dashboard

A high-fidelity Discord-style chat application built with **Next.js 15**, **Stream Chat SDK**, and **Tailwind CSS**.  
The project focuses on real-time messaging, server and channel organization, and a custom UI that mirrors the core Discord experience.

---

## 🚀 Key Features

- **Real-time Messaging**  
  Powered by Stream Chat for low-latency message delivery and typing indicators.

- **Server and Channel Management**  
  Create and join servers with multiple text channels and category-based organization.

- **Custom UI Components**  
  Hand-crafted components including message reactions, custom headers, and Discord-style sidebar navigation.

- **Authentication and User Sync**  
  Secure token generation and user registration via Next.js API routes.

- **Interactive Messaging**  
  Emoji reactions, file uploads, and threaded conversations.

- **Containerized Environment**  
  Fully Dockerized setup for consistent development and deployment.

---

## 🛠 Tech Stack

- **Frontend:** Next.js 15 (App Router), React 19, TypeScript  
- **Styling:** Tailwind CSS, Lucide React  
- **Chat Backend:** Stream Chat SDK (GetStream)  
- **API:** Next.js Serverless Functions (TypeScript)  
- **DevOps:** Docker, Docker Compose  

---

## 📂 Project Structure

- **/app**  
  Next.js App Router logic and API endpoints (`/api/token`, `/api/register-user`)

- **/components**  
  Modular UI components (`ServerList`, `ChannelList`, `MessageList`)

- **/context**  
  Global state management for Discord-specific data

- **/hooks**  
  Custom hooks for Stream Chat client initialization

- **/models**  
  TypeScript interfaces and definitions for servers and users

---

## 🏃‍♂️ Getting Started

### Prerequisites

- Node.js 18+ or Docker  
- A Stream Chat API key and secret  

### Environment Variables

Create a `.env.local` file in the root directory:

```env
NEXT_PUBLIC_STREAM_API_KEY=your_api_key
STREAM_API_SECRET=your_api_secret
```

### Installation

Clone the repository:

```bash
git clone <your-repo-link>
cd discord-clone
```

Run with Docker (recommended):

```bash
docker-compose up --build
```

Run locally:

```bash
npm install
npm run dev
```

The application will be available at **http://localhost:3000**.

---

## 🧪 Testing

The project includes unit and integration tests for API routes and middleware using **Vitest** and **Jest**.

```bash
npm run test
```

---

## 📝 License

This project is licensed under the **MIT License**.

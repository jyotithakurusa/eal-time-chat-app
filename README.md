# Real-Time Chat Application

> Multi-room real-time chat with typing indicators, read receipts, and presence tracking. Built on WebSockets with Redis pub/sub for cross-instance scaling.

**Status:** 🚧 Work in progress
**Tech stack:** React · Socket.IO · Node.js · Redis · AWS

---

## What it does

A real-time chat application designed to demonstrate production-grade WebSocket patterns: bidirectional communication, presence tracking, typing indicators, read receipts, and horizontal scaling via Redis pub/sub. Built as a reference implementation rather than a Slack clone.

## Planned features

- [x] Project scaffolding
- [ ] User authentication (JWT)
- [ ] Real-time messaging via Socket.IO
- [ ] Multi-room chat with join / leave
- [ ] Typing indicators + read receipts
- [ ] Presence tracking (online / offline / away)
- [ ] Redis pub/sub for cross-instance scaling
- [ ] Message history persistence (MongoDB)
- [ ] CI/CD via GitHub Actions
- [ ] AWS deployment with CloudWatch logs + alerts

## Tech stack rationale

- **React + Socket.IO client** — the standard real-time UI stack
- **Node.js + Socket.IO server** — non-blocking I/O is the right fit for many concurrent connections
- **Redis pub/sub** — lets the app scale horizontally across multiple Node instances
- **MongoDB** — flexible schema for messages and chat history
- **AWS + CloudWatch** — production deploy with observability built in

## How to run locally

```bash
git clone https://github.com/jyotithakurusa/real-time-chat-app.git
cd real-time-chat-app
docker compose up
```

## Roadmap

- v0.1 — Basic real-time messaging in a single room
- v0.2 — Multi-room + auth
- v0.3 — Typing indicators, read receipts, presence
- v0.4 — Redis pub/sub scaling
- v1.0 — AWS production deploy with observability

---

**Author:** Jyoti Thakur · [GitHub](https://github.com/jyotithakurusa) · jyotithakurusa@gmail.com

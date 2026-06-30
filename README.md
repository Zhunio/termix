# 💻 Termix

Self-hosted web-based terminal and remote access platform powered by Apache Guacamole.

## ✨ Features

- 💻 Browser-based terminal access.
- 🌐 Remote desktop and SSH connections via Apache Guacamole.
- 🔒 Secure web interface.
- 💾 Persistent application data.
- ❤️ Lightweight deployment.
- 🐳 Run with Docker Compose or Coolify.

## 🚀 Coolify

Deploy this repository as a Docker Compose service.

- 🔐 Repository Type: `Private Repository (with GitHub App)`
- 🐙 GitHub App: `zhunio-coolify`
- 🌿 Branch: `main`
- 🐳 Build Pack: `Docker Compose`
- 🌐 Domain: `termix.example.com`
- 📂 Data mount:
  - `/opt/termix/data`

For detailed deployment instructions, see [`DEPLOY.md`](DEPLOY.md).

## ⚙️ Configuration

Configure Termix using Coolify environment variables.

### Required

- 🖥️ **GUACD_HOST** — Hostname of the Guacamole daemon.
- 🔌 **GUACD_PORT** — Port exposed by the Guacamole daemon.

Example:

```env
NODE_ENV=production
GUACD_HOST=guacd
GUACD_PORT=4822
```

## ♻️ Restore

Restore consists of:

1. 🛑 Stop the application.
2. ☁️ Restore `/opt/termix/data`.
3. 🚀 Start the application.


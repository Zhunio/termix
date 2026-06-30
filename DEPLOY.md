# 🚀 Deploy to Coolify

1. 📁 Create a new project.
2. ➕ Create a new resource.
3. 🔐 Select `Private Repository (with GitHub App)`.
4. 🐙 Select GitHub App `zhunio-coolify`.
5. 📦 Select the `termix` repository.
6. ⚙️ Configure:
   - 🌿 Branch: `main`
   - 🐳 Build Pack: `Docker Compose`
   - 📄 Docker Compose Location: `/docker-compose.yml`

7. 🏷️ Set:
   - **Name:** `termix`
   - **Domain:** `https://termix.zhunio.com`
8. 💾 Verify the host data directory:
   - `/opt/termix/data`
9. 🔑 Configure the required environment variables.
10. 🚀 Click **Deploy**.

## 🔑 Environment Variables

```text
NODE_ENV=production
GUACD_HOST=guacd
GUACD_PORT=4822
```

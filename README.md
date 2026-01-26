## 👋 Welcome to rabbitmq 🚀

Self-hosted rabbitmq application

## 📋 Description

Self-hosted rabbitmq application

## 🚀 Services

- **db**: rabbitmq:management

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/rabbitmq/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/rabbitmq" ~/.local/srv/docker/rabbitmq
cd ~/.local/srv/docker/rabbitmq
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install rabbitmq
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:59043

## 📂 Volumes

- `./rootfs/data/db/rabbitmq` - Data storage
- `./rootfs/config/rabbitmq/plugins` - Data storage

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄

[中文版](https://github.com/uuky77/lioil-vault-sync/blob/master/README_ZH.md)
 # Lioil Vault Sync

Multi-cloud vault sync plugin for [Obsidian](https://obsidian.md). Sync your vault to multiple cloud providers.

## Supported Cloud Providers

- **Baidu Netdisk** (百度网盘)
- **Aliyun Drive** (阿里云盘)
- **WebDAV** (Nextcloud, ownCloud, etc.)
- **S3 Compatible** (AWS S3, MinIO, Cloudflare R2, etc.)
- **Google Drive**

## Features

- Bidirectional sync with conflict detection
- Selective file/folder sync
- Encrypted sync support
- OAuth 2.0 authentication (Baidu, Google, Aliyun)
- Background auto-sync
- Chinese & English UI

## Installation

### From Obsidian Community Plugins
1. Open Settings → Community Plugins
2. Search "Lioil Vault Sync"
3. Install and enable

### Manual Installation
1. Download `main.js`, `manifest.json`, `styles.css` from [Releases](https://github.com/lioil/obsidian-vault-sync/releases)
2. Copy to `.obsidian/plugins/lioil-vault-sync/`

## Setup

1. Enable the plugin in Settings → Community Plugins
2. Click the cloud icon in the ribbon or run "Open Cloud Vault Sync" command
3. Choose your cloud provider and authenticate via OAuth
4. Configure sync directory and options in plugin settings

## External Services

This plugin connects to the following third-party APIs:

| Provider | Domains | Purpose |
|---|---|---|
| Baidu Netdisk | `pan.baidu.com`, `d.pcs.baidu.com` | File upload/download, OAuth |
| Aliyun Drive | `auth.aliyundrive.com`, `api.aliyundrive.com` | File sync, OAuth |
| Google Drive | `www.googleapis.com`, `oauth2.googleapis.com` | File sync, OAuth |

All data is transmitted directly between your device and the cloud provider. No third-party servers are involved.

## Privacy

- OAuth tokens are stored locally in Obsidian's `data.json`
- No analytics, telemetry, or data collection
- File content is only transferred between your device and the chosen cloud provider

## Development

```bash
npm install
npm run dev    # Watch mode
npm run build  # Production build
```

## License

MIT

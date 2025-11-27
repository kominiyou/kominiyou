# 🤖 Wily Bot - WhatsApp Automation

Bot WhatsApp otomatis dengan Baileys untuk handler pesan, event, dan integrasi Telegram dengan database JSON.

## ✨ Fitur Utama

- ✅ Otomasi pesan WhatsApp real-time
- ✅ Handler event dan message processing
- ✅ Integrasi Telegram seamless
- ✅ Database JSON untuk penyimpanan data
- ✅ QR Code terminal untuk autentikasi
- ✅ Environment variable configuration

## 🚀 Quick Start

### Prerequisites
- Node.js v16+
- npm atau yarn

### Installation

```bash
# Clone repository
git clone https://github.com/kominiyou/wily-bot.git
cd wily-bot

# Install dependencies
npm install

# Setup environment
cp .env.example .env
```

### Configuration

Edit file `.env` dengan konfigurasi Anda:

```env
# WhatsApp Configuration
BOT_NAME=Wily Bot

# Telegram Integration (optional)
TELEGRAM_TOKEN=your_token_here
```

### Running

Development mode dengan auto-reload:
```bash
npm run dev
```

Production mode:
```bash
npm start
```

## 📁 Project Structure

```
wily-bot/
├── src/
│   ├── index.js           # Entry point
│   ├── db/
│   │   └── json.js        # JSON database handler
│   ├── handler/
│   │   ├── event.js       # Event handler
│   │   └── message.js     # Message handler
│   └── helper/
│       ├── telegram.js    # Telegram integration
│       ├── text.js        # Text utilities
│       ├── utils.js       # General utilities
│       ├── inject.js      # Injection helpers
│       └── index.js       # Helper exports
├── sessions/              # WhatsApp sessions
├── package.json
└── .env                   # Environment variables
```

## 🔧 Dependencies

- **[Baileys](https://github.com/WhiskeySockets/Baileys)** - WhatsApp Web API wrapper
- **[dotenv](https://github.com/motdotla/dotenv)** - Environment variable loader
- **[qrcode-terminal](https://github.com/gtanner/qrcode-terminal)** - QR code display

## 📖 Usage

### Dasar

Bot akan menampilkan QR code saat pertama kali dijalankan. Scan dengan WhatsApp untuk login.

```javascript
// Example: Mengirim pesan
await sock.sendMessage(chatId, { text: "Hello World!" });
```

### Handler Pesan

Implementasi custom message handler di `src/handler/message.js` untuk merespons pesan otomatis.

### Integrasi Telegram

Configure Telegram token di `.env` dan gunakan functions di `src/helper/telegram.js`.

## 🤝 Kontribusi

Kontribusi welcome! Silakan:

1. Fork repository
2. Buat feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## ⚠️ Disclaimer

Bot ini untuk tujuan edukatif. Pastikan Anda mematuhi ToS WhatsApp dan hukum lokal yang berlaku.

## 📝 License

MIT License - Lihat file [LICENSE](LICENSE) untuk detail.

## 👤 Author

**Wily Kaish**

- GitHub: [@kominiyou](https://github.com/kominiyou)
- Email: Contact via GitHub

---

<div align="center">

Made with ❤️ by [Wily Kaish](https://github.com/kominiyou)

⭐ Jika project ini membantu, berikan star!

</div>

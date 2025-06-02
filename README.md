# 🔊 WhatsApp Audio Messaging API for JavaScript | Send Audio Messages via WhatsApp API

> **Professional WhatsApp API Integration** - Send audio messages programmatically using JavaScript/Node.js with Maytapi's powerful WhatsApp API. Perfect for voice notes, podcasts, music sharing, and audio communications.

[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Node.js](https://img.shields.io/badge/Node.js-16%2B-green.svg)](https://nodejs.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![WhatsApp API](https://img.shields.io/badge/WhatsApp-API-25D366.svg)](https://maytapi.com/)
[![Maytapi](https://img.shields.io/badge/Powered%20by-Maytapi-orange.svg)](https://maytapi.com/)

## 🌟 Overview

This JavaScript/Node.js library provides seamless integration with **WhatsApp API** for sending audio messages programmatically. Designed specifically for businesses and developers who need to share voice recordings, audio announcements, music files, and voice communications through WhatsApp with professional quality and reliability.

**Perfect for:** Voice notifications, podcast sharing, music distribution, voice memos, audio announcements, customer support recordings, and automated voice communications.

## 🔗 Essential Links & Resources

| Resource | Description | Link |
|----------|-------------|------|
| 🌐 **Official Website** | Maytapi WhatsApp API Platform | [Visit Site](https://maytapi.com/) |
| 🔐 **Developer Console** | API management and configuration | [Login Portal](https://console.maytapi.com/login) |
| 💰 **Pricing & Plans** | Flexible pricing for all business sizes | [View Pricing](https://maytapi.com/whatsapp-api-pricing) |
| 📖 **API Documentation** | Complete developer documentation | [Read Docs](https://maytapi.com/whatsapp-api-documentation) |

## ⭐ Key Features & Capabilities

### 🔊 **Audio Messaging Methods**
- ✅ **URL-based Audio Sending** - Direct audio URLs (MP3, WAV, OGG, M4A, AAC)
- ✅ **Base64 Audio Encoding** - Send audio from local files or memory buffers
- ✅ **Audio Captions** - Add descriptive text to your audio messages
- ✅ **Bulk Audio Broadcasting** - Send to multiple recipients simultaneously
- ✅ **Audio Format Validation** - Automatic format checking and duration validation

### 🛠️ **Developer-Friendly Features**
- ✅ **Modern JavaScript/ES6+** - Built with latest JavaScript standards
- ✅ **Lightweight Axios Implementation** - Optimized HTTP client for audio uploads
- ✅ **Promise-based API** - Full Promise and async/await support
- ✅ **Robust Error Handling** - Detailed error messages and stack traces
- ✅ **TypeScript Support** - Full TypeScript definitions included
- ✅ **Audio Duration Detection** - Automatic audio length validation

### 🔒 **Security & Performance**
- ✅ **Secure Token Authentication** - Token-based security
- ✅ **HTTPS Encryption** - All communications secured with TLS
- ✅ **Audio File Security** - Format validation and content scanning
- ✅ **Rate Limiting** - Built-in request throttling
- ✅ **Retry Mechanisms** - Automatic retry with exponential backoff
- ✅ **Bandwidth Optimization** - Compressed audio transfer

---

## 📦 Installation  
Install Axios to enable HTTP requests:

```bash
npm install axios
```
## 🔧 Usage Example
```javascript
const WhatsAppAPI = require('./index');

// Initialize the API
const api = new WhatsAppAPI({
  productId: "YOUR_PRODUCT_ID",
  phoneId: "YOUR_PHONE_ID",
  apiToken: "YOUR_API_TOKEN"
});

// Send an audio message via URL
api.sendAudioMessage({
  to: "1234567890",
  audioUrl: "https://example.com/audio.mp3",
  caption: "Check out this audio!"
})
.then(response => {
  console.log("Message sent successfully:", response);
})
.catch(error => {
  console.error("Message sending failed:", error);
});

// Send an audio message from Base64 data
api.sendAudioFromBase64({
  to: "1234567890",
  base64Data: "data:audio/mp3;base64,...",
  caption: "Base64 audio message"
})
.then(response => {
  console.log("Base64 message sent:", response);
})
.catch(error => {
  console.error("Base64 message sending failed:", error);
});
```
## 🔒 Authentication  
Ensure you have the following credentials:  
- Product ID  
- Phone ID  
- API Token

## 📝 Methods  
- `sendAudioMessage()`: Send audio via URL  
- `sendAudioFromBase64()`: Send audio using Base64 encoding

## 🔍 Error Handling  
The library provides comprehensive error logging and throws detailed error messages.

## 📜 License  
MIT License

## 🤝 Support  
For issues or questions, please open a GitHub issue.

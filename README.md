## 🔊 WhatsApp Audio Messaging API  
Send audio messages via WhatsApp using Maytapi's powerful API.

## 🚀 Features  
- Send audio messages with ease  
- Support for both URL-based and Base64 encoded audio  
- Optional captions for audio messages  
- Lightweight Axios implementation  
- Robust error handling

## 🔗 Navigation Links

Based on stakeholder feedback, the following key navigation links have been added:

- 🌐 [Home Page](https://maytapi.com/)  
- 🔐 [Login Page](https://console.maytapi.com/login)  
- 💰 [Pricing](https://maytapi.com/whatsapp-api-pricing)  
- 📄 [Documentation](https://maytapi.com/whatsapp-api-documentation#)
  

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

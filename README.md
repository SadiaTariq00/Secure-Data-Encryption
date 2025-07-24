# 🔐 Secure Data Encryption System using Streamlit

This is a **Streamlit** web application that allows users to **register**, **login**, **securely encrypt**, and **decrypt personal text data** using a passphrase. It includes protection against brute-force attacks via **temporary lockouts** after failed login attempts.

---

## 🌟 Features

- 📝 **User Registration & Login**
- 💾 **Encrypt and Store Data Locally**
- 🔓 **Decrypt with Passkey**
- 🚫 **Lockout after 3 failed login attempts**
- 🎨 Integrated **Lottie animation** for UI
- ✅ No external database – 100% local storage (`secure_data.json`)

---

## 🧠 How It Works

- Passwords are hashed using **PBKDF2-HMAC (SHA256)** with salt.
- Encryption/Decryption is done using **Fernet (symmetric key)** from the `cryptography` library.
- All user data is stored in a local JSON file.
- Encrypted data can only be retrieved with the correct passkey.

---

## 🛠️ Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/secure-data-encryption.git
   cd secure-data-encryption

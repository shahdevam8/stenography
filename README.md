# 🔐 Steganography with Password Protection and GUI

A Python-based tool to securely hide and retrieve messages inside images using pixel-level steganography with password protection. Includes both CLI and GUI options.

---

## 🧩 Features

- Hide secret messages inside PNG images
- Password-protected encryption and decryption
- Simple GUI using Tkinter
- CLI scripts for quick use
- No external APIs or internet required

---

## 🛠 Requirements

- Python 3.6 or higher
- Required libraries:
  ```bash
  pip install opencv-python pillow
  ```

---

## 🚀 How to Use

### 🔸 1. Encrypt via CLI
```bash
python encryption.py
```
- Input: Image path (`mypic.png`), message, password
- Output: Encrypted image saved as `encryptedImage.png`

### 🔸 2. Decrypt via CLI
```bash
python decryption.py
```
- Input: Encrypted image path and password
- Output: Prints hidden message if password is correct

---

### 🔸 3. Use the GUI
```bash
python gui.py
```
- Encrypt: Select an image, type a message and password → output saved as `encryptedImage.png`
- Decrypt: Select `encryptedImage.png`, enter password → message shown in popup

---

## 📁 File Structure

```
stenography/
├── encryption.py        # Encrypt message with password into image
├── decryption.py        # Decrypt message with password from image
├── gui.py               # GUI tool for encryption/decryption
├── encryptedImage.png   # Output file (created after encryption)
├── mypic.png            # Example input image (use your own PNG)
```

---

## ⚠ Notes

- Use **PNG or BMP** images only (JPG may corrupt data).
- Message length is limited by image size.
- Password is required for decryption. Wrong password = no access.

---

## 💡 To Improve

- Add SHA-256 hashing for password security
- Encrypt messages using AES
- Add drag-and-drop support in GUI
- Implement message length validation in GUI

---

## 👨‍💻 Author

Made by [Devam Shah](https://github.com/shahdevam8)
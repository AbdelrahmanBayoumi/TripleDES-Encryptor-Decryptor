# TripleDES-Encryptor-Decryptor

A simple web-based tool for performing Triple DES (3DES) encryption and decryption directly in your browser.

## Overview

This project provides an HTML page that allows users to encrypt and decrypt text using the Triple DES algorithm in ECB mode with PKCS7 padding. The tool is built using plain HTML, CSS, and JavaScript, utilizing the CryptoJS library for cryptographic functions.

## Features

- **Encrypt Text**: Input plaintext and a key to generate ciphertext.
- **Decrypt Text**: Input ciphertext and a key to retrieve the original plaintext.
- **Toggle Mode**: Seamlessly switch between encryption and decryption modes.
- **No External Dependencies**: Runs entirely in the browser without the need for server-side code or installations.

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari).

### Usage

1. **Clone or Download the Repository**

   ```bash
   git clone https://github.com/yourusername/TripleDES-Encryptor-Decryptor.git
   ```

2. **Open the HTML File**

   - Navigate to the project directory.
   - Open `index.html` in your web browser.

3. **Encrypting Text**

   - Select the **Encrypt** mode.
   - Enter your **Key** (encryption key).
   - Enter the **Plaintext** you wish to encrypt.
   - Click the **Encrypt** button.
   - The **Ciphertext** (Base64 encoded) will be displayed.

4. **Decrypting Text**

   - Select the **Decrypt** mode.
   - Enter your **Key** (must be the same as used for encryption).
   - Enter the **Ciphertext** (Base64 encoded) you wish to decrypt.
   - Click the **Decrypt** button.
   - The **Decrypted Text** will be displayed.

## Example

- **Key**: `Test_Key`
- **Plaintext**: `Hello World`
- **Ciphertext**: `p9vn6X7NFoLHeGIfusyALQ==`

## Security Considerations

**Important**: This tool is intended for educational purposes to demonstrate how Triple DES encryption and decryption work. **Triple DES and ECB mode are considered outdated and insecure for protecting sensitive data**. They are vulnerable to various cryptographic attacks and should not be used for securing confidential or personal information.

- **Triple DES (3DES)**: Deprecated by NIST since 2017 due to its smaller block size and susceptibility to cryptographic attacks.
- **ECB Mode**: Does not use an initialization vector (IV) and can reveal patterns in the plaintext.

**Recommendation**: For modern encryption needs, consider using AES (Advanced Encryption Standard) with secure cipher modes like CBC (Cipher Block Chaining) or GCM (Galois/Counter Mode).

## Dependencies

- **CryptoJS Library**: Included via CDN in the HTML file.

  ```html
  <script src="https://cdn.jsdelivr.net/npm/crypto-js@4.1.1/crypto-js.js"></script>
  ```

## License

This project is licensed under the [MIT License](LICENSE).

# Encryption-and-Decryption

🔑 Secure Encrypter & Decrypter (Gradio Edition)
This project provides a simple and secure web-based tool to encrypt and decrypt messages using symmetric-key encryption. It is built with Python, using the gradio library for the user interface and the cryptography library for the underlying security.

The application runs locally in your browser, ensuring that your messages and keys are not sent over the internet.

✨ Features
Web-Based UI: Modern, clean, and responsive interface that works in any web browser.

Strong Encryption: Uses Fernet symmetric encryption (AES-128 in CBC mode with a 128-bit HMAC-SHA256 for authentication).

Key Management:

Generate new, cryptographically secure encryption keys.

Download keys directly from the UI.

Upload existing keys to decrypt messages.

User-Friendly: Clear separation between encryption/decryption tasks and key generation.

Secure by Design: Processes all data locally; no need for a constant internet connection after the initial page load.

🚀 How to Use
Follow these steps to get the application running on your local machine.

Prerequisites
Make sure you have Python 3 installed on your system.

1. Clone or Download the Project
First, get the project files onto your computer. If you have git installed, you can clone the repository. Otherwise, download the gradio_cipher_app.py file.

2. Install Dependencies
Navigate to the project directory in your terminal or command prompt and install the required Python libraries:

pip install gradio cryptography

3. Run the Application
Execute the main script from your terminal:

python gradio_cipher_app.py

4. Open in Your Browser
The terminal will display a message with a local URL, typically:

Running on local URL: http://127.0.0.1:7860

Open this URL in your web browser to start using the application.

5. Using the App
To Generate a Key:

Go to the "Generate New Key" tab.

Click the "Generate & Download Key" button.

Your browser will download a secret.key file. Save this file in a secure location.

To Encrypt a Message:

Go to the "Encrypt / Decrypt" tab.

Type or paste your message into the "Input Message" box.

Make sure "Encrypt" is selected under "Action".

Upload the secret.key file you generated.

Click "Process Message". The encrypted text will appear in the "Output" box.

To Decrypt a Message:

Go to the "Encrypt / Decrypt" tab.

Paste the encrypted text into the "Input Message" box.

Select "Decrypt" under "Action".

Upload the same key file that was used to encrypt the message.

Click "Process Message". The original message will appear in the "Output" box.

⚠️ Security Note
The security of your encrypted messages depends entirely on the secrecy of your key file.

Do NOT share your .key file. Anyone who has this file can decrypt any message encrypted with it.

Store your key files in a secure, private location.

Use a different key for different communication partners or purposes to limit the impact if one key is compromised.

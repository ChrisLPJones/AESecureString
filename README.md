 # AESecureString

 AESecureString is a C# console application that provides simple AES-256 encryption and decryption for secure message handling. This application uses a passphrase to generate a unique encryption key for each session, offering enhanced data protection.

 ## Features

 - **Encryption**: Encrypt messages using AES-256 with a passphrase-derived key.
 - **Decryption**: Decrypt messages with the original passphrase.
 - **Security**: Generates a unique salt and IV for each encryption to ensure secure, unpredictable ciphertext.

 ## Getting Started

 ### Prerequisites

 - [.NET 5 or later](https://dotnet.microsoft.com/download/dotnet) is required to run this console application.

 ### Installation

 1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/AESecureString.git
    cd AESecureString
    ```

 2. Open the project in Visual Studio or your preferred .NET IDE.

 3. Build and run the project.

 ### Usage

 1. Run the application:
    ```bash
    dotnet run
    ```

 2. Follow the on-screen instructions to:
    - Enter a passphrase to use as an encryption key.
    - Encrypt a message of your choice.
    - Decrypt a message using the correct passphrase.

 ### Example

 ```
 ==== AES Encryption and Decryption ====

 --- Encryption ---
 Enter a passphrase to use as the encryption key: mysecurepass
 Enter the message you want to encrypt: Hello, world!

 Encrypted text: [Your Encrypted Text]

 --- Decryption ---
 Enter the encrypted text to decrypt: [Paste Your Encrypted Text]
 Enter the passphrase used for encryption: mysecurepass

 Decrypted text: Hello, world!
 ```

 ## Project Structure

 - **Program.cs**: Contains the main encryption and decryption logic.
 - **EncryptString()**: Encrypts the given message with AES-256.
 - **DecryptCipher()**: Decrypts the provided ciphertext using the specified passphrase.

 ## Security

 This project leverages:
 - **AES-256 encryption**: A symmetric block cipher known for its robustness.
 - **PBKDF2 key derivation**: Ensures that the key is derived securely from the passphrase with salt and hashing.

 ## Contributing

 Contributions are welcome! Please submit a pull request for any improvements or issues.

 ## License

 This project is licensed under the MIT License.
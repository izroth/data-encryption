# data-cypher Module

The `data-cypher` module is a Node.js package that allows you to perform data encryption and decryption using the Advanced Encryption Standard (AES) algorithm with a specified password. It provides a simple and convenient way to secure sensitive data in your applications.

## Installation

You can install the `data-cypher` module using npm:

```bash
npm install data-cypher --save
```

## Usage

```javascript
const datacypher = require('data-cypher');

// Replace 'yourSecretPassword' with your actual secret password
const password = 'yourSecretPassword';

const encryptor = datacypher(password);

const originalData = 'This is my secret data';

// Encrypt data
const encryptedData = encryptor.encrypt(originalData);

console.log('Encrypted Data:', encryptedData);

// Decrypt data
const decryptedData = encryptor.decrypt(encryptedData);

console.log('Decrypted Data:', decryptedData);
```

### Parameters

- `password` (String): Your secret password used for encryption and decryption.

## Example

```javascript
const datacypher = require('data-cypher');

// Replace 'yourSecretPassword' with your actual secret password
const password = 'yourSecretPassword';

const encryptor = datacypher(password);

const originalData = 'This is my secret data';

// Encrypt data
const encryptedData = encryptor.encrypt(originalData);

// Decrypt data
const decryptedData = encryptor.decrypt(encryptedData);

console.log('Original Data:', originalData);
console.log('Encrypted Data:', encryptedData);
console.log('Decrypted Data:', decryptedData);
```

## Security Note

Please ensure that you keep your secret password safe and do not share it publicly. The security of your encrypted data depends on the strength of your password.

## Contributing

If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on [GitHub](https://github.com/izroth/data-encryption.git).

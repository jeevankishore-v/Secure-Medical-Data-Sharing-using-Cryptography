# 🔒 Secure Medical Data Sharing System

A web-based application demonstrating end-to-end encrypted healthcare information exchange using asymmetric cryptography principles.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![React](https://img.shields.io/badge/React-18.x-61dafb.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Security Considerations](#security-considerations)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🌟 Overview

This project is an educational demonstration of secure medical data sharing using cryptographic techniques. It simulates how healthcare providers can securely exchange patient information using public-key cryptography, ensuring data confidentiality and integrity.

**⚠️ Important:** This is an educational project for learning purposes. For production healthcare systems, use industry-standard cryptographic libraries and comply with HIPAA regulations.

## ✨ Features

- **🔐 Asymmetric Encryption**: Public-private key pair generation for each user
- **👥 User Management**: Add and manage healthcare providers with unique cryptographic keys
- **📝 Data Encryption**: Encrypt sensitive medical data using recipient's public key
- **🔓 Secure Decryption**: Decrypt data using private keys (only accessible to authorized recipients)
- **✅ Data Integrity**: Hash-based verification to ensure data hasn't been tampered with
- **📊 Activity Logging**: Real-time audit trail of all encryption/decryption operations
- **🎨 Modern UI**: Clean, responsive interface built with React and Tailwind CSS

## 🎥 Demo

### Encrypt Medical Data
1. Select a healthcare provider from the dropdown
2. Enter patient medical information
3. Click "Encrypt with Public Key"
4. View the encrypted ciphertext

### Decrypt Medical Data
1. Select the authorized user
2. Click "Decrypt with Private Key"
3. View the original plaintext data
4. Verify data integrity through hash matching

### Manage Users
- Add new healthcare providers
- View public and private keys
- Each user gets unique cryptographic keys

## 🛠️ Technologies Used

- **React 18** - Frontend framework
- **Tailwind CSS** - Styling and UI components
- **Lucide React** - Icon library
- **JavaScript (ES6+)** - Core programming language
- **Cryptographic Concepts**: XOR cipher, hashing, asymmetric encryption

## 📦 Installation

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Steps

1. Clone the repository:
```bash
git clone https://github.com/yourusername/secure-medical-data-sharing.git
cd secure-medical-data-sharing
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

4. Open your browser and navigate to:
```
http://localhost:3000
```

## 🚀 Usage

### Basic Workflow

1. **Initialize System**: The app loads with sample healthcare providers (Dr. Sarah Chen and Dr. James Wilson)

2. **Encrypt Data**:
   ```
   - Navigate to "Encrypt Data" tab
   - Select a recipient
   - Enter medical data (or load sample)
   - Click "Encrypt with Public Key"
   ```

3. **Decrypt Data**:
   ```
   - Navigate to "Decrypt Data" tab
   - Select the user with matching private key
   - Click "Decrypt with Private Key"
   - Verify data integrity
   ```

4. **Add Users**:
   ```
   - Navigate to "Manage Users" tab
   - Enter new user name
   - Click "Add User"
   - Keys are automatically generated
   ```

### Sample Medical Data Format

```
Patient: John Doe (ID: P-2024-1547)
Date: Oct 27, 2025
Diagnosis: Type 2 Diabetes Mellitus
BP: 135/85 mmHg | Heart Rate: 78 bpm
Current Medications: Metformin 500mg, Lisinopril 10mg
Notes: Patient responding well to treatment.
```

## 🔒 Security Considerations

### Educational Implementation

This project uses simplified cryptographic algorithms for educational purposes:
- **XOR cipher** for encryption/decryption
- **Simple hash function** for integrity verification

### Production Recommendations

For real-world healthcare applications, implement:

- **RSA-2048 or RSA-4096** for asymmetric encryption
- **AES-256-GCM** for symmetric encryption
- **SHA-256 or SHA-3** for hashing
- **Digital signatures** for authentication
- **TLS/SSL** for data transmission
- **Key management systems** (KMS)
- **HIPAA compliance** measures
- **Access control** and audit logging
- **Regular security audits**

### HIPAA Compliance

Real medical data systems must comply with:
- HIPAA Privacy Rule
- HIPAA Security Rule
- Protected Health Information (PHI) safeguards
- Breach notification requirements

## 📁 Project Structure

```
secure-medical-data-sharing/
├── public/
│   ├── index.html
│   └── favicon.ico
├── src/
│   ├── components/
│   │   └── SecureMedicalDataSharing.jsx
│   ├── App.js
│   ├── index.js
│   └── index.css
├── .gitignore
├── package.json
├── README.md
├── LICENSE
└── CONTRIBUTING.md
```

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and development process.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)

## 🙏 Acknowledgments

- Inspired by healthcare security standards and HIPAA guidelines
- Built with modern React practices
- Icons by [Lucide](https://lucide.dev)

## 📞 Contact

For questions or feedback, please open an issue on GitHub or contact:
- Email: your.email@example.com
- Project Link: [https://github.com/yourusername/secure-medical-data-sharing](https://github.com/yourusername/secure-medical-data-sharing)

---

⭐ If you find this project helpful, please give it a star!

**Note**: This is an educational project. Always consult with security professionals and comply with healthcare regulations when building production medical systems.

# Firebase User Management

## **Overview**
This project provides administrative tools to manage data in Firebase that cannot be modified directly through the console. It includes tasks such as updating user email addresses, synchronizing data between Firebase Authentication and Firestore, and other advanced database manipulations.

It is designed to facilitate the management of critical data that requires advanced logic and cannot be handled manually.

---

## **Core Features**
- **Firebase Authentication Management:**
  - Updating user email addresses.
  - Deleting and creating specific users.

- **Firestore Synchronization:**
  - Updating user-related data based on authentication changes.

- **Firebase Admin SDK Integration:**
  - Advanced interactions with Firebase Authentication and Firestore.

---

## **Project Structure**
The project follows a modular structure for easy maintenance and scalability:


firebase-user-management/
├── scripts/                   # Scripts for specific tasks
│   ├── updateEmail.js         # Updates user email addresses
├── utils/                     # Reusable utility functions
│   ├── firebaseAdmin.js       # Firebase Admin SDK initialization
│   └── logging.js             # Logging functions for debugging
├── config/                    # Configuration files
│   └── serviceAccountKey.json # Admin SDK credentials
├── package.json               # Project dependencies
├── .gitignore                 # Files ignored by Git
├── README.md                  # Project documentation
└── tsconfig.json              # TypeScript configuration (if applicable)

Getting Started

Prerequisites

Node.js: Install the latest version from nodejs.org.

Firebase CLI: Install the Firebase CLI globally:

npm install -g firebase-tools

Firebase Admin SDK Credentials:

Download the serviceAccountKey.json file from the Firebase console:

Go to Project Settings > Service Accounts.

Generate a new private key and save it to config/serviceAccountKey.json.

Installation

Clone this repository:

git clone https://github.com/yourusername/firebase-user-management.git

cd firebase-user-management

Install project dependencies:

npm install

Set up environment variables:

Create a .env file in the root directory with the following variables:

FIREBASE_CONFIG=your_firebase_config

Running the Application

To execute scripts, use node.

Example: Update Email

node scripts/updateEmail.js

Available Scripts

1. Update Email
updateEmail.js: Updates the email address of a specific user in Firebase Authentication.

Built With

Firebase Admin SDK: For advanced user and database management in Firebase.
Node.js: Backend runtime environment.

TypeScript (optional): For static typing and improved code robustness.

Contributing

Contributions are welcome! Follow these steps to contribute:

Fork the repository.
Create a new branch for your feature:

git checkout -b feature/AmazingFeature

Commit your changes:

git commit -m "Add some AmazingFeature"

Push to the branch:

git push origin feature/AmazingFeature

Open a Pull Request.

License

Distributed under the MIT License. See LICENSE for more information

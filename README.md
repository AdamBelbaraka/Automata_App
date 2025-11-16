# Automata App

A Python desktop application for creating, visualizing, and analyzing finite state automata (DFA/NFA), combined with an integrated security system including authentication, role management, 2FA, and full activity logging.

## Features

- **Security Features**:
  - User authentication with bcrypt password hashing
  - Two-factor authentication (2FA) using TOTP
  - Role-based access control (RBAC)
  - Secure password reset functionality
  - Security and activity logging
  - JSON-based secure storage

- **Automata Tools**:
  - Create and edit deterministic and nondeterministic automata
  - Visual representation of states and transitions
  - Analyze automata properties (determinism, completeness, accessibility)
  - Convert NFA to DFA
  - Minimize automata
  - Simulate and test words
  - Perform set operations (union, intersection, complement)

## System Requirements

- Python 3.7 or higher  
- Compatible with Windows, macOS, and Linux

## Installation

### Option 1: Using Virtual Environment

1. **Clone repository**:
   ```bash
   git clone https://github.com/AdamBelbaraka/Automata_App.git
   cd Automata_App
Create and activate virtual environment:

For Windows:

bash
Copier le code
python -m venv venv
venv\Scripts\activate
For macOS/Linux:

bash
Copier le code
python3 -m venv venv
source vvenv/bin/activate
Install dependencies:

bash
Copier le code
pip install -r requirements.txt
Option 2: Using Conda
Clone repository:

bash
Copier le code
git clone https://github.com/AdamBelbaraka/Automata_App.git
cd Automata_App
Create and activate conda environment:

bash
Copier le code
conda create -n automata_app python=3.9
conda activate automata_app
Install dependencies:

bash
Copier le code
pip install -r requirements.txt
Running the Application
Start the application:

bash
Copier le code
python -m gui.main
No additional setup is required.

Using the Application
Authentication
Login: Enter your username and password.

Register: Create a new account.

Enable 2FA during registration.

Add the displayed TOTP secret key to your authenticator app (Google Authenticator, Microsoft Authenticator).

Use the “Copy Secret Key” button to copy the key automatically.

Password Reset: Use "Forgot Password" to generate a secure reset request.

Creating and Analyzing Automata
Automata Tab:

Define the alphabet.

Add states (initial and final).

Create transitions.

Analysis Tab:

Check determinism and completeness.

Convert NFA to DFA.

Minimize automata.

Advanced Tab:

Simulate and test words.

Generate accepted or rejected words.

Apply set operations (union, intersection, complement).

Security Recommendations
Enable 2FA for all accounts.

Use strong and unique passwords.

Review security logs regularly.

Assign roles and permissions carefully.

Project Structure
pgsql
Copier le code
Automata_App/
├── Automates/          Saved automata
├── automata/           Core DFA/NFA functionality
├── Security/           Security system
├── gui/                GUI components
│   ├── main.py         Application entry point
│   └── pages/          GUI pages
│   └── widgets/        Custom widgets
└── requirements.txt    Dependencies
Troubleshooting
Login Issues: Check username, password, and 2FA code.

Automata Errors: Ensure automata use the same alphabet for set operations.

If you encounter a problem, feel free to open an issue.

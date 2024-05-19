# Secure E-Voting System

## Abstract

### Secure E-Voting System for Hotel Chain


Welcome to the repository for our Secure E-Voting System, developed specifically for a hotel chain. This system provides a robust and secure platform for conducting elections within the organization, ensuring voter privacy, data integrity, and protection against various cyber threats. The system features two main panels: The Admin Panel and the Voter Panel, each equipped with advanced security measures.

## Features

### Admin Panel

The Admin Panel is designed for administrative users who manage the election process. Admins have two secure login options:

- **Office ID + Password + Captcha + OTP + Image Verification:**
  1. Admin logs in with their office ID, password, and captcha.
  2. Admin enters the OTP sent to their registered email.
  3. Admin provides a verification image. The system first compares the image hash and then verifies the pixels. Successful verification grants access to the Admin Panel.

- **Office ID + Fingerprint:**
  - Admin logs in with their office ID and fingerprint. Upon successful fingerprint verification, access to the Admin Panel is granted.

**Admin Panel Pages:**

- **Add Candidate:** Register new candidates for the election.
- **Add Voters:** Register new voters in the system.
- **Add Admins:** Register new administrative users.
- **Send Credentials:** Send specific images and passwords to new users via email.
- **Sent Mails:** View logs of sent emails.
- **View Result:** View election results.
- **Vote Reset:** Reset voting status for users.
- **Voter Remove:** Remove voters from the system.

### Voter Panel

The Voter Panel allows voters to participate in the election with two secure login options:

- **Office ID + Password + Captcha + OTP:**
  1. Voter logs in with their office ID, password, and captcha.
  2. Voter enters the OTP sent to their registered email. Successful verification redirects the voter to the voting page.

- **Office ID + Fingerprint:**
  - Voter logs in with their office ID and fingerprint. Upon successful fingerprint verification, access to the voting page is granted.

**Voting Page:**

- **Vote:** Voters can cast their vote. The system ensures each voter can vote only once. After voting, the voter is required to enter their verification image. The vote is published only upon successful image verification.

## Security Features

Our Secure E-Voting System employs a multi-layered security approach:

- **Multi-Factor Authentication (MFA):** Combines office ID, password, captcha, OTP, and image verification for secure access.
- **Fingerprint Authentication:** Provides an alternative secure login method using biometric verification.

- **Advanced Image Verification:** Utilizes hash comparison and pixel-by-pixel verification for identity confirmation.

- **AES-256 Encryption:** Encrypts sensitive voter information to protect against unauthorized access and data breaches.

- **Role-Based Access Control (RBAC):** Ensures that system access is restricted based on user roles, enhancing security.

- **HTTPS and TLS 1.3:** All web communications are encrypted using HTTPS with TLS 1.3, ensuring data integrity and confidentiality.

- **Real-Time Anomaly Detection:** Integrates machine learning models to detect and respond to suspicious activities in real-time.

- **Secure Session Management:** Implements secure session cookies with HttpOnly, Secure, and SameSite attributes to prevent session hijacking.


This system is designed to provide a secure, reliable, and user-friendly platform for conducting elections within the hotel chain, ensuring high standards of security and integrity in the electoral process.

Feel free to explore the repository, contribute, and provide feedback to help us improve this secure e-voting system. For more details on installation, setup, and usage, refer to the documentation provided in this repository.

## Documentation

### Software Requirements
<br>

- **Operating System:** Windows 10/11

## Front End

<div style="text-align: center;">
  <table style="border-collapse: collapse; margin: 0 auto;">
    <tr>
      <td style="text-align: center; border: none;">
        <img src="https://upload.wikimedia.org/wikipedia/commons/6/61/HTML5_logo_and_wordmark.svg" alt="HTML" width="50" height="50">
        <br>HTML
      </td>
      <td style="text-align: center; border: none;">
        <img src="https://upload.wikimedia.org/wikipedia/commons/d/d5/CSS3_logo_and_wordmark.svg" alt="CSS" width="50" height="50">
        <br> CSS
      </td>
      <td style="text-align: center; border: none;">
        <img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png" alt="JavaScript" width="50" height="50">
        <br>JavaScript
      </td>
      <td style="text-align: center; border: none;">
        <img src="https://upload.wikimedia.org/wikipedia/commons/b/b2/Bootstrap_logo.svg" alt="Bootstrap" width="50" height="50">
        <br>Bootstrap
      </td>
    </tr>
  </table>
</div>
<br>

## Back End

<table style="border-collapse: collapse; width: 100%;">
  <tr>
    <td style="text-align: center; border: none;">
      <img src="https://upload.wikimedia.org/wikipedia/commons/2/27/PHP-logo.svg" alt="PHP" width="50" height="50">
      <br>PHP
    </td>
    <td style="text-align: center; border: none;">
      <img src="https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg" alt="Python" width="50" height="50">
      <br>Python
    </td>
  </tr>
</table>

<br>

- **Database:**

  <div style="display: inline-block; text-align: center; margin: 0 20px;">
    <img src="https://upload.wikimedia.org/wikipedia/en/d/dd/MySQL_logo.svg" alt="MySQL" width="50">
   
  </div>

<br>

- **Device:**  MFS100 (Fingerprint Scanner)



## Prerequisites
1. **Enable GD Extension in XAMPP:** 
    - Open `php.ini` file located in the XAMPP installation directory.
    - Uncomment the line `extension=gd`.
    - Restart Apache from the XAMPP control panel.
    
2. **Install OpenSSL:**
    - Download and install OpenSSL from [here](https://slproweb.com/products/Win32OpenSSL.html).

3. **Install Composer:**
    - Download and install Composer from [here](https://getcomposer.org/download/).

4. **Install PHPMailer:**
    - Use Composer to install PHPMailer by running the following command in your project directory:
      ```bash
      composer require phpmailer/phpmailer
      ```
      Github link: https://github.com/PHPMailer/PHPMailer


5. **Install Python Libraries:**
    - Ensure you have Python installed. Then, install the necessary libraries:
      ```bash
      pip install pandas scikit-learn flask
      ```
      Start the Flask Server for ML Anomaly Detection

## Download and Install
1. **Download the Project:**
    - Download "E-Voting System Online" as a zip file or use WinRAR.

2. **Extract the File:**
    - Extract the downloaded zip file.
    - Copy the "E-Voting System Online" folder.

3. **Paste in XAMPP Directory:**
    - Paste the folder inside the root directory where you installed XAMPP (e.g., `C:/xampp/htdocs`).

4. **Set Up Database:**
    - Open PHPMyAdmin by navigating to [http://localhost/phpmyadmin](http://localhost/phpmyadmin).
    - Create a database named `evvv`.
    - Import the `evvv.sql` file found inside the `db` folder of the extracted package.

5. **Run the Script:**
    - Start Apache and MySQL from the XAMPP control panel.
    - Open your web browser and navigate to `https://localhost/E-Voting System Online`.

### Admin Credentials
- **Username:** Admin
- **Password:** password

## Testing

To test the API, follow these steps:

1. Open a terminal.
2. Make sure the API is running.
3. Send the payload for testing using the `curl` command and observe whether it is normal or fraud.

```sh
# Normal data point

curl -X POST -H "Content-Type: application/json" -d "{\"ct_src_dport_ltm\": 10, \"ct_dst_sport_ltm\": 15, \"sbytes\": 1500, \"dbytes\": 3000, \"spkts\": 10, \"dpkts\": 20, \"rate\": 0.5}" http://127.0.0.1:5000/detect_fraud

# Output:

# {
#   "result": "normal"
# }


# Anomalous data point

curl -X POST -H "Content-Type: application/json" -d "{\"ct_src_dport_ltm\": 100, \"ct_dst_sport_ltm\": 200, \"sbytes\": 100000, \"dbytes\": 200000, \"spkts\": 300, \"dpkts\": 400, \"rate\": 10.5}" http://127.0.0.1:5000/detect_fraud

# Output:
# {
#   "result": "fraud"
# }

```

## Future Work

- **Multi-Factor Authentication (MFA) and Image Verification:** 
  - Enhancing security by requiring multiple forms of verification, including image hash and pixel verification, to prevent brute force attacks.

- **Integration with Blockchain and Smart Contracts:** 
  - Incorporating blockchain technology for a decentralized, tamper-proof ledger and smart contracts to automate and enforce voting rules.

- **Homomorphic Encryption:** 
  - Allowing computations on encrypted data to ensure voter privacy and data integrity during analysis.

# 📱 SmartPay Design

---
#⚙️ Functional Requirements

## Users should be able to:
- Register using email verification or OTP.
- Log in and log out securely from web or mobile.
- View and update their profile and account settings.
- Reset or change their password securely.

## Administrators should be able to:
- View and manage user profiles.
- Deactivate or flag user accounts for review.
- Assist users with account recovery.


## End Users should be able to:
- View their current wallet balance in real-time.
- Link and unlink multiple payment methods (credit cards, bank accounts).
- Make real-time payments to merchants or other users.
- Top up their wallet using external funding sources.
- View a full history of transactions, including dates, amounts, and status.

## External Payment Gateway/Bank Systems should be able to:
- Process and authorize user payments and top-ups.
- Send confirmation of successful or failed transactions.


## End Users should be able to:
- Receive real-time push or in-app notifications about payment success or failure.
- Get SMS or email alerts for verification, login attempts, or critical account actions.


## Administrators should be able to:
- Monitor all user transactions in the system.
- Access detailed user profiles and account activity.
- Flag suspicious transactions or users for investigation.
- Take administrative actions such as freezing accounts or rolling back transactions.
- Resolve user disputes and complaints regarding transactions.


## Administrators should be able to:
- Generate daily, weekly, and monthly transaction reports.
- View usage statistics such as top users or most common transaction types.
- Access audit logs of administrative actions taken.
- Track system performance and user growth metrics.


## End Users should be able to:
- Authenticate using secure, encrypted methods.
- Access their account only with proper credentials or 2FA.
- Receive alerts for login from new devices or suspicious activity.

## Administrators should be able to:
- Define and manage roles and access levels (admin vs. support staff).
- Ensure system compliance with PCI DSS and GDPR.
- Monitor system logs for anomalies or unauthorized access attempts.

---

## ⚙️ Non-Functional Requirements – Smart Pay Digital Wallet
1. Real-Time Notification Accuracy
100% of successful or failed wallet-related operations ( payments, top-ups, account linking) must trigger a real-time notification that is displayed to the user within 2 seconds of the operation’s completion.

2. OTP Delivery Timing
One-Time Passwords (OTPs) for login and registration must be delivered to the user via email or SMS within 5 seconds of the request being triggered.

3. Transaction Responsiveness
All user-initiated payment transactions must be reflected in the wallet balance and transaction history within 1.5 seconds on both web and mobile platforms.

4. Wallet Top-Up Reflection
Wallet top-up actions initiated via linked bank accounts or cards must reflect updated balances in the user's dashboard within 3 seconds of receiving external confirmation.


---
# 📊 Use Case Diagrams

Below are the key use cases represented visually.

![User Management](UseCases/UserManagement.png)

![Payment Management](UseCases/PaymentManagement.png)


![Admin Management](UseCases/AdminManagement.png)
 
![Report Management](UseCases/ReportManagement.png)

![Notification Management](UseCases/NotificationManagement.png)

---
# 🗃️ SmartPay Database Design Diagrams
![Use Case 1 - SmartPay Database](Database/database.png)
---

# SmartPay Component&Deployement Design Diagrams
![Use Case 1 - SmartPay Deployement](Deployement/deployement.png)
---
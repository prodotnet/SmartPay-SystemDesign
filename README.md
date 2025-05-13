# SmartPay: Documentation

## 1. Introduction

The **SmartPay** project introduces an innovative voice-activated security feature aimed at protecting users from financial and personal harm in high-risk environments. By leveraging AI-driven voice recognition and a dynamic **"Safe Mode"** feature, SmartPay offers a unique solution that:

- Secures sensitive financial information.
- Disables transactions under duress.
- Sends silent alerts to trusted contacts during moments of threat.

With its **cross-platform support** and **seamless integration**, SmartPay empowers users to protect themselves in critical situations while maintaining ease of use and accessibility.

## 2. Problem Statement

In high-crime scenarios such as **armed robberies** or **coercion**, users are at significant risk when forced to open their mobile wallets. The primary concerns are:

- **Exposure of Sensitive Data**: If a criminal sees the real balance or is able to initiate transfers, the user may lose money or, worse, face personal harm.
- **Lack of Protection in Existing Wallets**: Most digital wallets lack an emergency safety mechanism for users under duress. This leaves users with no choice but to comply with a criminal's demands, putting their financial and personal safety in jeopardy.
- **User Stress and Panic**: In extreme situations, users may be too stressed to act or think clearly. There’s a need for an automatic solution that secures their information and acts in their defense.

## 3. Solution

SmartPay addresses the problem of coercion with a multi-layered security approach via its **Voice-Activated Safe Mode (VASM)**. Here’s how it works:

- **Voice-Activated Panic Mode**: The user speaks a predefined panic phrase (e.g., *“Please don’t hurt me”*), and SmartPay automatically detects the voice command and switches into Safe Mode. This mode immediately:
  - Displays a **fake balance** (e.g., *R0.00*).
  - Disables all transaction options to prevent unauthorized activity.
  
- **Silent Alerts**: SmartPay sends **real-time, silent alerts** to predefined contacts or administrators, notifying them of the user’s distress without alerting the attacker.

- **Offline Functionality**: The app uses the **Vosk API** for offline voice recognition, ensuring the Safe Mode can be activated even when there’s no network connection.

- **Dual Authentication**: To exit Safe Mode, users must log out and authenticate with a **secondary PIN**, preventing the attacker from bypassing the security layer.

This solution creates a **secure environment** that allows users to safely interact with their financial data even in life-threatening situations, while safeguarding them from harm.

## 4. Value Added

SmartPay stands out in several key ways:

- **User Safety and Financial Protection**: SmartPay’s core mission is to protect users. The VASM feature provides a **proactive safety mechanism** that addresses real-world threats, ensuring financial protection under duress.
  
- **AI and Offline Capability**: The offline voice recognition module ensures that panic mode can be activated even in **low or no network conditions**, making it more reliable than many traditional apps.

- **Cross-Platform Accessibility**: Built with **.NET MAUI**, SmartPay is available on **iOS, Android, and Windows**, ensuring **cross-platform compatibility** without sacrificing security or functionality.

- **Real-World Use Case**: This solution directly addresses critical safety concerns in high-risk environments, filling a gap in the market where many financial apps overlook user safety under threat.

- **Seamless User Experience (UX)**: Despite its complex security features, the app maintains a **simple and intuitive interface**. Even under stress, users can quickly and easily activate Safe Mode and manage their wallet without confusion.

---

## 5. Data Analytics in SmartPay

In addition to providing top-notch security features, **SmartPay** utilizes **data analytics** to enhance its functionalities, improve user experience, and monitor for any suspicious or fraudulent activities. Here's how **data analytics** is integrated into the system:

### 5.1. **User Behavior Analytics**
SmartPay tracks user behavior to optimize security and improve the overall user experience:

- **Voice Command Patterns**: Analytics are used to monitor the frequency and context in which the panic phrase is triggered. This helps identify patterns, including abnormal usage or potential abuse.
- **Transaction Monitoring**: SmartPay analyzes transaction patterns over time to detect unusual activity. For example, large transfers, rapid repeated transactions, or transfers to new addresses can trigger alerts for review.
  
By analyzing data patterns, SmartPay can improve its fraud detection and prevent unauthorized transactions from occurring during times of stress.

### 5.2. **Real-Time Analytics for Suspicious Activity**
To ensure the safety of users, **SmartPay** uses real-time data analysis for monitoring suspicious activities:

- **Unusual Transaction Behavior**: By applying machine learning algorithms, the app can learn a user’s typical transaction behavior (e.g., amounts, frequency, locations). If there is a significant deviation (such as a sudden large transfer), the system flags the activity and can trigger an automatic Safe Mode.
- **Geolocation Analytics**: Combined with **transaction data**, SmartPay analyzes users’ location data to detect discrepancies. For example, if a user’s phone is located in one region but a transaction is initiated from a different region, the system will consider this as suspicious and can prompt additional authentication checks or trigger Safe Mode.

### 5.3. **Voice Recognition Performance Optimization**
Using **TensorFlow.js** and **Vosk**, SmartPay improves the accuracy of voice recognition based on continuous data input:

- **Voice Data Analysis**: By collecting and analyzing voice recognition success rates, the system can adjust and optimize its algorithm for better accuracy under various conditions (background noise, accents, etc.).
- **Emotion Detection (Future Scope)**: In the future, SmartPay will analyze vocal emotions to improve the **panic phrase detection**. For example, a higher urgency in the user's tone could trigger an immediate response from Safe Mode.

### 5.4. **Predictive Analytics for Safety**
Predictive analytics is used to proactively identify potential risks before they occur:

- **Risk Scoring**: The system calculates a risk score for every transaction based on historical data and behavior analysis. If the score exceeds a threshold, additional safety measures such as double authentication or temporary transaction locks can be applied.
- **User Alert System**: Users receive **customized alerts** based on predictive analysis of their activity patterns. For instance, users who regularly transact at certain times or amounts might be alerted if a transaction deviates from their usual habits.

### 5.5. **Analytics for Operational Insights**
SmartPay also uses data analytics for **internal monitoring**:

- **Admin Dashboards**: The **admin panel** tracks user activity and provides analytics on system performance, including the frequency of panic mode activations, the number of transactions blocked, and the overall health of the app's security systems.
- **Real-Time Monitoring**: Admins can monitor live data feeds to identify potential security threats or misuse of the system, allowing for quick intervention if necessary.

---

## 6. How It Works: Flow Summary

1. **Normal Mode**: User logs in with **PIN or biometric authentication**, and the wallet interface loads with:
   - Real wallet balance
   - Quick actions for sending, receiving, and paying bills
   - Recent transaction history

2. **Safe Mode Activation**:
   - User speaks a predefined panic phrase (e.g., *“Please don’t hurt me”*).
   - Voice recognition detects the phrase and activates Safe Mode, displaying a **fake balance** and locking transaction capabilities.
   - Optionally, the app sends **silent alerts** to trusted contacts or administrators.

3. **Exiting Safe Mode**:
   - The user must log out and re-enter the app with the **secondary PIN** to exit Safe Mode.

---

## 7. Tech Stack

- **Frontend**: Angular 19, TypeScript, CSS, Bootstrap 5
- **Voice Recognition**: Vosk (offline), TensorFlow.js
- **Backend**: ASP.NET Core Web API (C#)
- **Authentication**: PIN + JWT Tokens
- **Database**: SQL Server
- **Mobile App**: .NET MAUI (Cross-Platform)
- **Analytics Tools**: Python (Pandas, Scikit-learn for machine learning), TensorFlow.js

---

## 8. Future Scope

- **Vocal Emotion Detection**: We plan to integrate emotion detection to make the panic phrase detection even smarter, based on the user’s tone, pitch, and urgency.
- **Extended Device Support**: Additional platforms, such as **smartwatches** and **IoT devices**, to broaden the app's coverage in emergency scenarios.

---

## 9. Conclusion

SmartPay is more than just a digital wallet; it is a **security-first financial solution**. By addressing a **real-world problem**—the safety of users in dangerous situations—SmartPay is pioneering the next generation of secure digital wallets. This combination of cutting-edge technology, **AI integration**, **data analytics**, and **real-world use cases** makes SmartPay a standout project in the fintech space.

---


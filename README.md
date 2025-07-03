# FINGERPRINT-AUTHENTICATION-VOTING-SYSTEM-USING-ARDUINO
Biometric EVM using Arduino and fingerprint sensor for secure, real-time voter authentication. Prevents duplicate voting, displays instructions on LCD, and provides buzzer feedback. A low-cost, standalone system enhancing election integrity and efficiency.
# Proposed System
We have designed an advanced system using a fingerprint module and arduino. In this biometric based voting machine, a person has to register a fingerprint ID with the system which will be centrally stored in Arduino. During the election process a person should place a finger, if the fingerprint matches with pre-stored information then the person is allowed to cast a vote. Else it will display Unauthorized voter.. For confirmation of voters, the confirmation message will be displayed on LCD regarding the  voting. If a voter has already voted then it displays the message of “already voted”.So in this way fake voting can be prevented. After the voting process is completed, results can be viewed by pressing the result button and the winner will be declared. It has a simple and  easily accessible hardware design

## 📌 Project Overview

- **Platform**: Arduino UNO
- **Authentication Methods**: Fingerprint / Password ID
- **Interface:** LCD Display + Buttons + Buzzer
- **Security:** Prevents duplicate voting and unauthorized access
- **Data Handling:** Stores votes in flash memory (EEPROM)

## 🛠️ Hardware Components

- Arduino Uno
- R305 Fingerprint Sensor
- 16x2 LCD Display
- Push Buttons (3 for voting)
- Buzzer
- Jumper Wires
- Breadboard or PCB
- Power Supply

## 🔄 System Workflow

### ✅ Step-by-Step Breakdown

**1. Start**  
- **Role:** Voter  
- **Action:** Voter begins the voting process.


**2. Authentication**

🔹 **Option A: Fingerprint**  
- Fingerprint sensor is enabled.  
- Fingerprint is compared with the database.  
  - ✅ **Match:** Proceed to Voting  
  - ❌ **No Match:** Show “Unknown” message + Beep alarm

🔹 **Option B: Password ID**  
- Prompt voter to enter a password ID.  
- ID is compared with stored data.  
  - ✅ **Match:** Proceed to Voting  
  - ❌ **No Match:** Show “Error” message + Beep alarm


**3. Check for Previous Vote**  
- System verifies if the voter has already voted.  
  - ❌ **Already Voted:** Show warning  
  - ✅ **Not Voted:** Continue


**4. Enable EVM**  
- EVM is activated for authenticated voter.


**5. Cast Vote**  
- Voter selects a party using push buttons.


**6. Store Vote**  
- Voter data and vote are stored securely in flash memory.


**7. End**  
- Voting process concludes with a thank-you message.


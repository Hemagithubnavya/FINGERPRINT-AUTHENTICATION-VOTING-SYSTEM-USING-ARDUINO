# FINGERPRINT-AUTHENTICATION-VOTING-SYSTEM-USING-ARDUINO
Biometric EVM using Arduino and fingerprint sensor for secure, real-time voter authentication. Prevents duplicate voting, displays instructions on LCD, and provides buzzer feedback. A low-cost, standalone system enhancing election integrity and efficiency.
# Proposed System
We have designed an advanced system using a fingerprint module and arduino. In this biometric based voting machine, a person has to register a fingerprint ID with the system which will be centrally stored in Arduino. During the election process a person should place a finger, if the fingerprint matches with pre-stored information then the person is allowed to cast a vote. Else it will display Unauthorized voter.. For confirmation of voters, the confirmation message will be displayed on LCD regarding the  voting. If a voter has already voted then it displays the message of “already voted”.So in this way fake voting can be prevented. After the voting process is completed, results can be viewed by pressing the result button and the winner will be declared. It has a simple and  easily accessible hardware design
# Step-by-Step Breakdown:
 1. Start
    
 ● Activity: "Voter"
 
 ● Description: The process begins when a voter initiates the voting procedure.
 3. Authentication
 ● Activity: Voter chooses between fingerprint authentication or password ID for 
authentication.
 ● Description: The voter decides on the method of authentication.
        Option 1: Fingerprint Authentication
            1. Enable fingerprint module for authentication.
            2. Description: The system activates the fingerprint reader.
            3. Compare the voter's fingerprint with the fingerprint database.
 Outcome:
 ■ Match: Proceed to step 8.
 ■ No Match: Display "unknown message" with a beep alarm.
 Option 2: Password ID Authentication
 1. Prompt the voter to enter their password ID.
 2. Description: The system requests the password ID from the voter.
 3. Compare the password ID with the database.
 Outcome:
 ■ Match: Proceed to step 8.
 ■ No Match: Display "error message" with a beep alarm.
 3. Check for Previous Vote
 ● Activity: Verify if the voter has already cast a vote.
 ● Description: The system checks the database to see if the voter has previously 
voted.
 Outcome:
 ■ Already Voted: Display a message informing the voter they have already 
voted.
 ■ Not Voted: Proceed to step 4.
 4. Enable EVM
 ● Activity: Enable the Electronic Voting Machine (EVM).
 ● Description: The system activates the EVM for the authenticated voter.
5. Cast Vote
 ● Activity: Voters cast their vote using the EVM.
 ● Description: The voter makes their selection on the EVM.
 6. Store Information
 ● Activity: Store all information in the database flash memory.
 ● Description: The system saves the vote and related data securely.
 7. End
 ○ Activity: "Activity Final"
 ○ Description: The voting process concludes

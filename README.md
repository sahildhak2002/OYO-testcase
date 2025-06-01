# OYO-testcase
🔴 Fail Test Cases
TC001 - Signup/Login: Accepts 12-digit Mobile Number (Fail)

Description: The Signup/Login page accepts mobile numbers with more than 10 digits (e.g., 12 digits), which is a clear violation of mobile number validation standards in India. It should restrict the user to only 10 numeric digits.

Impact: Users may register with invalid phone numbers, which could impact OTP verification and account management.

TC002 - Signup/Login: Accepts Alphabets in Mobile Number Field (Fail)

Description: The input field accepts alphabetic characters (e.g., "abcd1234"), which indicates a missing input type validation. Only numeric values should be allowed.

Impact: Invalid mobile numbers may be submitted, leading to failed verifications and a poor user experience.

TC003 - Signup/Login: Accepts More Than 20 Digits (Fail)

Description: The app does not limit the character length for the mobile number field. It accepts more than 20 digits, which is incorrect.

Impact: This can break form submissions, create database inconsistencies, and allow invalid registrations.

TC004 - Booking Page: Accepts 12-digit Mobile Number (Fail)

Description: Even on the booking page, the mobile number field allows users to input 12 digits. This inconsistency between modules reveals lack of shared validation logic.

Impact: Users may be unable to receive booking confirmations or updates if invalid numbers are entered.

✅ Pass Test Cases
TC005 - Signup/Login: Valid 10-digit Mobile Number (Pass)

Description: When the user enters a valid 10-digit Indian mobile number, the app accepts it and proceeds without any error.

Impact: Confirms correct input handling for standard use case.

TC006 - Signup/Login: Leave Mobile Field Empty (Pass)

Description: If the user skips the mobile number field and tries to proceed, the app displays a validation message such as "Mobile number is required."

Impact: Ensures mandatory field validation is implemented correctly.

TC007 - Booking Page: Valid 10-digit Number (Pass)

Description: On the booking page, entering a valid 10-digit number allows the user to continue with the booking process smoothly.

Impact: Confirms consistent validation in booking flow.

TC008 - Signup/Login: Paste Valid Number (Pass)

Description: Copying and pasting a 10-digit number into the mobile number field is handled correctly, showing that the paste functionality is also validated.

Impact: Confirms robustness of input handling even through copy-paste.

TC009 - Signup/Login: Input Restriction to Numeric Only (Pass)

Description: The field restricts input to numbers only and does not accept any alphabetic or special characters.

Impact: Prevents malformed data submission and enhances data integrity.

TC010 - Signup/Login: Cursor Stops After 10 Digits (Pass)

Description: The input field enforces a 10-digit limit, not allowing any more digits to be entered beyond the limit.

Impact: Avoids user error and maintains consistent data entry.

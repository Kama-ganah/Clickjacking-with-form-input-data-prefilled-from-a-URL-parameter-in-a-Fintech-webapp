# Overview
As a penetration tester, I assessed the user account management interface for UI redressing vulnerabilities. During testing, I identified a clickjacking issue caused by the absence of frame protections and the use of URL parameters to prefill sensitive form inputs. By embedding the account page within a transparent iframe and aligning a decoy element over the “Update email” action, I was able to trick a user into unknowingly modifying their account details. This project demonstrates how combining weak UI defenses with unsafe input handling can lead to unauthorized account changes through social engineering.

# Steps Undertaken

Step 1: Analyzed the account update functionality and identified URL-based input prefilling.

Step 2: Confirmed the absence of anti-clickjacking headers.

Step 3: Built an iframe-based exploit with CSS alignment to hijack user clicks.

Step 4: Verified successful exploitation by changing account data without user awareness.

# Conclusion

This assessment revealed a medium–high risk clickjacking vulnerability that enabled unauthorized modification of user data. The findings highlight the importance of proper frame protections and cautious handling of user-controllable input in sensitive UI workflows.

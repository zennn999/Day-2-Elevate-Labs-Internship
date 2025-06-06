# Day-2-Elevate-Labs-Internship


1. Example of a phishing email


From: support@netflix-security.com
To: user@example.com
Subject: Reset Your Netflix Password Immediately

Dear Netflix User,

We detected multiple failed login attempts to your Netflix account from a suspicious device.
For your security, we’ve temporarily locked your account. Please reset your password immediately to restore access:
Reset your password now:
http://netflix.com.account-recovery-reset.com
If you do not act within 24 hours, your account will be permanently locked.

Thank you for your attention,
Netflix Security Team

2. As we can see, the email above was sent by support@netflix-security.com which is similar to @netflix.com but it is not a legitimate netflix domain.

3. Header Analysis Summary

Email claims 'netflix.com', but comes from 'netflix-security.com'
SPF: Failed – the IP address is not authorized to send mail for the domain
DKIM: Failed – no valid cryptographic signature
DMARC: Failed – domain policy says reject such messages
These failures prove the email is spoofed and likely a phishing attempt.

4. The visible link http://netflix.com.account-recovery-reset.com has the domain account-recovery-reset.com which is not owned by netflix.

5. The sentances "we’ve temporarily locked your account" and "If you do not act within 24 hours" are threatening and shw uegency to use fear as a manipulation tactic.

6. Howering over the link http://netflix.com.account-recovery-reset.com showed the mismatch between the display name and the actual link.

7. "Dear Netflix User" has been used by them whereas netflix would have addressed you to your actual Username.

8.Conclusion
The email is a phishing attempt that uses:
- A fake sender domain
- A deceptive password reset link
- Urgency tactics to trigger emotional response

Recommendations:
- Block the sender domain
- Educate users about fake reset emails
- Report to Netflix and anti-phishing authorities

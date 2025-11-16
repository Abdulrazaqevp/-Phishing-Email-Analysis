# Analyze a Phishing Email - Sample Repository

This repo contains a complete example of a phishing email analysis, including:
- A sample phishing email
- Header analysis example
- Screenshots (placeholders)
- Updated README
- Full 7-step analysis example

## 7-Step Phishing Analysis Example

### 1. Sample Obtained
File: samples/sample-email.txt  
A fake PayPal security alert claiming account suspension.

### 2. Sender Email Analysis
- Display name: PayPaI Support
- From: support@paypaI-security.com  
(Mispelled domain: uses capital i instead of lowercase L)

### 3. Header Analysis
Stored in: headers/header-analysis.txt  
SPF: FAIL  
DKIM: NONE  
DMARC: FAIL  
Originating IP belongs to an ISP in another country.

### 4. Links & Attachments
Visible link: https://paypal.com/security  
Actual link: http://192.88.34.221/verify-login

### 5. Urgency Language
“Your account will be suspended in 24 hours unless you verify.”

### 6. Technical Indicators
- IP-based login page
- No HTTPS on destination link

### 7. Summary
Verdict: **Phishing**  
Confidence: High  
Reason: Spoofed domain, mismatched URLs, failed authentication.

See: analysis_example.md

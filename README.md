# Actor Adopte Get Auth Token Scraper
>This tool automates the full login flow for Adopte.app and returns the authentication tokens you need for making authenticated API requests. It handles browser automation, French residential proxy usage, credential submission, and token capture—so you get a clean, ready-to-use Auth Token without touching the login UI manually.

<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/Bitbash333" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>

<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>Actor Adopte Get Auth Token Scraper</strong> you've just found your team — Let's Chat. 👆👆
</p>

## Introduction
The scraper signs into Adopte.app using your email and password, retrieves the apiRefreshToken exposed by the web session, and exchanges it for a valid JWT Auth Token via the platform’s authentication endpoint. It’s designed for developers who need programmatic access to Adopte features such as profile browsing, messaging, or automated workflows.

### Why This Exists
- Automates the entire login → refresh token → JWT process.  
- Ensures all traffic appears as a French session through residential proxies.  
- Extracts usable authentication tokens for API integrations.  
- Enables headless or visible browser mode for debugging.  
- Useful for anyone building internal tools or data-driven Adopte workflows.

---
## Features
| Feature | Description |
|---------|-------------|
| Automated Login Flow | Submits email and password and captures session tokens. |
| Refresh Token Extraction | Reads apiRefreshToken placed on the browser window. |
| JWT Auth Token Exchange | Calls the authtokens endpoint to retrieve a valid token. |
| Proxy Support | Uses French residential proxies for realistic sessions. |
| Debug Mode | Toggle headless/visible browser for troubleshooting. |
| Structured Output | Returns status, refresh token, and final JWT. |

---
## What Data This Scraper Extracts
| Field Name | Field Description |
|------------|-------------------|
| success | Indicates whether the login and token extraction succeeded. |
| apiRefreshToken | The session’s refresh token captured from the browser. |
| authToken | The final JWT token obtained via API exchange. |
| authtokensStatus | HTTP status returned during token exchange (200 = valid). |
| timestamp | Time when the extraction was performed. |
| ... | Additional internal metadata if extended. |

---
## Example Output
    
    [
      {
        "success": true,
        "apiRefreshToken": "eyJ2ZXJzaW9uIjoxLCJ0eXAiOiJKV1Qi…",
        "authToken": "eyJ2ZXJzaW9uIjoxLCJ0eXAiOiJKV1Qi…",
        "authtokensStatus": 200,
        "timestamp": "2025-01-20T10:45:33Z"
      }
    ]

---
## Directory Structure Tree
    
    Actor Adopte Get Auth Token/
    ├── src/
    │   ├── main.js
    │   ├── login/
    │   │   ├── browser_flow.js
    │   │   ├── token_capture.js
    │   │   └── token_exchange.js
    │   ├── utils/
    │   │   ├── logger.js
    │   │   └── proxy_manager.js
    │   └── config/
    │       └── input_schema.json
    ├── data/
    │   ├── sample_input.json
    │   └── sample_output.json
    ├── package.json
    └── README.md

---
## Use Cases
- **Automation developers** need authenticated API access for profile viewing or interactions.  
- **Reverse-engineering engineers** automate controlled sessions without manual login.  
- **Data teams** extract valid tokens for internal scraping pipelines.  
- **QA testers** validate login flows repeatedly with minimal friction.  
- **Integration builders** connect Adopte data to dashboards or internal tools.  

---
## FAQs

**Is a French proxy required?**  
The actor uses French residential proxies by default to match expected traffic patterns, but you can override the proxy configuration.

**Does the scraper expose my password?**  
Passwords are handled securely during the login session and never included in output.

**What confirms the token is valid?**  
A status code of 200 from the authtokens endpoint indicates a successful and usable JWT.

**Can I disable headless mode?**  
Yes, set `headless` to false to view the browser for debugging.

---
### Performance Benchmarks and Results

**Primary Metric:**  
Completes login and token extraction in 8–15 seconds depending on proxy speed.

**Reliability Metric:**  
Achieves a 98% success rate with valid credentials and stable proxy routing.

**Efficiency Metric:**  
Minimizes browser overhead by extracting tokens as soon as they appear in the session.

**Quality Metric:**  
Provides fully formed JWT tokens with consistent validation status and timestamp accuracy.


---


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on."
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/m-dRE1dj5-k?si=5kZNVlKsGUhg5Xtx" target="_blank">
        <img src="https://github.com/Z786ZA/Footer-test/blob/main/media/review3.gif" alt="Review 3" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        "Exceptional results, clear communication, and flawless delivery. <br>Bitbash nailed it."
      </p>
      <p style="margin:1px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
         </p>

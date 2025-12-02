## Findings Table

| Code | Issue | Risk | Affected | Why It Matters |
| 10038 | Content Security Policy (CSP) Header Not Set | Medium | http://localhost:5000 | Prevents XSS attacks by controlling which resources can be loaded |
| 10020 | Missing Anti-clickjacking Header | Medium | http://localhost:5000 | Prevents clickjacking attacks where users are tricked into clicking hidden elements |
| 90004 | Insufficient Site Isolation Against Spectre Vulnerability | Low | http://localhost:5000 | Mitigates Spectre side-channel attacks through cross-origin isolation headers |
| 10063 | Permissions Policy Header Not Set | Low | http://localhost:5000 | Controls browser features (camera, microphone, geolocation) that scripts can access |
| 10036 | Server Leaks Version Information via "Server" HTTP Response Header | Low | http://localhost:5000 | Information disclosure - prevents attackers from knowing server version |
| 10021 | X-Content-Type-Options Header Missing | Low | http://localhost:5000 | Prevents MIME-sniffing attacks that could execute malicious scripts |
| 10109 | Modern Web Application | Informational | http://localhost:5000 | Detection indicates modern web application frameworks in use |
| 90005 | Sec-Fetch-Dest Header is Missing | Informational | http://localhost:5000 | Helps identify request context for CSRF protection |
| 90005 | Sec-Fetch-Mode Header is Missing | Informational | http://localhost:5000 | Identifies if request is for same-site or cross-site resource |
| 90005 | Sec-Fetch-Site Header is Missing | Informational | http://localhost:5000 | Identifies origin of the request for CSRF protection |
| 90005 | Sec-Fetch-User Header is Missing | Informational | http://localhost:5000 | Identifies user-initiated requests vs automatic requests |
| 10049 | Storable and Cacheable Content | Informational | http://localhost:5000 | Content could be cached by proxies, potential data leakage risk if sensitive |
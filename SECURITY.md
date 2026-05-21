# Security Policy

## Supported Versions

This is a static personal portfolio site. There is no backend, database, or server-side processing.

| Version | Supported |
|---------|-----------|
| V3 (current) | ✅ |
| V2 | ❌ |
| V1 | ❌ |

## Reporting a Vulnerability

If you discover a security issue (e.g. a malicious dependency, XSS in the contact form, or a compromised CDN resource), please:

1. **Do not** open a public GitHub issue
2. Email directly: **moekyawaung@fastmail.com**
3. Include a description of the issue and steps to reproduce

I will respond within 48 hours.

## Security Considerations

- The contact form uses **client-side validation only** — no data is transmitted server-side
- External resources are loaded from trusted CDNs only (Google Fonts, unpkg.com)
- No cookies, localStorage, or tracking scripts are used
- No user data is collected or stored

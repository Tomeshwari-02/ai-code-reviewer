<p align="center">
  <img src="https://img.shields.io/badge/RepoSage-Security%20Policy-critical?style=for-the-badge&logo=shield" alt="Security Policy" />
  <br/>
  <strong>🔒 Keeping RepoSage secure for everyone</strong>
</p>

---

# 🛡️ Security Policy

We take the security of **RepoSage** and our users seriously. This document outlines our supported versions, how to report vulnerabilities, and security best practices for contributors.

---

## 📦 Supported Versions

We provide security patches for the following versions:

| Version | Status | Support Level |
|---------|--------|---------------|
| `latest` (main branch) | ✅ **Active** | Full security support — patches applied promptly |
| Previous minor release | ⚠️ **Maintenance** | Critical security fixes only |
| Older versions | ❌ **End of Life** | No security updates — please upgrade |

> [!IMPORTANT]
> We strongly recommend always running the **latest version** of RepoSage. Security patches are only guaranteed for the current release.

---

## 🚨 Reporting a Vulnerability

If you discover a security vulnerability, please follow responsible disclosure practices. **Do not** disclose it publicly or file a GitHub issue.

### How to Report

1. **📧 Email us directly:**

   **bhoompallykalyanreddy@gmail.com**

2. **Include the following details:**
   - 📝 A clear description of the vulnerability
   - 🔄 Step-by-step instructions to reproduce the issue
   - 🖥️ Environment details (OS, browser, Node.js/Python version)
   - 💥 Potential impact and severity assessment
   - 🔧 Suggested fix or mitigation (if any)
   - 📎 Proof-of-concept (PoC) code or screenshots (if available)

3. **Use this subject line format:**
   ```
   [SECURITY] Brief description of vulnerability
   ```

### What to Expect

| Timeline | Action |
|----------|--------|
| **Within 24 hours** | Acknowledgment of your report |
| **Within 48 hours** | Initial assessment and severity classification |
| **Within 7 days** | Development of a fix or mitigation plan |
| **Within 14 days** | Patched release (for critical/high severity) |

> [!NOTE]
> We are committed to coordinated disclosure. We will work with you to determine an appropriate disclosure timeline after the fix is released.

---

## 📋 Disclosure Policy

RepoSage follows a **Coordinated Vulnerability Disclosure** process:

1. **🔒 Private Report** — Reporter sends details via email (not public issues)
2. **✅ Acknowledgment** — We confirm receipt within 24 hours
3. **🔍 Triage** — We assess severity using [CVSS v3.1](https://www.first.org/cvss/) scoring
4. **🔧 Remediation** — We develop and test a fix internally
5. **📦 Release** — We publish the patched version
6. **📢 Advisory** — We publish a security advisory with credit to the reporter
7. **🏅 Recognition** — Reporter is credited in the advisory (unless anonymity is requested)

### Severity Classification

| Severity | CVSS Score | Response Time |
|----------|------------|---------------|
| 🔴 **Critical** | 9.0 – 10.0 | Patch within 48 hours |
| 🟠 **High** | 7.0 – 8.9 | Patch within 7 days |
| 🟡 **Medium** | 4.0 – 6.9 | Patch within 14 days |
| 🟢 **Low** | 0.1 – 3.9 | Patch in next scheduled release |

---

## 🔐 Security Best Practices for Contributors

When contributing to RepoSage, please follow these security guidelines:

### 🔑 Secrets & Credentials

- **Never** commit API keys, tokens, passwords, or secrets to the repository
- Use environment variables (`.env` files) for all sensitive configuration
- Ensure `.env` files are listed in `.gitignore`
- Use placeholder values in example/config files (e.g., `YOUR_API_KEY_HERE`)

### 🛡️ Code Security

- **Validate all inputs** — Never trust user-supplied data; sanitize and validate
- **Avoid SQL injection** — Use parameterized queries and ORM methods
- **Prevent XSS** — Sanitize HTML output in the frontend; avoid `dangerouslySetInnerHTML`
- **Secure dependencies** — Run `npm audit` and `pip audit` before submitting PRs
- **Use HTTPS** — All external API calls must use HTTPS endpoints
- **Minimize permissions** — Request only the GitHub OAuth scopes you need

### 📦 Dependency Management

- Keep dependencies up to date with `npm update` and `pip install --upgrade`
- Review new dependencies before adding them — prefer well-maintained packages
- Run `npm audit fix` to resolve known vulnerabilities in Node.js packages
- Pin dependency versions in production environments

### 🔒 Authentication & Authorization

- Never store tokens in localStorage — use httpOnly cookies or secure session storage
- Implement proper rate limiting on all API endpoints
- Use CSRF protection for state-changing requests

---

## 📚 Security Resources

- [OWASP Top 10](https://owasp.org/www-project-top-ten/) — Most critical web application security risks
- [Node.js Security Checklist](https://blog.risingstack.com/node-js-security-checklist/) — Best practices for Node.js
- [Python Security Best Practices](https://snyk.io/blog/python-security-best-practices-cheat-sheet/) — Secure Python development
- [GitHub Security Advisories](https://docs.github.com/en/code-security/security-advisories) — Managing security advisories

---

## 🙏 Acknowledgments

We sincerely appreciate the efforts of security researchers and contributors who help keep RepoSage safe. Responsible reporters will be:

- 🏅 Credited in our security advisories
- 📝 Listed in our Hall of Fame (with consent)
- 💌 Thanked by the maintainer team

---

<p align="center">
  <strong>🔒 Security is everyone's responsibility.</strong>
  <br/>
  Thank you for helping keep <strong>RepoSage</strong> safe for the community.
  <br/><br/>
  Made with ❤️ by <strong>RepoSage</strong> &amp; the open-source community
</p>

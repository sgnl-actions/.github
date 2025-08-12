# Security Policy

## Supported Versions

We release patches for security vulnerabilities. Which versions are eligible for receiving such patches depends on the CVSS v3.0 Rating:

| Version | Supported          |
| ------- | ------------------ |
| latest  | :white_check_mark: |
| < latest| :x:                |

## Reporting a Vulnerability

We take the security of our actions seriously. If you believe you have found a security vulnerability in any sgnl-actions repository, please report it to us as described below.

### Please do NOT:
- Open a public GitHub issue
- Disclose the vulnerability publicly before a fix is available

### Please DO:
- Email your findings to security@sgnl.ai
- Include the following information:
  - Type of issue (e.g., buffer overflow, SQL injection, cross-site scripting, etc.)
  - Full paths of source file(s) related to the manifestation of the issue
  - The location of the affected source code (tag/branch/commit or direct URL)
  - Any special configuration required to reproduce the issue
  - Step-by-step instructions to reproduce the issue
  - Proof-of-concept or exploit code (if possible)
  - Impact of the issue, including how an attacker might exploit it

### What to expect:
- We will acknowledge receipt of your vulnerability report within 48 hours
- We will send a more detailed response within 72 hours indicating the next steps
- We will keep you informed of the progress towards fixing the vulnerability
- We will notify you when the vulnerability is fixed

## Security Best Practices for Actions

When using SGNL actions in your workflows:

1. **Pin to specific versions**: Always use a specific version tag rather than `@main`
   ```yaml
   uses: sgnl-actions/okta-create-user@v1.0.0  # Good
   uses: sgnl-actions/okta-create-user@main     # Avoid
   ```

2. **Use secrets properly**: Never hardcode credentials
   ```yaml
   with:
     api_token: ${{ secrets.OKTA_API_TOKEN }}  # Good
     api_token: "SSWS 00xxx..."                 # Never do this
   ```

3. **Review permissions**: Ensure the action only has the permissions it needs

4. **Audit dependencies**: Regularly review and update action dependencies

## Security Features

All sgnl-actions repositories include:
- Automated dependency updates via Dependabot
- Security vulnerability scanning via GitHub Security
- CodeQL analysis for code security issues
- Secret scanning to prevent credential leaks
- Required code reviews for all changes

## Contact

For any security concerns, please contact security@sgnl.ai
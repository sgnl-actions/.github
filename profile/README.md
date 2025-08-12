# SGNL Actions

**Enterprise-grade identity and security automation actions for the SGNL Job Service**

## 🎯 Overview

SGNL Actions is a collection of JavaScript-based automation actions designed for identity and access management, security operations, and compliance workflows. These actions integrate with major identity providers, SaaS applications, and security platforms to enable automated provisioning, deprovisioning, access reviews, and security response workflows.

## 🚀 Quick Start

### Using an Action in Your Workflow

Actions are executed through the SGNL's CAEP Hub feature.

## 📚 Available Actions

### Identity Management
- **[okta-user-provisioning](https://github.com/sgnl-actions/okta-user-provisioning)** - Create and manage Okta users
- **[okta-user-deprovisioning](https://github.com/sgnl-actions/okta-user-deprovisioning)** - Deactivate and remove Okta users
- **[okta-group-management](https://github.com/sgnl-actions/okta-group-management)** - Manage Okta group memberships
- **[azure-ad-sync](https://github.com/sgnl-actions/azure-ad-sync)** - Synchronize users with Azure Active Directory
- **[google-workspace-mgmt](https://github.com/sgnl-actions/google-workspace-mgmt)** - Manage Google Workspace users and groups

### Security Operations
- **[session-termination](https://github.com/sgnl-actions/session-termination)** - Terminate active sessions across platforms
- **[access-review](https://github.com/sgnl-actions/access-review)** - Automated access certification workflows
- **[caep-event-handler](https://github.com/sgnl-actions/caep-event-handler)** - Process CAEP security events

### Example & Templates
- **[hello-world](https://github.com/sgnl-actions/hello-world)** - Simple example action demonstrating core concepts
- **[javascript-template](https://github.com/sgnl-actions/javascript-template)** - Template repository for creating new actions

## 🏗️ Architecture

### Action Structure
Each action follows a consistent structure:

```
action-name/
├── src/
│   └── script.mjs          # Main action logic (ES6)
├── dist/
│   └── index.js           # Built distribution (CommonJS)
├── tests/
│   └── script.test.js     # Unit tests (80%+ coverage)
├── examples/
│   └── usage.json         # Example job requests
├── metadata.yaml          # Action configuration
├── package.json          # Dependencies and scripts
└── README.md            # Documentation
```

### Execution Model
1. **Job Submission** - Jobs are submitted to the SGNL Job Service with action reference and inputs
2. **Worker Execution** - Worker pods fetch actions from GitHub and execute in isolated Node.js 22 containers
3. **Event Handlers** - Actions implement three handlers:
   - `invoke` (required) - Main business logic
   - `error` (optional) - Recovery and retry logic
   - `halt` (optional) - Cleanup on termination

### Error Handling
Actions use a simplified error model:
- **Default behavior** - All errors are retryable
- **Custom recovery** - Optional `error` handler for specific retry logic
- **Fatal errors** - Error handler can re-throw to stop retries

## 🔧 Development

### Creating a New Action

1. **Use the template**:
   ```bash
   gh repo create sgnl-actions/my-action --public \
     --template sgnl-actions/javascript-template --clone
   cd my-action
   npm install
   ```

2. **Implement your logic** in `src/script.mjs`:
   ```javascript
   export default {
     invoke: async (params, context) => {
       // Your action logic here
       const { apiKey } = context.secrets;
       const { email } = params;
       
       // Make API calls, process data, etc.
       const result = await createUser(email, apiKey);
       
       return { 
         status: 'success',
         userId: result.id 
       };
     }
   }
   ```

3. **Configure metadata** in `metadata.yaml`:
   ```yaml
   name: my-action
   description: Description of what your action does
   version: 1.0.0
   inputs:
     - name: email
       type: string
       required: true
   outputs:
     - name: userId
       type: string
   secrets:
     - name: API_KEY
       description: API key for service
   ```

4. **Test and build**:
   ```bash
   npm test           # Run tests (80%+ coverage required)
   npm run build      # Build CommonJS distribution
   ```

### Development Standards

- **Node.js 22** - Use modern ES6+ features
- **ES6 Modules** - Write in ESM, build to CommonJS
- **80% Test Coverage** - Comprehensive unit testing required
- **No External Dependencies** - Use native Node.js APIs when possible
- **Security First** - Never hardcode secrets, validate all inputs
- **Clear Documentation** - Every action must have complete README

## 🔒 Security

### Best Practices
- **Secrets Management** - All credentials passed via `context.secrets`
- **Input Validation** - Validate and sanitize all inputs
- **URL Encoding** - Prevent injection attacks
- **HTTPS Only** - Never use unencrypted connections
- **Audit Logging** - Log security-relevant events

### Authentication Patterns
```javascript
// OAuth Bearer Token
headers: { 'Authorization': `Bearer ${context.secrets.OAUTH_TOKEN}` }

// API Key
headers: { 'X-API-Key': context.secrets.API_KEY }

// Okta SSWS
headers: { 'Authorization': `SSWS ${context.secrets.OKTA_TOKEN}` }
```

## 📋 Requirements

### Runtime
- Node.js 22 runtime environment
- SGNL CAEP Hub for execution

### Development
- Node.js 22+
- npm or yarn
- Git

## 🤝 Contributing

### Contribution Process
1. Fork the repository
2. Create a feature branch
3. Implement changes with tests
4. Ensure 80%+ test coverage
5. Submit pull request

### Code Review Checklist
- [ ] Security review (secrets, validation, encoding)
- [ ] Test coverage meets 80% minimum
- [ ] Documentation is complete
- [ ] Error handling is comprehensive
- [ ] Follows established patterns

## 📖 Documentation

### Action Documentation
Each action repository includes:
- **README.md** - Complete usage documentation
- **metadata.yaml** - Input/output specifications
- **examples/** - Sample job requests
- **CHANGELOG.md** - Version history

## 📊 Status

## 📝 License

All actions in this organization are provided under the MIT License unless otherwise specified.

## 🆘 Support

- **Issues** - Report bugs in individual action repositories
- **Discussions** - Use GitHub Discussions for questions
- **Security** - Report security issues to security@sgnl.ai

---
&copy; 2025 SGNL.ai, Inc.

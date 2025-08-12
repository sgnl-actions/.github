# SGNL Actions

**Enterprise-grade identity and security automation actions for SGNL's CAEP Hub**

## 🎯 Overview

SGNL Actions is a collection of JavaScript-based automation actions designed for identity and access management, security operations, and compliance workflows. These actions integrate with major identity providers, SaaS applications, and security platforms to enable automated provisioning, deprovisioning, access reviews, and security response workflows.

## 🚀 Quick Start

### Using an Action in Your Workflow

Actions are executed through SGNL's CAEP Hub feature.

## 📚 Available Actions

### Session Management

| Service | Action | Description |
|---------|--------|-------------|
| AWS | [aws-revoke-session](https://github.com/sgnl-actions/aws-revoke-session) | Terminate AWS Identity Center sessions |
| AWS | [aws-revoke-user-access-tokens](https://github.com/sgnl-actions/aws-revoke-user-access-tokens) | Revoke AWS user access tokens |
| Azure AD | [aad-revoke-session](https://github.com/sgnl-actions/aad-revoke-session) | Revoke Azure AD sign-in sessions |
| Box | [box-revoke-session](https://github.com/sgnl-actions/box-revoke-session) | Terminate Box sessions |
| Google | [google-revoke-session](https://github.com/sgnl-actions/google-revoke-session) | Revoke Google Workspace sessions |
| HashiCorp | [hashicorp-boundary-cancel-sessions](https://github.com/sgnl-actions/hashicorp-boundary-cancel-sessions) | Cancel Boundary sessions |
| Okta | [okta-revoke-session](https://github.com/sgnl-actions/okta-revoke-session) | Terminate active Okta user sessions |
| Salesforce | [salesforce-revoke-session](https://github.com/sgnl-actions/salesforce-revoke-session) | Invalidate Salesforce sessions |
| Slack | [slack-revoke-session](https://github.com/sgnl-actions/slack-revoke-session) | Revoke Slack authentication |
| Snowflake | [snowflake-revoke-session](https://github.com/sgnl-actions/snowflake-revoke-session) | Terminate Snowflake sessions |
| Zoom | [zoom-revoke-session](https://github.com/sgnl-actions/zoom-revoke-session) | Invalidate Zoom sessions |

### User Lifecycle Management

| Service | Action | Description |
|---------|--------|-------------|
| Azure AD | [aad-disable-user](https://github.com/sgnl-actions/aad-disable-user) | Disable Azure AD user account |
| Azure AD | [aad-enable-user](https://github.com/sgnl-actions/aad-enable-user) | Enable Azure AD user account |
| Google | [google-delete-workforce-user](https://github.com/sgnl-actions/google-delete-workforce-user) | Delete Google Workspace user |
| Google | [google-undelete-workforce-user](https://github.com/sgnl-actions/google-undelete-workforce-user) | Restore deleted Google user |
| Okta | [okta-create-user](https://github.com/sgnl-actions/okta-create-user) | Create new Okta user |
| Okta | [okta-suspend-user](https://github.com/sgnl-actions/okta-suspend-user) | Suspend Okta user account |
| Okta | [okta-unsuspend-user](https://github.com/sgnl-actions/okta-unsuspend-user) | Unsuspend Okta user account |
| Okta | [okta-update-user](https://github.com/sgnl-actions/okta-update-user) | Update Okta user by login |
| Okta | [okta-update-user-by-id](https://github.com/sgnl-actions/okta-update-user-by-id) | Update Okta user by ID |
| SailPoint | [sailpoint-identity-now-disable-account](https://github.com/sgnl-actions/sailpoint-identity-now-disable-account) | Disable SailPoint account |
| SailPoint | [sailpoint-identity-now-enable-account](https://github.com/sgnl-actions/sailpoint-identity-now-enable-account) | Enable SailPoint account |

### Access Management

| Service | Action | Description |
|---------|--------|-------------|
| AWS | [aws-add-to-identity-center-group](https://github.com/sgnl-actions/aws-add-to-identity-center-group) | Add user to AWS Identity Center group |
| AWS | [aws-remove-from-identity-center-group](https://github.com/sgnl-actions/aws-remove-from-identity-center-group) | Remove user from AWS Identity Center group |
| Azure AD | [aad-add-to-group](https://github.com/sgnl-actions/aad-add-to-group) | Add user to Azure AD group |
| Azure AD | [aad-assign-role-to-user](https://github.com/sgnl-actions/aad-assign-role-to-user) | Assign Azure AD directory role |
| Azure AD | [aad-remove-from-group](https://github.com/sgnl-actions/aad-remove-from-group) | Remove user from Azure AD group |
| Azure AD | [aad-unassign-role-from-user](https://github.com/sgnl-actions/aad-unassign-role-from-user) | Remove Azure AD directory role |
| HashiCorp | [hashicorp-boundary-add-user-to-group](https://github.com/sgnl-actions/hashicorp-boundary-add-user-to-group) | Add user to Boundary group |
| HashiCorp | [hashicorp-boundary-remove-user-from-group](https://github.com/sgnl-actions/hashicorp-boundary-remove-user-from-group) | Remove user from Boundary group |
| Okta | [okta-assign-user-to-group](https://github.com/sgnl-actions/okta-assign-user-to-group) | Add user to Okta group |
| Okta | [okta-unassign-user-from-group](https://github.com/sgnl-actions/okta-unassign-user-from-group) | Remove user from Okta group |
| SailPoint | [sailpoint-identity-now-grant-access](https://github.com/sgnl-actions/sailpoint-identity-now-grant-access) | Grant access in SailPoint |
| SailPoint | [sailpoint-identity-now-revoke-access](https://github.com/sgnl-actions/sailpoint-identity-now-revoke-access) | Revoke access in SailPoint |
| Salesforce | [salesforce-add-to-permission-set](https://github.com/sgnl-actions/salesforce-add-to-permission-set) | Assign Salesforce permission set |
| Salesforce | [salesforce-remove-from-permission-set](https://github.com/sgnl-actions/salesforce-remove-from-permission-set) | Remove Salesforce permission set |

### Messaging & Communication

| Service | Action | Description |
|---------|--------|-------------|
| Slack | [slack-send-direct-message](https://github.com/sgnl-actions/slack-send-direct-message) | Send direct message in Slack |
| Slack | [slack-send-message](https://github.com/sgnl-actions/slack-send-message) | Send message to Slack channel |

### Generic & Utility Actions

| Type | Action | Description |
|------|--------|-------------|
| HTTP | [generic-webhook](https://github.com/sgnl-actions/generic-webhook) | Execute custom HTTP requests |

### Templates & Examples

| Type | Repository | Description |
|------|------------|-------------|
| Example | [hello-world](https://github.com/sgnl-actions/hello-world) | Simple example action demonstrating core concepts |
| Template | [javascript-template](https://github.com/sgnl-actions/javascript-template) | Template repository for creating new actions |

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
1. **Job Submission** - Jobs are submitted to SGNL's CAEP Hub with action reference and inputs
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

### Production Readiness
All completed actions are:
- ✅ Fully tested with 80%+ coverage
- ✅ Security reviewed
- ✅ Performance optimized
- ✅ Production ready

### By Service
| Service | Actions | Coverage |
|---------|---------|----------|
| Okta | 8 | Session, User, Group Management |
| Azure AD | 7 | Session, User, Group, Role Management |
| AWS | 4 | Session, Token, Group Management |
| Google | 3 | Session, User Management |
| Salesforce | 3 | Session, Permission Management |
| SailPoint | 4 | Account, Access Management |
| HashiCorp | 3 | Session, Group Management |
| Slack | 3 | Session, Messaging |
| Box | 1 | Session Management |
| Zoom | 1 | Session Management |
| Snowflake | 1 | Session Management |
| Generic | 1 | HTTP Webhooks |

## 📝 License

All actions in this organization are provided under the MIT License unless otherwise specified.

## 🆘 Support

- **Issues** - Report bugs in individual action repositories
- **Discussions** - Use GitHub Discussions for questions
- **Security** - Report security issues to security@sgnl.ai

---
&copy; 2025 SGNL.ai, Inc.

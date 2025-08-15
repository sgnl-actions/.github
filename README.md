# SGNL Actions Organization Configuration

This repository contains organization-wide configurations for the sgnl-actions GitHub organization.

## 📊 Organization Status

- **Total Repositories**: 42 action repositories + 2 special repos (.github, javascript-template)
- **Languages**: JavaScript/Node.js
- **Dependencies**: All repos updated to Jest v30, @rollup/plugin-node-resolve v16
- **Test Coverage**: All repositories have passing tests with 80%+ coverage requirement
- **Security**: Dependabot enabled, secret scanning active, CodeQL available

## 📦 Available Actions

### Azure Active Directory (AAD)
| Action | Description | Repository |
|--------|-------------|------------|
| Add to Group | Add user to AAD group | [aad-add-to-group](https://github.com/sgnl-actions/aad-add-to-group) |
| Assign Role | Assign role to user | [aad-assign-role-to-user](https://github.com/sgnl-actions/aad-assign-role-to-user) |
| Disable User | Disable AAD user account | [aad-disable-user](https://github.com/sgnl-actions/aad-disable-user) |
| Enable User | Enable AAD user account | [aad-enable-user](https://github.com/sgnl-actions/aad-enable-user) |
| Remove from Group | Remove user from AAD group | [aad-remove-from-group](https://github.com/sgnl-actions/aad-remove-from-group) |
| Revoke Session | Revoke user sessions | [aad-revoke-session](https://github.com/sgnl-actions/aad-revoke-session) |
| Unassign Role | Remove role from user | [aad-unassign-role-from-user](https://github.com/sgnl-actions/aad-unassign-role-from-user) |

### AWS
| Action | Description | Repository |
|--------|-------------|------------|
| Add to Identity Center Group | Add user to AWS Identity Center group | [aws-add-to-identity-center-group](https://github.com/sgnl-actions/aws-add-to-identity-center-group) |
| Remove from Identity Center Group | Remove user from AWS Identity Center group | [aws-remove-from-identity-center-group](https://github.com/sgnl-actions/aws-remove-from-identity-center-group) |
| Revoke Session | Revoke AWS user sessions | [aws-revoke-session](https://github.com/sgnl-actions/aws-revoke-session) |
| Revoke User Access Tokens | Revoke AWS user access tokens | [aws-revoke-user-access-tokens](https://github.com/sgnl-actions/aws-revoke-user-access-tokens) |

### Okta
| Action | Description | Repository |
|--------|-------------|------------|
| Assign to Group | Assign user to Okta group | [okta-assign-user-to-group](https://github.com/sgnl-actions/okta-assign-user-to-group) |
| Create User | Create new Okta user | [okta-create-user](https://github.com/sgnl-actions/okta-create-user) |
| Device Risk Change | Handle device risk changes | [okta-device-risk-change](https://github.com/sgnl-actions/okta-device-risk-change) |
| Revoke Session | Revoke user sessions | [okta-revoke-session](https://github.com/sgnl-actions/okta-revoke-session) |
| Suspend User | Suspend Okta user account | [okta-suspend-user](https://github.com/sgnl-actions/okta-suspend-user) |
| Unassign from Group | Remove user from Okta group | [okta-unassign-user-from-group](https://github.com/sgnl-actions/okta-unassign-user-from-group) |
| Unsuspend User | Reactivate suspended user | [okta-unsuspend-user](https://github.com/sgnl-actions/okta-unsuspend-user) |
| Update User | Update user profile | [okta-update-user](https://github.com/sgnl-actions/okta-update-user) |
| Update User by ID | Update user by ID | [okta-update-user-by-id](https://github.com/sgnl-actions/okta-update-user-by-id) |
| User Risk Change | Handle user risk changes | [okta-user-risk-change](https://github.com/sgnl-actions/okta-user-risk-change) |

### Google Workspace
| Action | Description | Repository |
|--------|-------------|------------|
| Delete Workforce User | Delete Google Workforce user | [google-delete-workforce-user](https://github.com/sgnl-actions/google-delete-workforce-user) |
| Revoke Session | Revoke user sessions | [google-revoke-session](https://github.com/sgnl-actions/google-revoke-session) |
| Undelete Workforce User | Restore deleted user | [google-undelete-workforce-user](https://github.com/sgnl-actions/google-undelete-workforce-user) |

### SailPoint IdentityNow
| Action | Description | Repository |
|--------|-------------|------------|
| Disable Account | Disable IdentityNow account | [sailpoint-identity-now-disable-account](https://github.com/sgnl-actions/sailpoint-identity-now-disable-account) |
| Enable Account | Enable IdentityNow account | [sailpoint-identity-now-enable-account](https://github.com/sgnl-actions/sailpoint-identity-now-enable-account) |
| Grant Access | Grant access entitlement | [sailpoint-identity-now-grant-access](https://github.com/sgnl-actions/sailpoint-identity-now-grant-access) |
| Revoke Access | Revoke access entitlement | [sailpoint-identity-now-revoke-access](https://github.com/sgnl-actions/sailpoint-identity-now-revoke-access) |

### Salesforce
| Action | Description | Repository |
|--------|-------------|------------|
| Add to Permission Set | Add user to permission set | [salesforce-add-to-permission-set](https://github.com/sgnl-actions/salesforce-add-to-permission-set) |
| Remove from Permission Set | Remove user from permission set | [salesforce-remove-from-permission-set](https://github.com/sgnl-actions/salesforce-remove-from-permission-set) |
| Revoke Session | Revoke user sessions | [salesforce-revoke-session](https://github.com/sgnl-actions/salesforce-revoke-session) |

### HashiCorp Boundary
| Action | Description | Repository |
|--------|-------------|------------|
| Add User to Group | Add user to Boundary group | [hashicorp-boundary-add-user-to-group](https://github.com/sgnl-actions/hashicorp-boundary-add-user-to-group) |
| Cancel Sessions | Cancel active sessions | [hashicorp-boundary-cancel-sessions](https://github.com/sgnl-actions/hashicorp-boundary-cancel-sessions) |
| Remove User from Group | Remove user from Boundary group | [hashicorp-boundary-remove-user-from-group](https://github.com/sgnl-actions/hashicorp-boundary-remove-user-from-group) |

### Collaboration Tools
| Action | Description | Repository |
|--------|-------------|------------|
| Box - Revoke Session | Revoke Box user sessions | [box-revoke-session](https://github.com/sgnl-actions/box-revoke-session) |
| Slack - Revoke Session | Revoke Slack user sessions | [slack-revoke-session](https://github.com/sgnl-actions/slack-revoke-session) |
| Slack - Send Direct Message | Send DM to Slack user | [slack-send-direct-message](https://github.com/sgnl-actions/slack-send-direct-message) |
| Slack - Send Message | Send message to Slack channel | [slack-send-message](https://github.com/sgnl-actions/slack-send-message) |
| Zoom - Revoke Session | Revoke Zoom user sessions | [zoom-revoke-session](https://github.com/sgnl-actions/zoom-revoke-session) |

### Data Platforms
| Action | Description | Repository |
|--------|-------------|------------|
| Snowflake - Revoke Session | Revoke Snowflake sessions | [snowflake-revoke-session](https://github.com/sgnl-actions/snowflake-revoke-session) |

### Integration Tools
| Action | Description | Repository |
|--------|-------------|------------|
| Generic SSE Transmitter | Send Server-Sent Events | [generic-sse-transmitter](https://github.com/sgnl-actions/generic-sse-transmitter) |
| Generic Webhook | Send webhook notifications | [generic-webhook](https://github.com/sgnl-actions/generic-webhook) |

## 📁 Repository Structure

```
.github/
├── .github/
│   └── dependabot.yml              # Default Dependabot configuration
├── workflow-templates/             # Reusable workflow templates
│   ├── codeql-analysis.yml        # CodeQL security scanning
│   └── dependency-review.yml      # Dependency vulnerability review
├── ISSUE_TEMPLATE/                # Issue templates
│   ├── bug_report.yml            # Bug report template
│   └── feature_request.yml       # Feature request template
├── pull_request_template.md       # Pull request template
└── SECURITY.md                    # Security policy
```

## 🔒 Security Features

### Organization-wide Settings
- **Branch Protection**: Default branch protection rules via organization rulesets
- **Dependabot**: Automated dependency updates and security fixes
- **Secret Scanning**: Prevents accidental credential commits
- **Push Protection**: Blocks pushes containing secrets
- **Security Alerts**: Vulnerability notifications for dependencies

### Available Workflows
Teams can use these workflow templates in their repositories:
- **CodeQL Analysis**: Static code analysis for security vulnerabilities
- **Dependency Review**: Reviews PRs for vulnerable dependencies and license issues

## 🚀 Getting Started

### For Repository Maintainers

1. **Enable Security Features**: Most features are automatically enabled for new repositories

2. **Use Workflow Templates**: 
   - Go to Actions → New workflow
   - Choose from organization templates

3. **Customize Dependabot** (if needed):
   - Create `.github/dependabot.yml` in your repo to override defaults
   - The organization config applies only if no local config exists

### For Contributors

1. **Follow Security Policy**: Read [SECURITY.md](SECURITY.md) for vulnerability reporting
2. **Use PR Template**: Automatically applied to all pull requests
3. **Report Issues**: Use the provided issue templates

## 📋 Organization Standards

### Branch Protection Rules
All repositories have these protections on their default branch:
- Requires 1 approving review
- Dismisses stale reviews on new commits
- Requires conversation resolution
- Prevents force pushes
- Prevents branch deletion

### Dependency Management
- Weekly Dependabot updates for npm packages
- Security updates auto-enabled
- Grouped minor/patch updates to reduce PR noise
- GitHub Actions dependencies also monitored

### Code Quality
- CodeQL analysis for JavaScript security issues
- Dependency license compliance checking
- Automated security fixes for known vulnerabilities

## 🔧 Maintenance

This repository is maintained by the SGNL Actions team. To propose changes:
1. Open an issue describing the proposed change
2. Submit a PR with the changes
3. Changes will apply organization-wide once merged

## 📝 License

All configurations in this repository are available under the same license as the sgnl-actions projects.

## 🤝 Support

For questions or issues:
- Open an issue in this repository for org-wide concerns
- Contact security@sgnl.ai for security issues
- Open issues in specific action repositories for action-specific problems
# SGNL Actions Organization Configuration

This repository contains organization-wide configurations for the sgnl-actions GitHub organization.

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
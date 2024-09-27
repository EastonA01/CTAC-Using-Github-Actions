# CTAC-Using-Github-Actions

# CI/CD Workflow Documentation
## Continuous Integration (CI)
The CI pipeline is triggered on every push to the main branch. It performs the following actions:
1. **Checkout code**: Fetches the code from the repository.
2. **Install dependencies**: Installs project dependencies using npm.
3. **Run tests**: Executes the test suite.
4. **Build project**: Builds the application (if applicable).
5. **Archive artifacts**: Stores build artifacts (optional).

## Continuous Deployment (CD)
After a successful build and testing, the CD pipeline deploys the application to Github Pages. It:
1. Deploys the code to Github Pages using the gh-pages API key.
2. The deployment is automatic once tests pass.

## Secrets Configuration
- Secret's configuration shouldn't be a problem as your respective gh-pages API key should be tied to your the account default and should not need to be manually set

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
After a successful build and testing, the CD pipeline deploys the application to Heroku. It:
1. Installs the Heroku CLI.
2. Deploys the code to Heroku using the Heroku API key.
3. The deployment is automatic once tests pass.

## Secrets Configuration
- `HEROKU_API_KEY`: Used to authenticate deployment to Heroku.

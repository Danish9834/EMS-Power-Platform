# EMS Unmanaged Solution

This folder contains the unpacked Microsoft Power Platform solution source for the Event Management System (EMS).

## Solution Contents

- **CanvasApps/** — Canvas Power Apps application components.
- **Workflows/** — Solution workflow components.
- **EMS--Power BI/** — Files included in the extracted solution folder related to Power BI.

The solution metadata files are:

- `[Content_Types].xml`
- `customizations.xml`
- `solution.xml`

## Purpose

This unmanaged solution source is maintained in GitHub for version control, documentation, and future CI/CD integration.

## Development and Deployment

1. Make application changes in the development environment.
2. Update and validate the solution components.
3. Export the unmanaged solution from the development environment.
4. Unpack the solution source and commit the updated files to GitHub.
5. Validate the solution before preparing a managed deployment artifact.
6. Import the managed solution into the target production environment after configuring the required connections and environment variables.

## Important Notes

- Use the unmanaged solution for development and source maintenance.
- Use a managed solution for deployment to production.
- Configure environment-specific connections and environment variables before deployment.
- Do not commit credentials, API keys, secrets, connection strings, or personal data.

## Related Documentation

See the repository root `README.md` for the project overview, features, technology stack, and architecture.

## Status

Source files have been uploaded to GitHub. CI/CD configuration and production deployment are pending validation.

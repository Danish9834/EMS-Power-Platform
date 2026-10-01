# Event Management System (EMS)

A business application built using Microsoft Power Platform to manage events, registrations, attendees, and event analytics.

## Project Overview

The Event Management System (EMS) provides an application for browsing and managing events, registering attendees, and administering event-related information. It combines Power Apps, Dataverse, Power Automate, SQL Server, and Power BI.

## Features

- **Event Management:** Create, view, update, and manage event information.
- **Event Registration:** Support event registration through the Power Apps interface.
- **Attendee Management:** Manage attendee records and event-related users.
- **Admin Dashboard:** Centralized administration of event information and records.
- **Dataverse Integration:** Store and manage application data.
- **SQL Server Integration:** Support ticket sales and transaction records where configured.
- **Power Automate:** Automate confirmation emails and other configured workflows.
- **Power BI Analytics:** Visualize event-related data through reports and dashboards.
- **Search and Filtering:** Find records efficiently.
- **User Experience:** Provide navigation, status messages, and administrative actions.

## Technology Stack

| Technology               | Purpose                                  |
| ------------------------ | ---------------------------------------- |
| Microsoft Power Apps     | Application UI and business operations   |
| Microsoft Dataverse      | Application data storage                 |
| Microsoft Power Automate | Workflow automation and notifications    |
| Microsoft SQL Server     | Ticket sales and transaction data        |
| Microsoft Power BI       | Reports and analytics                    |
| GitHub                   | Source control and project documentation |
| GitHub Actions           | Planned CI/CD automation                 |

## Architecture

```text
Users and Administrators
          |
          v
     Power Apps
          |
          v
       Dataverse
          |
     +----+----+
     |         |
     v         v
Power Automate  SQL Server
     |         |
     v         |
Email / Alerts |
     +----+----+
          |
          v
       Power BI
   Reports and Analytics
```

*The architecture is a conceptual overview; actual connections depend on the configured application components.*

## Repository Structure

```text
EMS-Power-Platform/
├── README.md
├── PowerPlatform/
│   └── EMS-Unmanaged/
│       ├── CanvasApps/
│       ├── Workflows/
│       ├── EMS--Power BI/
│       ├── [Content_Types].xml
│       ├── customizations.xml
│       └── solution.xml
├── EMS Screenshots/
└── .github/
    └── workflows/
```

*The repository structure may evolve as source files, documentation, and CI/CD workflows are added.*

## Screenshots

See the `EMS Screenshots` folder for application screenshots, including the available event management and administration screens.

## Deployment Status

- [x] Unmanaged solution exported and source files uploaded to GitHub.
- [x] Initial project folders and files committed.
- [ ] Complete source structure verification.
- [ ] Configure development and production environments.
- [ ] Set up GitHub Actions CI/CD.
- [ ] Validate managed solution deployment in production.

## Getting Started

1. Review the solution source files in `PowerPlatform/EMS-Unmanaged/`.
2. Confirm the required Dataverse tables, applications, workflows, and connection references.
3. Configure environment-specific connections and environment variables.
4. Import and test the solution in an appropriate Power Platform environment.
5. Configure Power BI and SQL Server connectivity as required.

Deployment requires access to the relevant Microsoft Power Platform environment and any required data sources.

## Security

- Do not commit passwords, API keys, client secrets, or connection strings.
- Do not publish real attendee data or confidential business information.
- Store deployment credentials in GitHub Actions Secrets or an appropriate secure credential store.

## Future Improvements

- Automated build and deployment using GitHub Actions.
- Separate development and production environments.
- Automated solution validation.
- Improved event analytics and administration.

## Author

**Syed Danish**

Power Platform Developer

Technologies: Power Apps | Dataverse | Power Automate | Power BI | SQL Server | GitHub

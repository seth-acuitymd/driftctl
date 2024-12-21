# `driftctl` (fork)

## This project was forked from `snyk/driftctl` which is now in maintenance mode

## I ([seth](https://github.com/seth-acuitymd)) am going to see if I can get this project moving again, at least for my own use

## What is `driftctl`?

`driftctl` is a tool that measures infrastructure as code coverage, and tracks infrastructure drift from your Terraform code.

Supports:

- IaC Providers:
  - Terraform
- Cloud Providers:
  - AWS
  - Azure
  - GCP

_some_ GitHub Support?

:warning: - No guarantees on this project, I'm just doing this for my own use and hoping it'll pick up steam

---

# Legacy README

## Contents below this are from the original `snyk/driftctl` project and may not be accurate, current, and may be removed at some point

## Why `driftctl` ?

Infrastructure drift is a blind spot and a source of potential security issues.
Drift can have multiple causes: from team members creating or updating infrastructure through the web console without backporting changes to Terraform, to unexpected actions from authenticated apps and services.

You can't efficiently improve what you don't track. We track coverage for unit tests, why not infrastructure as code coverage?

Spot discrepancies as they happen: `driftctl` is a free and open-source CLI that warns of infrastructure drifts and fills in the missing piece in your DevSecOps toolbox.

## Features

- **Scan** cloud provider and map resources with IaC code
- Analyze diffs, and warn about drift and unwanted unmanaged resources
- Allow users to **ignore** resources
- Multiple output formats

## Links

**[Documentation](https://docs.driftctl.com)**

**[Installation](https://docs.driftctl.com/installation)**

## Contribute

To learn more about compiling driftctl and contributing, please refer to the [contribution guidelines](.github/CONTRIBUTING.md) and the [contributing guide](docs/README.md) for technical details.

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification and is brought to you by these [awesome contributors](CONTRIBUTORS.md).

Build with ❤️️ from 🇫🇷 🇬🇧 🇯🇵 🇬🇷 🇸🇪 🇺🇸 🇷🇪 🇨🇦 🇮🇱 🇩🇪

## Security notice

All Terraform state and Terraform files in this repository are for unit test
purposes only. No running code attempts to access these resources (except to
create and destroy them, in the case of acceptance tests). They are just opaque
strings.

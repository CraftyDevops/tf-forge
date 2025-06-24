# tf-forge

![PyPI Version](https://img.shields.io/pypi/v/tf-forge)
![Python Versions](https://img.shields.io/pypi/pyversions/tf-forge)
![License](https://img.shields.io/pypi/l/tf-forge)

An all-in-one CLI toolkit for managing the Terraform module lifecycle with best practices, from creation to publishing.

`forge` is a command-line tool designed to help DevOps engineers and Infrastructure developers streamline their Terraform module workflow. It automates repetitive tasks, enforces best practices, and integrates key quality checks directly into your development process. Stop wasting time on boilerplate and focus on writing great infrastructure code.

## Key Features

-   🚀 **Create New Modules** (`forge new`): Instantly create a new module with a standardized, best-practice directory structure, including `.gitignore`, `versions.tf`, and example usage.
-   📄 **Automate Documentation** (`forge docs`): Automatically parse your `.tf` files and generate comprehensive documentation for Requirements, Providers, Modules, Inputs, and Outputs, injecting it directly into your `README.md`.
-   🔒 **Lint & Validate** (`forge lint`): Run a suite of checks against your code, including `terraform fmt`, `terraform validate`, and custom checks for hardcoded secrets and module version pinning.
-   🎉 **Publish Releases** (`forge publish`): Interactively publish a new version of your module. The tool helps you choose a version, creates a Git tag, pushes it to the remote, and even helps you create a GitHub Release for it.

## Prerequisites

Before using `tf-forge`, you need to have the following tools installed on your system:

-   **Python 3.8+**
-   **Terraform**
-   **Git**
-   **GitHub CLI (`gh`)** (Optional, only required for the GitHub Release feature in the `publish` command)

## Installation

You can install `tf-forge` directly from PyPI using pip:

```bash
pip install tf-forge
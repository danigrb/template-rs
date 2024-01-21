# template-rs
Opinionated opensource template git repository to start off your rust project.

[![codecov](https://codecov.io/gh/danigrb/template-rs/graph/badge.svg?token=FTH3S4FXGH)](https://codecov.io/gh/danigrb/template-rs)
# Project Template for Rust

This repository serves as a template for Rust projects, streamlining the setup process and ensuring best practices in continuous integration and code coverage.

## Getting Started with the Template

To use this template for your project, simply clone or fork the repository. After obtaining a copy, replace all instances of "template-rs" in the project files with your project's name. This can be done efficiently using a tool like Visual Studio Code's 'Replace All' feature.

## Tarpaulin for Test Coverage

### Introduction to Tarpaulin

[Tarpaulin](https://github.com/xd009642/tarpaulin) is a code coverage tool specifically designed for Rust projects. It helps in assessing the effectiveness of tests by reporting the percentage of code executed during testing.

### Setting Up Tarpaulin

To use Tarpaulin in this template:

1. Ensure you have Rust and Cargo installed.
2. Install Tarpaulin by running `cargo install cargo-tarpaulin`.

### Running Tarpaulin

Execute your tests with Tarpaulin by using the command `cargo tarpaulin`. This will run your test suite and provide a coverage report upon completion.

## GitHub Actions for Build and Test on Pull Requests

### About GitHub Actions

GitHub Actions automate workflows directly in your GitHub repository. For this template, we use Actions to build and test the codebase whenever a new pull request (PR) is made.

### Configuring the Workflow

The `.github/workflows/rust_build_and_test.yml` file contains the workflow configuration. It's set up to trigger on pull requests, executing the build and test processes.

### Workflow Steps

The workflow includes the following steps:

1. Set up the Rust environment.
2. Cache dependencies to speed up builds.
3. Build the project.
4. Run tests.

## Codecov Integration with GitHub Actions

### Introduction to Codecov

[Codecov](https://codecov.io) is a tool that visualizes code coverage and helps ensure that all parts of your code are tested. It's particularly useful in reviewing pull requests.

### Setting Up Codecov

To integrate Codecov with this template:

1. Sign up on [Codecov's website](https://codecov.io) and link your GitHub repository.
2. In your GitHub repository settings, add the `CODECOV_TOKEN` as a secret.

### Configuring GitHub Actions for Codecov

The `.github/workflows/rust_build_and_test.yml` file already includes a step that uploads the coverage report to Codecov. This can be done after the test step using Tarpaulin.

### Adding a Codecov Badge

To add a Codecov badge to your README:

1. Go to your repository page on Codecov.
2. Copy the Markdown code for the badge.
3. Paste it at the top of your `README.md` file.

## Disclaimer

This Rust project template is made for educational purposes.

If you have any suggestions or tips on what should be added, please feel free to reach out info@danielegarbagnati.com .
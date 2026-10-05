# Security Policy

## Supported Versions

This SDK is generated from the Maesn API specification and released frequently. Security fixes are only applied to the latest released version.

Please upgrade to the latest version of `@maesn/typescript-sdk` before reporting an issue.

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues, discussions, or pull requests.**

Instead, report them privately using one of the following channels:

- **GitHub Private Vulnerability Reporting:** use the [Report a vulnerability](https://github.com/maesndev/sdk-typescript/security/advisories/new) button under the repository's **Security** tab.
- **Email:** [dev@maesn.com](mailto:dev@maesn.com)

Please include as much of the following information as possible:

- Type of issue (e.g. credential leakage, injection, insecure transport, dependency vulnerability)
- Affected SDK version(s) and runtime (Node.js, Bun, Deno, browser)
- Location of the affected source code (file path, function, or operation)
- Step-by-step instructions to reproduce the issue
- Proof-of-concept or exploit code, if available
- Impact of the issue and how an attacker might exploit it

## Our Process

- We will acknowledge receipt of your report.
- We will investigate and keep you informed of our progress.
- Once confirmed, we will work on a fix. Because this SDK is generated code, fixes may be applied upstream (API specification or generator configuration) and shipped in the next SDK release.
- We will coordinate public disclosure with you and credit you for the discovery, unless you prefer to remain anonymous.

We ask that you give us a reasonable amount of time to address the issue before any public disclosure.

## Scope

This policy covers the code in this repository (`@maesn/typescript-sdk`). Vulnerabilities in the Maesn API or platform itself should also be reported via the email address above.

## Best Practices for SDK Users

- Never commit API keys or account keys to source control. Load them from environment variables or a secrets manager.
- Do not use this SDK with secret credentials in client-side (browser) code where they can be exposed to end users.
- Keep the SDK and its dependencies up to date.

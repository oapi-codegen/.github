# Security Policy

As a key component in the implementation of API clients and servers, [`oapi-codegen`](https://github.com/oapi-codegen/oapi-codegen) is in an critical position to keep secure.

## Supported versions

Only `oapi-codegen`'s latest minor version is generally supported.

Related: [`oapi-codegen`'s support model (`SUPPORT.md`)](https://github.com/oapi-codegen/oapi-codegen/blob/HEAD/SUPPORT.md)

However, depending on the severity of a given security vulnerability, there may be case(s) where this would lead to a backport of the patch on a currently unsupported version.

## Reporting Security Issues

<!-- Via https://github.com/github/.github/blob/main/SECURITY.md -->

If you believe you have found a security vulnerability in `oapi-codegen` or any of the related projects in [the `oapi-codegen` GitHub organisation](https://github.com/oapi-codegen/), please report it to us through coordinated disclosure.

> [!IMPORTANT]
> **Please do not report security vulnerabilities through public GitHub issues, discussions, or pull requests.**

Please report the vulnerability through the GitHub security advisories page.

For instance, for the core `oapi-codegen` CLI, you would report it [on this page](https://github.com/oapi-codegen/oapi-codegen/security/advisories/).

Please include as much of the information listed below as you can to help us better understand and resolve the issue:

* The type of issue (e.g., buffer overflow, SQL injection, or cross-site scripting)
* Full paths of source file(s) related to the manifestation of the issue
* The location of the affected source code (tag/branch/commit or direct URL)
* Any special configuration required to reproduce the issue
* Step-by-step instructions to reproduce the issue
* Proof-of-concept or exploit code (if possible)
* Impact of the issue, including how an attacker might exploit the issue

This information will help us triage your report more quickly.

## CVEs in dependencies

If a dependency that `oapi-codegen` (or its child projects) contains a CVE, we will look to patch that dependency in the following cases:

- The dependency's CVE is exploitable using static analysis, via [`govulncheck`](https://pkg.go.dev/golang.org/x/vuln/cmd/govulncheck)
- The dependency's CVE requires a mix of some code changes and a version bump to address the CVE
- If we are generally updating dependencies (for instance part of general hygiene or as part of updating dependencies ahead of a release)

> [!NOTE]
> Given the Go ecosystem allows projects to override dependency updates, this allows consumers of `oapi-codegen` to upgrade dependencies separate to `oapi-codegen` making changes upstream.
>
> We will strive to make sure that we do update these dependencies on a regular basis, but until a fix or release is made, it is possible to override the version in your `go.mod`.

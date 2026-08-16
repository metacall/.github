# Security Policy

## Supported Versions

MetaCall is under active development. Security fixes are applied to the latest
release on the `develop` branch and backported to the most recent tagged release.
We do not patch older releases; please update to the latest version.

| Version | Supported          |
| ------- | ------------------ |
| latest (develop) | :white_check_mark: |
| < latest         | :x:                |

## Reporting a Vulnerability

We take security vulnerabilities seriously. If you discover a security issue
in any MetaCall repository, please report it responsibly:

- **Preferred:** Use GitHub's built-in
  [private vulnerability reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing/privately-reporting-a-security-vulnerability)
  on the affected repository (Security tab → "Report a vulnerability").
- **Alternatively:** Email the maintainers at **security@metacall.io**
  (or contact@metacall.io).

Please **do not** open a public GitHub issue for security vulnerabilities.

### What to include

To help us triage and fix the issue quickly, please include:

1. A clear description of the vulnerability and its potential impact.
2. The affected repository, file(s), and line numbers (`path:line`).
3. The MetaCall version or commit hash you tested against.
4. Steps to reproduce or a minimal proof-of-concept.
5. Any suggested remediation (optional but appreciated).

### Response timeline

- **Acknowledgement:** within 72 hours.
- **Initial assessment / triage:** within 7 days.
- **Fix or mitigation:** we aim for 90 days, depending on severity and complexity.
- **Disclosure:** coordinated with the reporter after a fix is released.

We will keep you informed throughout the process and credit you in the
advisory unless you prefer to remain anonymous.

## Scope

### In scope

- All repositories under the
  [MetaCall GitHub organization](https://github.com/metacall), including:
  - [metacall/core](https://github.com/metacall/core) — the polyglot runtime (C, Rust, Python, NodeJS, etc.)
  - [metacall/faas](https://github.com/metacall/faas) — the FaaS platform reimplementation
  - [metacall/deploy](https://github.com/metacall/deploy) — the deployment tool
  - [metacall/protocol](https://github.com/metacall/protocol) — the shared protocol modules
  - [metacall/polyglot-repl](https://github.com/metacall/polyglot-repl) — the polyglot REPL
  - [metacall/metassr](https://github.com/metacall/metassr) — server-side rendering framework
  - All other first-party repositories (excluding forks of upstream projects)
- The MetaCall Hub platform at [dashboard.metacall.io](https://dashboard.metacall.io)
- The MetaCall website at [metacall.io](https://metacall.io)

### Out of scope

- Forks of upstream third-party projects (e.g., `plthook`, `backward-cpp`,
  `homebrew-metacall`, `nixpkgs`, `tinycc`, `brew-pkg`, `ruby-loco`, `ruby-mswin`,
  `nim-packages`). Report those to their respective upstream maintainers.
- Denial of Service via resource exhaustion on shared infrastructure.
- Social engineering, phishing, or physical attacks against MetaCall staff or infrastructure.
- Vulnerabilities in third-party dependencies — report those upstream, or let us
  know so we can update.
- Issues that require root or privileged access to a system already compromised.
- Findings from automated tools without a demonstrated, reproducible impact.
- Missing security headers or best-practice suggestions without a concrete exploit path.

## Safe Harbor

MetaCall supports safe harbor for security researchers who act in good faith and
follow this policy. We will not pursue legal action against individuals who:

- Make a good-faith effort to avoid privacy violations, destruction of data,
  and interruption or degradation of MetaCall services.
- Do not access or modify data that does not belong to them.
- Report vulnerabilities promptly and exclusively to MetaCall through the
  channels above.
- Do not disclose the vulnerability publicly until a fix has been released and
  MetaCall has agreed to a disclosure timeline.

In return, we ask that researchers respect our systems, data, and users.

## Acknowledgements

We are grateful to the security research community. Contributors who report
valid vulnerabilities in accordance with this policy will be acknowledged
(here, in the advisory, or by request) unless they prefer to remain anonymous.

---

This policy is adapted from widely-used responsible disclosure templates and
GitHub's recommended [SECURITY.md](https://docs.github.com/en/code-security/getting-started/adding-a-security-policy-to-your-repository)
guidelines.

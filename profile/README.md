# ltsboot

ltsboot is an open source (Apache License 2.0) long-term-support fork of the **Spring Boot 2.7** line and the portfolio it manages (Spring Framework 5.3, Spring Security 5.7). It receives security fixes (CVEs) and critical bug fixes. It does not add features.

ltsboot is a drop-in replacement: the Java packages (`org.springframework.*`) do not change. Consuming projects change only the version and the groupId.

> **Disclaimer.** ltsboot is not affiliated with, endorsed by, or sponsored by Broadcom Inc. or VMware, Inc. Spring and Spring Boot are trademarks of Broadcom Inc. and are used here only to describe compatibility.

## Scope

- **In scope:** fixes for applicable CVEs and critical bugs.
- **Out of scope:** new features, refactorings, and public API changes.
- **Sources:** only OSS tags and public commits under Apache 2.0. Code, binaries, and diffs from commercial releases are never used.

## Repositories

| Repository | Purpose |
|---|---|
| `ltsboot/boot` | Spring Boot 2.7 fork: Boot, starters, and BOM |
| `ltsboot/framework` | Spring Framework 5.3 fork |
| `ltsboot/security` | Spring Security 5.7 fork |
| `ltsboot/bom` | Dependency override BOM |
| `ltsboot/relocator` | Republishes artifacts to an internal repository with the original coordinates |
| `ltsboot/compat-tests` | Compatibility test applications (Maven and Gradle) |
| `ltsboot/security-advisories` | Public CVE inventory, advisories, and per-CVE specs |
| `ltsboot/.github` | Community health files (this repository) |

## Contributing and security

- Read [CONTRIBUTING.md](https://github.com/ltsboot/.github/blob/main/CONTRIBUTING.md) before opening a pull request. Commits require a `Signed-off-by` line (`git commit -s`).
- To report a vulnerability, follow [SECURITY.md](https://github.com/ltsboot/.github/blob/main/SECURITY.md). Do not open a public issue.

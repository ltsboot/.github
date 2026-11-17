# Contributing to ltsboot

Thank you for your interest in ltsboot. The project maintains the Spring Boot 2.7, Spring Framework 5.3, and Spring Security 5.7 lines with security and critical bug fixes only.

## Scope

- Accepted: fixes for applicable CVEs and critical bugs.
- Not accepted: new features, refactorings, and public API changes. Open an issue first if you are unsure.

## Source provenance

- Patches must come only from open source code under Apache License 2.0: public OSS tags and public commits.
- Never copy code, binaries, or diffs from commercial releases. For example, do not use VMware Tanzu builds of Spring Boot 2.7.19 and later.
- State the source commit or tag in the pull request.

## Developer Certificate of Origin (DCO)

Every commit must include a `Signed-off-by` line certifying the [Developer Certificate of Origin 1.1](https://developercertificate.org/). Add it with the `-s` flag:

```sh
git commit -s -m "Fix CVE-XXXX-YYYY in ClassName"
```

Git adds `Signed-off-by: Your Name <you@example.com>` from your `user.name` and `user.email` settings. Commits without this line fail the DCO check.

## Human review for security patches

- Every security patch requires review and approval by a human maintainer before merge.
- Do not merge security patches automatically or with your own approval only.

## Tests

- Use JUnit 5, AssertJ, and Mockito, the same as the upstream projects.
- Name test classes with the `Tests` suffix (for example, `StringUtilsTests`) and place them in the same package and module as the code under test.
- Every security patch includes a regression test that fails before the patch and passes after it. Include both results in the pull request.
- Run the project formatter and Checkstyle before committing. No existing test may start failing.

## Modification headers

Keep every original copyright and license header intact. In each modified file, add this line directly below the original copyright line:

```
Modifications Copyright 2026 the ltsboot contributors.
```

New files use `Copyright 2026 the ltsboot contributors.` followed by the standard Apache License header.

## Changelog

Add every changed file to `CHANGES.md` in the repository, with its change and the related CVE or issue.

## Pull requests

Use the pull request template. A pull request must be complete before review starts.

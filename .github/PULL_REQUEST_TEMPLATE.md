## Summary

<!-- What does this change fix, and why? -->

## Linked CVE or issue

<!-- Required. For example: CVE-XXXX-YYYY or #123 -->

## Source

<!-- Upstream OSS tag or public commit this patch comes from. -->

## Test evidence

<!-- Regression test name and results before and after the patch. -->

- Fails before the patch: <!-- command and result -->
- Passes after the patch: <!-- command and result -->

## Checklist

- [ ] Every commit has a `Signed-off-by` line (DCO; `git commit -s`).
- [ ] For a security fix, a regression test fails before the patch and passes after it.
- [ ] Every modified file has `Modifications Copyright 2026 the ltsboot contributors.` below the original copyright line, and original headers are unchanged.
- [ ] `CHANGES.md` lists every changed file, with the change and the CVE or issue.
- [ ] Tests use JUnit 5, AssertJ, and Mockito, and test classes end with `Tests`.
- [ ] The formatter and Checkstyle pass, and no existing test fails.
- [ ] The patch contains no code, binaries, or diffs from commercial releases.
- [ ] For a security fix, a human maintainer has reviewed and approved it before merge.

# Security Policy

ltsboot is an independent, open source (Apache-2.0) long-term support fork compatible with Spring Boot 2.7.
It is not affiliated with, endorsed by or sponsored by Broadcom Inc. or VMware.

## Reporting a vulnerability

Report vulnerabilities privately through GitHub private vulnerability reporting:

1. Open the **Security** tab of the affected repository (`ltsboot/boot`, `ltsboot/framework`, `ltsboot/security`, or `ltsboot/bom`).
2. Select **Report a vulnerability**.

Do not open a public issue, pull request, or discussion for a suspected vulnerability.

Include the affected component and version, a description of the impact, steps to reproduce, and a proposed fix if you have one.

If you cannot use GitHub private vulnerability reporting, e-mail **fernando@morais.net.br** with the subject
`[ltsboot security]`. Do not send vulnerability details to any public mailing list or chat.

## Supported versions

Only the latest release of each line receives security fixes.

| Line | Base | Supported |
|---|---|---|
| Boot 2.7 (ltsboot; fork compatible with Spring Boot 2.7) | `2.7.18.x` | Yes |
| Framework 5.3 (ltsboot; fork compatible with Spring Framework 5.3) | `5.3.39.x` | Yes |
| Security 5.7 (ltsboot; fork compatible with Spring Security 5.7) | `5.7.14.x` | Yes |

Versions are four numeric parts: the public OSS version of the base, followed by the ltsboot release number (for example `5.3.39.1`).
Earlier ltsboot releases and the upstream commercial releases are not covered by this policy.

## Response process

1. **Acknowledgement and triage.** The maintainers acknowledge the report and confirm or reject its applicability to the
   supported lines.
2. **Embargo.** Accepted issues are kept private until a fix is released. The reporter is asked to keep the details private
   until the advisory is published.
3. **Review.** Every security patch is reviewed by a human maintainer before it is merged.
4. **Release and advisory.** The fix is released as a new ltsboot version, then the advisory is published.

### Response targets

These are targets, not guarantees. "Fix available" means an OSS upstream fix is public, or ltsboot has its own fix.

| Severity | Also covers | Target for the patch release |
|---|---|---|
| CRITICAL | Any CVE listed in the CISA KEV catalogue | 7 days after a public upstream fix; 14 days if the fix is ltsboot's own |
| HIGH | — | 30 days |
| MEDIUM | — | Next scheduled release (about 90 days) |
| LOW | — | Best effort |

Severity follows the official advisory when one exists.

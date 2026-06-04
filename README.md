# Nagoya University (nagoya)

Nagoya University (名古屋大学) is a national research university in Nagoya, Aichi, Japan, ranked #152 in the QS World University Rankings 2025. This repository catalogs the institution's public developer/API footprint as an [APIs.json](https://apisjson.org) profile. The most clearly documented, verified-live machine API is the NAGOYA Repository OAI-PMH interface on the NII WEKO3 / JAIRO Cloud platform; most other systems are gated behind THERS / GakuNin (Shibboleth/SAML) authentication.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/nagoya/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=nagoya-api-evangelist&utm_content=repo

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Access, Institutional Repository, OAI-PMH, Japan

## APIs

- **NAGOYA Repository OAI-PMH** — OAI-PMH 2.0 metadata harvesting for the Nagoya University institutional repository (WEKO3 / JAIRO Cloud). Base URL: `https://nagoya.repo.nii.ac.jp/oai`. Docs / front end: https://nagoya.repo.nii.ac.jp/

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/nagoya-plans-pricing.yml](plans/nagoya-plans-pricing.yml)
- Rate Limits: [rate-limits/nagoya-rate-limits.yml](rate-limits/nagoya-rate-limits.yml)
- FinOps: [finops/nagoya-finops.yml](finops/nagoya-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-06-03

## Common Properties

- Website: https://en.nagoya-u.ac.jp/
- Institutional Repository: https://nagoya.repo.nii.ac.jp/
- IT Services (ICTS): https://icts.nagoya-u.ac.jp/en/
- Authentication (NU-ID): https://icts.nagoya-u.ac.jp/en/services/nuid/
- LinkedIn: https://www.linkedin.com/school/nagoya-university/

## Notes

- The NAGOYA Repository OAI-PMH endpoint was verified live: the `Identify` verb returns valid OAI-PMH 2.0 XML with `repositoryName` "NAGOYA Repository" and `baseURL` `https://nagoya.repo.nii.ac.jp/oai`.
- The underlying WEKO3 platform also exposes search/record paths, but probes returned 400/500/410 and they are not presented as documented developer APIs, so they are not cataloged.
- Student/staff systems (portal, NU-ID, course registration) are gated behind THERS / GakuNin Shibboleth/SAML SSO and are not public developer APIs.
- No official university-wide GitHub organization or public developer portal was found; only individual lab/research-group orgs exist. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com

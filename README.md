# OEMConfig Validator Pro

> Helps Intune admins managing Android Enterprise fleets instantly diagnose why OEMConfig policies aren't applying — without six weeks of trial and error.

## Overview

A SaaS web tool that ingests exported Intune OEMConfig JSON policy files and device diagnostics, then runs automated validation against known schema versions for major OEMs (Zebra, Honeywell, Samsung Knox) to flag misconfigurations, schema version mismatches, and policy layering conflicts. It generates a prioritized remediation report with copy-paste-ready corrected JSON and deployment sequencing recommendations. A companion PowerShell module pulls device OEMConfig managed configuration status directly from the Microsoft Graph API for real-time compliance visibility.

## Problem This Solves

OEMConfig settings silently fail to apply after device restarts or OEM app updates due to schema version drift and policy layering conflicts — a problem Microsoft documentation does not help diagnose, forcing admins into weeks of manual trial-and-error troubleshooting that stalls warehouse or field operations

## Target Audience

IT admins and Intune consultants managing 200+ Android Enterprise COBO devices in logistics, warehousing, healthcare, or retail environments using Zebra, Honeywell, or Samsung hardware

## Tech Stack

PowerShell, Next.js, React, Node.js, Microsoft Graph API, Stripe, Gumroad, PostgreSQL, Docker

## Installation

```powershell
# Clone the repository
git clone https://github.com/oemconfig-validator-pro.git
cd oemconfig-validator-pro

# Review the script before running
Get-Content scripts/oemconfig-validator-pro.ps1

# Run with appropriate permissions
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
.\scripts\{oemconfig-validator-pro}.ps1
```

## Usage



## Monetization Strategy

SaaS subscription at $29/month per tenant (up to 500 devices) and $59/month for enterprise (unlimited devices) sold via Stripe on a self-hosted Next.js app; companion PowerShell module sold separately as a one-time $49 download on Gumroad with a free lite version for top-of-funnel; consulting retainer upsell at $150/hr for OEM schema customization engagements

| Metric | Value |
|--------|-------|
| Revenue Potential | HIGH |
| Estimated Effort  | 1-3months |

## Contributing

1. Fork this repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'feat: add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

MIT License — see [LICENSE](LICENSE) for details.

---

*Generated from the article: [OEMConfig on Android Enterprise: The Complete Intune Guide](https://msendpoint.com/articles/oemconfig-on-android-enterprise-the-complete-intune-guide) on 2026-03-28*
*Blog: [MSEndpoint.com](https://msendpoint.com)*
# Mail-to-GitHub Recon Tool

A simple Bash script for reconnaissance (OSINT). It takes a target domain, finds associated email addresses using third-party APIs (Ful.io and Hunter.io), and then attempts to discover the corresponding GitHub user profiles for those emails.

This tool is intended for penetration testers and bug bounty hunters to quickly map a target's potential developer footprint.

# Features

- Email Enumeration: Gathers emails from a domain using:

> Ful.io

> Hunter.io (requires an API key)

- GitHub Correlation: Searches the GitHub user database for profiles matching the enumerated emails.

- Unique Results: Uses anew to ensure email and user lists are unique.

- Organized Output: Saves results to a dedicated directory (/tmp/<org_name>/).

- Readable Output: Simple, color-coded console logs.

# Usage

- Run the script with the target domain and an organization name (which is used to create the output folder).

> ./findEmail.sh <domain> <org_name>

- Example

> ./findEmail.sh tori.fi tori

# Disclaimer
> This tool is for educational purposes and authorized security testing only. Do not use it on any domain or organization without explicit permission. The author is not responsible for any misuse or damage caused by this script.

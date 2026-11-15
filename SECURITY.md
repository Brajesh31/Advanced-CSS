# 🔐 Security Policy

Advanced CSS is a static learning repository made up of HTML, CSS, and reference PNG images. It currently has no backend, database, authentication, API, or package-based runtime. Security still matters because static pages may be hosted publicly and can include external links, scripts, or contributed assets.

## 📚 Table of Contents

- [Supported Scope](#-supported-scope)
- [Reporting a Vulnerability](#-reporting-a-vulnerability)
- [Safe Testing](#-safe-testing)
- [Content and Script Safety](#-content-and-script-safety)
- [Third-Party Assets](#-third-party-assets)
- [Static Hosting](#-static-hosting)
- [Dependency and Workflow Safety](#-dependency-and-workflow-safety)
- [Maintainer Response](#-maintainer-response)
- [Security Checklist](#-security-checklist)

## 🎯 Supported Scope

This policy covers:
- HTML documents in the assignment directory.
- Embedded CSS and any future JavaScript.
- Reference images and contributed assets.
- Documentation and repository configuration.
- GitHub Actions workflows.
- Static deployment configuration.

Third-party hosting providers and browsers have their own security policies.

## 📣 Reporting a Vulnerability

Do not publish exploitable details in a public issue before a maintainer has had a reasonable chance to review the report.

Use GitHub's private vulnerability reporting feature for this repository when available. Otherwise, contact the repository owner privately through an appropriate GitHub channel. Do not include passwords, tokens, or sensitive personal information in a public report.

A useful report includes:
- Affected file or page.
- Browser and environment.
- Reproduction steps.
- Expected and actual behaviour.
- Potential impact.
- A minimal proof of concept that does not harm users.

## 🧪 Safe Testing

Test only on your own local copy or an environment where you have permission. Do not use the repository to probe unrelated services, hosts, or user accounts.

## 🧱 Content and Script Safety

- Avoid inline scripts unless the exercise specifically teaches JavaScript.
- Never embed API keys, passwords, tokens, or private credentials in HTML or CSS.
- Treat copied snippets and remote assets as untrusted until reviewed.
- Avoid unsafe HTML injection patterns in any future interactive example.
- Do not add hidden tracking or unexpected data collection.
- Avoid redirects or popups that mislead visitors.

Static pages can still execute JavaScript and load remote resources. "No backend" does not automatically mean "no risk".

## 🧩 Third-Party Assets

Before adding a font, image, script, stylesheet, or icon:
- Confirm that its licence permits the intended use.
- Record attribution or licence requirements where applicable.
- Prefer pinned and reputable sources if remote loading is necessary.
- Explain why the external asset is required.
- Consider local files when appropriate.
- Do not hotlink private or unlicensed material.

## 🌐 Static Hosting

Use HTTPS. Review host settings for directory listing, headers, caching, and unwanted redirects. Do not deploy private files, source maps containing secrets, credentials, or machine-specific configuration.

## ⚙️ Dependency and Workflow Safety

The current exercises need no npm dependencies. If a future change adds a toolchain:
- Explain the need.
- Commit the lockfile.
- Review dependency advisories.
- Avoid committing installed dependency folders.
- Use minimal GitHub Actions permissions.
- Pin third-party actions to trusted versions or immutable SHAs according to project policy.

## 🛠️ Maintainer Response

Maintainers should acknowledge reports, reproduce the issue, assess scope, prepare a fix, and communicate resolution responsibly. Response time is best effort and no SLA is promised.

## ✅ Security Checklist

- [ ] No secrets are committed.
- [ ] No unreviewed remote script is introduced.
- [ ] Third-party assets have permitted use.
- [ ] No unexpected tracking is added.
- [ ] Static hosting uses HTTPS.
- [ ] Workflow permissions are minimal.
- [ ] Security-related documentation remains accurate.

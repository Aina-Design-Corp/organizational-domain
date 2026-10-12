# Āina Design Corp

Āina Design Corp is a Hawaiʻi nonprofit corporation and an IRS 501(c)(3)
public charity. On GitHub it is the organization `Aina-Design-Corp`: the owner
of the people, teams, and repositories published under that name. This page
states how the organization is governed on GitHub and the enterprise pattern
it is built for. Nothing here claims adoption, endorsement, or deployment by
any government agency.

## Organization and enterprise posture

*Stated as of 2026-10-11.*

GitHub has three layers, and one rule about ownership runs through them:

```
Enterprise account   (the pattern)       rules that bind every organization under it — established when a program needs it
└── Organization     Aina-Design-Corp    the people, teams, and repositories of one owner — live today
    └── Repository   one per project     the record, the checks that run on every change, the public pages
```

- **The organization** is the unit an owner can hand over. It can be removed
  from one enterprise and invited into another with its repositories, history,
  and public pages intact.
- **The enterprise account** is the administrative layer above organizations:
  policies every organization must follow, billing, a 180-day audit log that
  can be streamed to storage the adopting program controls, and GitHub's own
  compliance reports.
- **The rule:** a program that adopts this pattern gets its own organization
  inside the enterprise. Its staff never become members of Āina Design Corp's
  repositories. They sign in with their own directory, work in their own
  organization, and can take that organization with them at any time.

### What exists today

- Two-factor sign-in is required for every member; default member access is
  read, and write access is granted deliberately, by team.
- Public repositories carry branch protection with a required validation
  check, a `CODEOWNERS` file naming who reviews what, and public pages built
  by workflow behind a repository variable and a deployment environment. A
  person publishes, never an automated process.

### The enterprise, when a program needs it

- **Licensing.** Āina Design Corp is registered with GitHub for Nonprofits.
- **Kind of enterprise.** An enterprise with personal accounts: the kind that
  can invite this existing organization and lets each organization bind its
  own identity provider. The other kind, Enterprise Managed Users, cannot add
  an existing organization, and its accounts cannot create public content, so
  public transparency pages could not be built in it.
- **Āina Design Corp remains an organization** inside the enterprise. An
  adopting program's organization sits beside it, transferable intact.
- **Identity is configured per organization, never for the whole
  enterprise.** That is a rule of the pattern: enterprise-level single sign-on
  overrides every organization's own and disables organization provisioning.
  With single sign-on left off at the enterprise, a program's directory (for
  example Microsoft Entra ID) governs membership of its organization through
  SAML single sign-on, SCIM provisioning, and team synchronization: who is a
  member, on which team, and when they leave.
- **What the enterprise adds** on top of the organization controls above:
  policies enforced across every organization, the enterprise audit log and
  its streaming, and the compliance reports that can accompany a program's
  architecture documentation.

The working demonstration of this pattern, with the full provisioning
walkthrough and a table of which controls it carries today, is
[kuleana-portal](https://github.com/Aina-Design-Corp/kuleana-portal) and its
[docs/ENTERPRISE.md](https://github.com/Aina-Design-Corp/kuleana-portal/blob/main/docs/ENTERPRISE.md).
Platform facts are GitHub's, from GitHub Docs (Enterprise Cloud); Āina Design
Corp makes no certification claims of its own here. The enterprise is
described as a pattern; its name and address are stated when they exist.

## Identifiers

- EIN: 32-0466202
- UEI: ML2PYA3W9BJ3
- CAGE Code: 7WCD4
- Legal Entity GLN: 0860004112402

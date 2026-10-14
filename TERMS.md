# Terms of Service — Hermes bot fleet

**Last updated:** 13 October 2026
**Operator:** Prakash Sewani ("the operator", "we")
**Contact:** adamjones2227@gmail.com

## 1. What these bots are

This repository holds the legal documents for the following Discord bots (together, "the bots"), each
operated by the operator inside Discord servers the operator controls or is a member of:

| Bot | Discord application | Role |
|---|---|---|
| 🤖 **Hermes** | Hermes Bot | general-purpose assistant: answers, searches, runs automations |
| 🛠️ **forge** | hermes_forge | builds approved work items on the operator's own machines (git branches, commits, pull requests) |
| 🔍 **sentry** | hermes_sentry | reviews pull-request diffs read-only and posts a verdict |
| 🧪 **canary** | hermes_canary | verifies merged changes by running the project's own checks and reporting results |

The bots are private automation agents. They are not a public service, are not offered for sale, and
are not marketed to third parties.

## 2. Acceptance

By adding a bot to a server, or by interacting with a bot in a server where it is present, you agree
to these terms. If you do not agree, do not add the bot and do not interact with it; server
administrators can remove a bot at any time.

## 3. Permitted use

You agree not to use the bots to:

- violate Discord's Terms of Service, Community Guidelines, or any applicable law;
- harass, deceive, or harm anyone, or to generate content that does so;
- attempt to extract credentials, tokens, private keys, or other secrets;
- gain unauthorised access to any system, account, or data;
- abuse, overload, or reverse-engineer the bots or the infrastructure they run on.

The bots may refuse any request, at any time, without explanation.

## 4. Actions the bots take

Some bots perform actions with real effects, and they act only on the operator's own infrastructure:

- **forge** creates git branches, commits, and pull requests, and may push branches to repositories the
  operator controls. It never merges, and it never pushes to a public remote without the operator's
  explicit permission for that specific action.
- **sentry** is read-only: it reads diffs and repository files and posts comments. It does not modify,
  commit, push, or merge anything.
- **canary** runs a project's test and build commands on the operator's own machine after a merge, and
  reports the results. It does not modify code.
- **Hermes** may run shell commands, read and write files, browse the web, and schedule recurring jobs
  on the operator's own infrastructure, on the operator's instruction.

No bot performs these actions on behalf of, or against, any third party's system.

## 5. No warranty

The bots are provided "as is" and "as available", without warranty of any kind, express or implied,
including merchantability, fitness for a particular purpose, and non-infringement. Output may be
incorrect, incomplete, or misleading — including confidently wrong statements about code, systems, or
facts. **Verify anything important before relying on it.** Automated actions, in particular, should be
reviewed by a human before being merged, deployed, or trusted.

## 6. Limitation of liability

To the maximum extent permitted by law, the operator is not liable for any indirect, incidental,
special, consequential, or punitive damages, or for any loss of data, profits, revenue, or goodwill,
arising from the use of or inability to use the bots — even if advised of the possibility.

## 7. Availability and changes

The bots may be changed, suspended, or discontinued at any time, with no notice and no obligation.
These terms may be updated; the "Last updated" date above will change, and continued use after an
update constitutes acceptance.

## 8. Termination

The operator may block any user or remove a bot from any server at any time. You may stop using a bot
at any time by not interacting with it and asking a server administrator to remove it.

## 9. Governing law

These terms are governed by the laws of India, with the courts of Thane, Maharashtra having
jurisdiction.

## 10. Contact

Questions about these terms: **adamjones2227@gmail.com**

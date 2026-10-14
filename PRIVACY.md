# Privacy Policy — Hermes bot fleet

**Last updated:** 13 October 2026
**Operator:** Prakash Sewani ("the operator", "we")
**Contact:** adamjones2227@gmail.com

This policy covers the Discord bots **Hermes** (Hermes Bot), **forge** (`hermes_forge`),
**sentry** (`hermes_sentry`) and **canary** (`hermes_canary`).

## 1. Short version

The bots read the Discord messages they are asked to act on and store what they need to do their job on
the operator's own server. Nothing is sold, nothing is used for advertising, and nothing is shared with
anyone except the model provider that generates the responses, as described below.

## 2. What is collected

- **Discord content:** messages, attachments, embeds, usernames, user IDs, channel and server IDs that
  the bot can see — in the channels where it is present, or in direct messages to it. Bots only see
  messages they are mentioned in or that arrive in channels they are configured to read.
- **Conversation state:** the session transcript (your prompts, the bot's replies, the tool calls it
  made and their results) so the conversation can continue across messages.
- **Operational logs:** timestamps, errors, job runs, and delivery status, for debugging and audit.
- **Repository and system data** (only where a bot's role requires it): git branch and commit metadata,
  pull-request diffs and comments, and command output from the operator's own machines.

The bots do **not** collect payment data, and they do not request or store passwords, bot tokens, API
keys, one-time codes, or other credentials.

## 3. Where it is stored

On infrastructure the operator controls: a private server running the agent framework, its SQLite
session database (`state.db`), log files, and the Discord channel history where the bots post. Session
transcripts are retained in that database and pruned on the framework's normal retention schedule.
Logs are kept for as long as they are useful for debugging, and are rotated.

Data is not stored in a public location. Nothing described here is published to a third-party analytics,
marketing, or advertising service.

## 4. Third parties

- **Discord** processes the messages that pass through it under
  [Discord's own Privacy Policy](https://discord.com/privacy).
- **Model providers.** To produce a reply, the relevant conversation content (your message, the
  retrieved context, and the tool results needed to answer) is sent to the large-language-model
  provider configured for that bot, so it can generate the response. That provider processes the
  content under its own terms and privacy policy. Which provider is in use can change without notice as
  the operator changes configuration.
- **GitHub** — only for the repository-related bots (forge, sentry, canary), which read repository and
  pull-request data through the GitHub API where that is required for their role.

No data is sold, rented, or shared with advertisers, data brokers, or any other third party.

## 5. Why it is processed

To run the assistant, keep conversation context, perform the specific job a bot was asked to do (write
code, review a diff, run tests), debug failures, and prevent abuse.

## 6. Retention and deletion

Session transcripts and logs are kept only as long as they serve the purposes above, then deleted or
rotated out. You can ask for content you posted to be deleted by contacting the operator at the address
above; where the content sits in Discord itself, delete it there or ask a server administrator.
Server administrators can remove a bot at any time, which stops further collection in that server.

## 7. Security

Access to the operator's infrastructure is restricted to the operator over SSH key authentication, and
secrets are stored in files readable only by the operator's account. No system is perfectly secure, and
the operator cannot guarantee absolute security.

## 8. Children

The bots are intended for users who are at least 13 years old, in line with Discord's own minimum age.
They are not directed at children and no data is knowingly collected from children below that age.

## 9. Your rights

Depending on where you live, you may have rights to access, correct, or delete personal data, or to
object to its processing. To exercise any of them, contact **adamjones2227@gmail.com**. Because the
bots run in the operator's own servers for a small private audience, most requests can be handled
directly by deleting the relevant messages or sessions.

## 10. Changes

This policy may be updated; the "Last updated" date above will change when it is. Material changes will
be announced in the Discord server where the bots run.

## 11. Contact

**adamjones2227@gmail.com**

# Plainmail for Claude

Real mailboxes on your own domains, set up and handled from Claude. Ask "set up hello@mynewapp.com" and Claude adds the domain to Plainmail, writes the MX, SPF, DKIM and DMARC records at your DNS host (Cloudflare, Vercel or Porkbun, or gives you the records to copy anywhere else), waits until they're live and creates the mailbox. After that it can read, send and reply to mail on that address. The mailbox is a normal IMAP account, so it also works in Apple Mail, the Gmail app, Outlook or Thunderbird.

## What's inside

- The Plainmail remote MCP server (`https://app.plainmail.dev/api/mcp/mcp`), signed in with OAuth. No API key to copy.
- A `set-up-email` skill with the setup steps.

## Install

```
/plugin marketplace add jdcodes1/plainmail-claude-plugin
/plugin install plainmail@plainmail
```

Then run `/mcp`, pick plainmail and sign in. You choose which permissions to allow: read mail, send and organize mail, and manage domains and mailboxes.

You need a [Plainmail account](https://app.plainmail.dev/signup) ($5 a month for up to 50 domains).

## Links

- Docs: https://plainmail.dev/docs
- Privacy: https://plainmail.dev/privacy
- Support: support@plainmail.dev

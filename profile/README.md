<div align="center">

# SMTPfast

**The email API for developers and AI agents.** Send, receive and manage email through one Resend-compatible API, with templates, inboxes, broadcasts and webhooks built in.

[Website](https://smtpfa.st) · [Docs](https://smtpfa.st/docs) · [Dashboard](https://smtpfa.st/dashboard) · [Changelog](https://smtpfa.st/changelog) · [Status](https://smtpfa.st/status)

</div>

---

## Send your first email

```bash
curl -X POST https://smtpfa.st/api/v1/emails \
  -H "Authorization: Bearer $SMTPFAST_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "from": "hello@yourapp.com",
    "to": ["user@example.com"],
    "subject": "Welcome!",
    "html": "<h1>Hello!</h1>"
  }'
```

Or from a terminal with the CLI:

```bash
npx smtpfast login
npx smtpfast send --from hello@yourapp.com --to user@example.com --subject "Welcome!" --text "Hello!"
```

Create an API key and verify your sending domain in the [dashboard](https://smtpfa.st/dashboard). Already on Resend? Point your code at `https://smtpfa.st/api/v1` and swap the key. See the [migration guide](https://smtpfa.st/docs/resend).

## Open source

- [**smtpfast-cli**](https://github.com/smtpfast/smtpfast-cli): every API endpoint as a command, generated from the OpenAPI spec and released automatically when the API changes. `npm install -g smtpfast`, or a single binary for macOS, Linux and Windows.
- [**terraform-provider-smtpfast**](https://github.com/smtpfast/terraform-provider-smtpfast): manage sending domains, API keys and webhooks as code. On the [Terraform Registry](https://registry.terraform.io/providers/smtpfast/smtpfast/latest).
- [**smtpfast-skill**](https://github.com/smtpfast/smtpfast-skill): an Agent Skill that teaches Claude and other agents to use the SMTPfast API.
- [**feedletter**](https://github.com/smtpfast/feedletter): turn an RSS feed or a folder of Markdown into a newsletter, curated in a browser studio and sent with SMTPfast.

## What you get

- **Resend-compatible API** for emails, templates, inboxes, contacts, segments and webhooks, so Resend SDKs and existing code keep working. The full [OpenAPI spec](https://smtpfa.st/api/v1/openapi.json) is public.
- **Hosted templates** with variables, a live desktop, mobile and dark-mode preview, and ten starters.
- **Inboxes on your own domain**: received mail in threads, with labels, folders, and drafts that a person approves before an agent's reply goes out.
- **Built for agents**: a hosted [MCP server](https://smtpfa.st/docs/mcp) with OAuth covers almost the whole API. Agents never get to create API keys or change team members.
- **Deliverability built in**: DKIM, SPF and DMARC setup, one-click DNS on Cloudflare, suppressions, and live delivery logs.
- **Teams** with roles, and broadcasts, signup forms and transactional email in one place.

<div align="center">
<sub>Built for developers who just want email to work.</sub>
</div>

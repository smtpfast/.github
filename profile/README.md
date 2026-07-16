<div align="center">

# SMTPfast

**Transactional email for developers.** A fast, simple API to send email and manage sending domains, contacts, broadcasts, and webhooks.

[Website](https://smtpfa.st) · [Docs](https://smtpfa.st/docs) · [Dashboard](https://smtpfa.st)

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

Create an API key and verify your sending domain in the [dashboard](https://smtpfa.st).

## Open source

We build in the open. A few things you can use today:

- [**terraform-provider-smtpfast**](https://github.com/smtpfast/terraform-provider-smtpfast): manage sending domains, API keys, and webhooks as code. Register a domain and publish its DNS records in a single `terraform apply`.
- [**smtpfast-skill**](https://github.com/smtpfast/smtpfast-skill): an Agent Skill that teaches Claude and other agents how to use the SMTPfast API.

## Why SMTPfast

- **Simple, modern API** with SDKs, an [OpenAPI spec](https://smtpfa.st), and an MCP server, so it works as well with agents as with your code.
- **Deliverability built in**: DKIM, SPF, DMARC, and one-click Cloudflare DNS setup for your sending domains.
- **The essentials, done well**: transactional sends, batches, contacts, broadcasts, suppressions, and webhooks.

## Links

- Website and docs: [smtpfa.st](https://smtpfa.st)
- Status and updates: on the [website](https://smtpfa.st)

<div align="center">
<sub>Built for developers who just want email to work.</sub>
</div>

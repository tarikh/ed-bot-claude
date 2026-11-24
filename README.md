# Ed Bot

![Ed.](assets/ed-bot.png)

Executive self-coaching

Think through the leadership challenges that don’t have easy answers.

Grounded in Ed Batista’s published writing, Ed Bot helps founders, leaders and coaches explore co-founder tension, difficult feedback, burnout, self-doubt and the demands of management. It offers thoughtful explanations, practical experiments and questions that help you examine your own situation.

Explore a challenge in depth, continue the conversation, or find the original essays—with source links and contributor credits.

Ed Bot provides AI-powered self-coaching. Ed Batista is not personally responding. Its published-writing collection may omit newer essays.

## Recorded demo

[Watch the Claude coaching demo](https://getsuperculture.com/edbot/demo/ed-bot-claude-semantic-demo-2026-11-24.mp4). Duration: 50 seconds.

The recording shows the actual private development installation: a delegation question, its response with a published source link, and a contextual follow-up asking for wording for a direct report. Waiting time was shortened and is labeled in the video. Response content was not changed. This is a usage demonstration, not a complete evaluation or proof of the retrieval route for every answer.

## Connection and use

The archive MCP points to the existing public HTTPS semantic service. It requires
no sign-in, access token or user API key. Enable the Ed Bot coaching skill, then
ask a leadership question or request a published essay. Both tools are read-only.
The package cannot read private notes, edit sources or import arbitrary URLs.

Try: “I keep taking delegated work back. Help me understand the pattern.”
Or: “Summarize Leading with Inquiry (How to Have a Better Dialogue).”

## Data handling and availability

Short deidentified topic queries go through the service to OpenAI-hosted retrieval.
Do not send names, personal details or whole conversations in tool queries.
The application stores aggregate usage counters, not query/conversation histories.
Host chat products and infrastructure process requests under their own policies.
The shared service permits 30 external semantic searches per minute, 500 per UTC
day and 5,000 per UTC month across all users. If search is unavailable, the host
should disclose that limit, avoid invented retrieval claims and distinguish any
available bundled-source response from a successful semantic search.

API keys stay in server runtime secrets and are absent from this package.
No purchase or payment flow is included. Host plan requirements may apply.

## Usage analytics

The shared source service records limited operational events in PostHog: tool
name, retrieval mode, timing, result count and a fixed outcome/error category.
It sends no coaching questions, answers, essay content or IDs, names, emails,
client IP addresses, cookies or conversation IDs to PostHog. It uses no browser
autocapture or session replay.

Where a host supplies a stable identifier, the service transforms it to a
service-specific code for unique/returning-user measurement. The current
no-sign-in Claude connection has no usable stable user identifier: its source
calls count as activity, not unique or returning people. ChatGPT host identifiers
were observed to deduplicate repeat calls. The platforms are not merged, and
conversations that use only bundled sources are invisible to the service.

After directory publication, Anthropic documents a separate connector dashboard
metric for distinct Claude accounts that used a tool in the last 30 days. This
is an aggregate platform count, not a user identifier delivered to PostHog or
a documented returning-user report. OAuth could support individual account
measurement, but this candidate does not add sign-in.

See the [privacy notice](https://getsuperculture.com/edbot/privacy/) for provider
processing, analytics retention and support arrangements. Person-profile
creation and geographic enrichment are disabled, and the PostHog project
discards client IP data. This service does not retain a name/email-to-code map.

## Support and policies

- Publisher: Tarikh Korula; edbot@getsuperculture.com
- Product: https://getsuperculture.com/edbot/
- Support: https://getsuperculture.com/edbot/support/
- Current product privacy: https://getsuperculture.com/edbot/privacy/
- Current product terms: https://getsuperculture.com/edbot/terms/
- Retrieval-service privacy: https://edbot-public-retrieval-2026-11-23.tarikhkorula.chatgpt.site/privacy
- Retrieval-service terms: https://edbot-public-retrieval-2026-11-23.tarikhkorula.chatgpt.site/terms

## Release status

Local submission candidate only, not a submitted, approved or published plugin
release. The main privacy and terms pages were updated November 24, 2026 for
both ChatGPT and Claude and the hosted semantic retrieval service. The matching
published policy text is bundled in docs/. The recorded usage demo is hosted
and publicly accessible. Remaining platform setup, required validation and the
authorized developer's attestations must be completed before submission.

See LICENSE and NOTICE.md for CC BY-SA 4.0 instruction/source rights and the
branding exclusion. No cancellation or resubmission of the existing OpenAI
4.0.0 review, original-GPT change, migration or redirect change was performed.

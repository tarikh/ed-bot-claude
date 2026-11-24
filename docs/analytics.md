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

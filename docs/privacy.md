# Ed Bot privacy notice

Updated November 24, 2026.

This notice covers Ed Bot, published by Tarikh Korula, its read-only source
service, and support emails you choose to send. Ed Bot combines coaching
instructions and published writing to help you reflect on leadership and working
relationships. Some editions use direct archive searches; semantic editions add
OpenAI-hosted retrieval. Browsing getsuperculture.com is separately covered by
the [Superculture website privacy policy](https://getsuperculture.com/privacy.html).

## Your conversation and the host product

ChatGPT or Claude processes your conversation and writes the answer. Ed Batista
is not personally responding. The host may use conversation context when choosing
tools and their arguments. Its handling of conversations, retention, model
improvement and privacy controls depends on its own policies and your account
or workspace settings. Using Ed Bot does not create a confidential coaching
relationship with Ed or Tarikh.

See [OpenAI's privacy policy](https://openai.com/policies/privacy-policy/),
[ChatGPT data controls](https://help.openai.com/en/articles/7730893-data-controls-in-chatgpt)
and [Anthropic's privacy policy](https://www.anthropic.com/legal/privacy).

## Source tool requests and semantic retrieval

When the host calls a source tool, it sends arguments such as a short search
query or a numeric essay ID to the Ed Bot service hosted on ChatGPT Sites. The
service returns published source text and metadata. It does not collect a full
conversation history for its publisher as a product feature.

The host is instructed to use short, deidentified descriptions of the leadership
topic, without names, private company details or full conversations. This is an
instruction to the host, not a guarantee that every generated query will exclude
personal information. Avoid including sensitive details that are unnecessary
to the topic you want to explore.

For a semantic search, the service sends the query to OpenAI's hosted Retrieval
API to locate relevant passages in an indexed snapshot of Ed Batista's published
essays. Exact-title and newest-essay lookups and complete essay reads use the
fixed archive directly. The service returns source material; it does not call
a separate model to write another coaching answer.

The indexed collection contains published essay text, titles, original URLs,
dates and source identifiers. It does not contain private coaching notes or
client records. The published-source snapshot remains available until the
archive is updated or removed; older downloaded packages can retain older copies.

## Storage, infrastructure and retention

The Ed Bot application does not persist tool queries or conversation histories.
The public semantic service uses PostHog (US Cloud) for limited usage analytics:
tool name, retrieval mode, timestamp, duration, result count, success or a fixed
error category, client family when available, and whether a stable host identifier
was available. It does not send search queries, coaching messages, answers,
source text, essay IDs or titles, error messages, names or email addresses to
PostHog. It does not use session replay or browser autocapture.

When the host supplies a stable user identifier, the service converts it to a
service-specific code using a private cryptographic key before sending it to
PostHog. This allows counts of unique and returning host users without sending
the original identifier. User counts cover only calls with a stable identifier;
other requests count as activity only. Identifiers from different platforms or
identity sources are not merged, and counts do not represent verified people or
all conversations. PostHog person-profile creation and geographic enrichment are
disabled; the project discards client IP data. The service does not forward
client IP addresses, cookies, conversation IDs or raw request headers to PostHog.

PostHog processes these limited analytics events under its
[privacy policy](https://posthog.com/privacy). Analytics retention follows the
PostHog project's configured retention and applicable provider policies. We do
not promise a separate automatic deletion period for analytics events. Contact
the support address with analytics privacy questions; we do not retain a mapping
from these codes to your name or email.

The application also stores aggregate usage counters to limit external semantic
searches to 30 per minute, 500 per UTC day and 5,000 per UTC month across all
users. These quota counters do not identify users or store their queries. API
credentials remain in server runtime settings and are not distributed in plugin
packages. The separate earlier archive service has not been instrumented with
PostHog.

Tool requests still reach the service and its infrastructure. OpenAI, Sites and
the host product process requests and may maintain request metadata, abuse-
monitoring records and operational logs under their own policies. This notice
does not promise anonymous requests, zero infrastructure logging or a particular
retention period for those providers. See [OpenAI's API data controls](https://developers.openai.com/api/docs/guides/your-data)
for hosted retrieval processing and the host's applicable privacy controls for
conversations.

## Support information you send directly

If you email [edbot@getsuperculture.com](mailto:edbot@getsuperculture.com), Tarikh
receives your email address, any name you include, and the message and attachments
you choose to send. You do not need to send a full conversation to get help.

Support information is used to respond to your request, troubleshoot the issue
and handle related privacy or deletion requests. Access to the support inbox is
limited to Tarikh and the email-service provider needed to deliver and store
those messages. Support messages are not used for marketing or advertising.

Support emails under Tarikh's control are deleted within 90 days after the issue
is resolved. You may request earlier deletion by emailing the support address.
The email provider manages its infrastructure and backup retention under its
own policies. This support-email policy does not set OpenAI's or Anthropic's
retention periods.

## Your choices and contact

You can use Ed Bot without emailing its publisher. Send only the support details
you want Tarikh to receive. For questions about, access to or deletion of support
information, contact [edbot@getsuperculture.com](mailto:edbot@getsuperculture.com).
Use your host's controls or support for host-account and conversation requests.
The application does not retain search histories that the publisher can retrieve
or delete on your behalf. This does not limit requests you may make to providers
that retain their own records.

If Ed Bot's data practices change, this notice will be updated.

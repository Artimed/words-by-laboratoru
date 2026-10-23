# Privacy and local data

Words by LaboratorU — private preview, updated 2026-10-23.

## What Words stores

Learning state, exposure counts and timestamps, selected native language, downloaded
English blocks and translations live under `~/.claude/english-ladder/`. The same
state is shared by the widget and connected chat apps. Window size, theme, pinning,
translation visibility and the acknowledged pin hint use macOS preferences in the
`local.artimed.words` domain.

Per-session scheduling files contain a hashed session key, request counter, current
turn identifier and offered word IDs. The local word log records time, source app,
model metadata when supplied, offered words and matched words. It does not store
message text. Installation ownership records and configuration backups are also
local; backups can contain unrelated settings already present in chat configuration
files and should not be posted publicly.

## Chat access and model providers

The optional adapters inject English word suggestions and native-language meanings
into normal assistant context. The selected assistant's provider processes that
context under its own service terms and privacy practices. Words does not operate
its own model service or send transcripts to a LaboratorU server.

For matching, Codex supplies assistant text in its hook event. Claude Code can supply
a transcript path: the current implementation reads that local file into memory and
examines up to its last 400 records for the current reply. Code and tool results are
excluded from word matching. Transcript text is not copied into Words' word log.
The original chats remain managed by the chat applications.

## Network requests and speech

GitHub serves public data-only dictionary archives over HTTPS. Build 0.2.0 (11)
downloads them without GitHub sign-in, CLI or tokens; only the selected missing
translation and required English cores are fetched. Earlier private developer builds
may use an authenticated GitHub CLI fallback. No developer token is bundled.
Download hosts receive ordinary connection/request metadata. Dictionary packs
contain data, not code.

New updater-enabled builds use Sparkle to request a public GitHub update feed and
download signed application updates when requested. Automatic checks are enabled by default and may be disabled in About;
system profiling is disabled. GitHub receives normal request metadata. Public build
11 does not yet include this updater.

The app does not include its own analytics or advertising SDK. Clicking website or
project links opens those sites, which have their own privacy practices. English
speech uses macOS system voices; voice availability and downloads are managed by
macOS. No separate Words audio account or audio-file upload is implemented.

## Removal

Full removal previews the owned files and edits, then requires confirmation. It
removes Words connections while preserving unrelated settings and original chats.
Files and settings backups are moved into a dated Words folder in Trash. They remain
recoverable until the user empties Trash; this is not secure erasure. Configuration
backups created by Words are removed only when ownership and integrity are verified.
Unknown or changed files stop removal for review. Restart old chat sessions so
instructions already in their context are no longer reused.

This describes the current implementation, not a guarantee about third-party
services. Do not include transcripts, personal progress, credentials, configuration
backups or payment information in public bug reports.

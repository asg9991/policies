# Privacy Policy — google-agent

Last updated: 2026-10-22

## What this application is

`google-agent` is a private, locally executed command-line tool used by its
owner to read and organize their own Google Drive, Google Calendar and Gmail
content. It is not a public service, has no end users other than its owner, and
runs entirely on the owner's personal computer.

## What data it accesses

When authorized, the application uses Google OAuth 2.0 to access:

- **Google Drive** — files and folders inside the owner's Drive, to read, create,
  update and trash them.
- **Google Calendar** — calendar events, to list and create reminders.
- **Gmail (read-only)** — message metadata and bodies, to search for
  information the owner requests.
- **Google Docs** — documents, to read and rewrite their content.

## Where the data goes

Nowhere. The application sends no data to any third party. It has no backend
server, no analytics, no telemetry and no advertising. All data stays between
the owner's computer and Google's APIs.

## How credentials are stored

The OAuth refresh token and access token are stored locally on the owner's
computer at `~/.config/google-agent/token.json`, with file permissions `0600`
(readable only by the owner). The OAuth client secret is stored alongside it and
is never committed to version control.

## Data retention and deletion

No copy of Google data is retained beyond what the owner explicitly saves as
local files. The owner can revoke the application's access at any time at
<https://myaccount.google.com/permissions>, which invalidates the stored token,
and can delete the local token file and any exported files directly.

## Contact

Questions about this policy: asg.telecosoluciones@gmail.com

# Wirecat

**A native, local-first API client.** Fast to start, light on memory, works fully offline.
No account, no cloud, no telemetry. Your collections are plain files you can keep in git.

Windows · Linux (coming soon)

> Free for personal use. A license is needed for work and commercial use, see [Licensing](#licensing).

## Why Wirecat

Most API clients today are web apps in a desktop wrapper. Many of them also want you to sign in and sync your
collections to their cloud. Wirecat takes the other road:

- **Native.** Written in C++ with Qt, not Electron. It starts in a moment, uses a fraction of the memory and stays
  responsive on large responses.
- **Offline and private.** Nothing leaves your machine unless you send it. There is no sign-in, no sync and no
  "phone home", and the license check works offline too. It is fine for closed networks.
- **Git-friendly.** One request is one readable JSON file in a folder. Diffs make sense, and teams share collections
  through their own repository. Wirecat picks up changes from `git pull` on the fly.
- **Portable.** Unpack the folder and run it, no installer needed.
- **Easy to switch to.** Import Postman collections and environments (v2.0/v2.1), OpenAPI 3 and Swagger 2
  (JSON or YAML) and cURL commands. Export environments back to Postman and copy any request as cURL.

## Features

**Protocols:** HTTP/HTTPS · WebSocket · Socket.IO (v2, v3, v4) · Server-Sent Events · GraphQL with schema-aware
completion and subscriptions (graphql-ws)

**Requests:** query parameters synced with the URL · headers · raw, JSON, form, multipart and binary bodies ·
proxy · cookies, with a cookie manager

**Auth:** Basic · Bearer · API key · Digest · NTLM · AWS Signature V4 · OAuth 2.0 (Authorization Code with PKCE,
Client Credentials, Password, Device Code, OIDC discovery) with token refresh · inheritance from folders and
collections

**Responses:** pretty JSON that keeps key order · search · JSONPath filter · streaming view · JWT decoder

**Workflow:** environments and `{{variables}}` with inline hints · secrets kept out of the repository · history ·
tabs that survive restarts · quick open (Ctrl+P) · dark and light themes

## Download

Get the latest build from [Releases](../../releases): `Wirecat-<version>-windows-x64.zip`. Unpack it anywhere
and run `wirecat.exe`. There is no installer and nothing else to install.

A Linux build is coming soon.

## Licensing

| Use | Price |
|---|---|
| Personal projects, learning, teaching, open-source projects | **Free**, all features, no time limit |
| At work, in a company, for commercial projects | **Paid license**, one per user |

- Nothing is locked in the free version. Unregistered copies show a small, rare note in the status bar, nothing more.
- A license is perpetual and includes updates.
- To buy a license, [open a license request](../../issues/new?template=license-request.yml). Say how many users and
  how to reach you privately: the key is sent privately, never posted in the issue.
- Enter your key in **Help → License**.

Full terms: [EULA.txt](EULA.txt). Wirecat uses Qt under the LGPLv3, see
[THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt).

## Feedback

Bugs and feature requests: [Issues](../../issues).

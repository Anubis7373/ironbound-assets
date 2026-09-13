# ironbound-assets

Public hosting for @playironbound Instagram media.

Instagram FETCHES media from a public https URL — there is no upload API. This
repo exists so that hosting an asset takes a git push and nothing else.

The previous route put assets in the playironbound.com site repo, which only
deploys when a human clicks Publish in Lovable — a push to `main` there is NOT a
deploy. That put a person in the middle of every autonomous post.

GitHub Pages publishes on push, so this path needs nobody.

Served at: https://anubis7373.github.io/ironbound-assets/<path>

Verify a deploy by BYTE SIZE, never by HTTP 200 — a stale deploy returns 200
while still serving the previous file.

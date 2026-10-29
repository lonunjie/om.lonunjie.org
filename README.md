# om.lonunjie.org

The site and web app for [OM](https://om.lonunjie.org) (Oh Messenger), an open-source, end-to-end-encrypted messenger from
[SeedLife](https://lonunjie.org). OM is in open beta. The source of the app is in [lonunjie/om](https://github.com/lonunjie/om).

- `public/` is the signed OM web release, served as-is by Cloudflare Pages. Do not edit files in it: the service worker rejects any byte that differs from the signed manifest.
- `release/` is the same signed release plus a `wrangler.toml`, used by the button below.

## Run your own copy

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/lonunjie/om.lonunjie.org/tree/main/release)

One click makes your own copy of OM on your own Cloudflare account. Before you use any release folder, check it:
`node verify.mjs --require-signed` (steps in [`deploy/README.md`](https://github.com/lonunjie/om/blob/main/deploy/README.md)).
A copy shows a small link back to the official site so it is not mistaken for it.

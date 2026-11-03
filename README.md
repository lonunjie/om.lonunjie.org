# om.lonunjie.org

The site and web app for [OM](https://om.lonunjie.org) (Oh Messenger), an open-source, end-to-end-encrypted messenger from
[SeedLife](https://lonunjie.org). OM is in open beta. The source of the app is in [lonunjie/om](https://github.com/lonunjie/om).

- `public/` is the signed OM web release, served as-is by Cloudflare Pages. Do not edit files in it: the service worker rejects any byte that differs from the signed manifest.

## Your own delivery service

OM does not run a delivery service for you: nobody starts on SeedLife's. The app's setup helps you create your own, free, on your own
Cloudflare account, from the signed relay template [lonunjie/om-relay](https://github.com/lonunjie/om-relay). The one-click button and the copy of the
web app that used to live here (`release/`) are gone (ADR-0186). To host your own copy of the web app, use the deploy kit in
[lonunjie/om](https://github.com/lonunjie/om/blob/main/deploy/README.md): verify the signed release, then upload it to any static host.

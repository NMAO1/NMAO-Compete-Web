# NMAO Compete — web (compete.nmao.us)

Hosts the **universal-link** support for the NMAO Compete (Tournament competitor) app.

- `.well-known/apple-app-site-association` — Apple app↔domain association. ✅ `appID` = `BYS8GWQB7Y.us.nmao.compete`, paths `/invite*`.
- `.nojekyll` — REQUIRED so GitHub Pages doesn't drop the dotted `.well-known/` folder.
- `CNAME` — custom domain `compete.nmao.us`.
- `invite/index.html` — fallback landing: tries `nmao-compete://invite?t=…`, else App Store (fill `APPSTORE_ID_PLACEHOLDER` once the App Store Connect record exists).

Deploy: publish this repo, enable GitHub Pages (main / root), custom domain compete.nmao.us, add the DNS CNAME → nmao1.github.io.

# shrike-website

The website for [Shrike](https://github.com/privkeyio/shrike), an unofficial fork of Sparrow Bitcoin Wallet that follows the BLAKE2b proof-of-work hardfork.

Plain static HTML and one stylesheet. There is no build step and no dependencies.

## Local development

```bash
npx serve .
```

## Deployment

Upload the repository contents to any static host. Paths are root-relative, so the site has to be served from the root of a domain rather than a subdirectory. Add a `CNAME` file with the domain when one is chosen.

## Structure

```
index.html              landing page
features/index.html     what the fork changes
download/index.html     releases and verification
docs/                   index, replay-protection, connect-node, building, faq
assets/css/main.css     the only stylesheet
assets/images/          screenshots, taken from the Shrike repository
```

Each page carries its own copy of the header and footer. Changing navigation means editing all eight files, which is the trade for having no build step.

## Content

The copy is written for this fork and the screenshots come from `docs/images/` in the Shrike repository. Nothing here is taken from sparrowwallet.com: that site's content is separately copyrighted and the Apache 2.0 licence on Sparrow's source does not extend to it.

Facts that mirror the application (activation heights, the `0x21` hash type, artifact names, the signing key fingerprint) are checked against the Shrike repository and need updating here when they change there.

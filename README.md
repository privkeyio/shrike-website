# shrike-website

The website for [Shrike](https://github.com/privkeyio/shrike), an unofficial fork of Sparrow Bitcoin Wallet that follows the BLAKE2b proof-of-work hardfork.

Static HTML and one stylesheet. No build step, no dependencies.

```bash
npx serve .
```

Deployed with GitHub Pages from `main`. Paths are root-relative, so it has to serve from the root of a domain rather than a subdirectory.

## Two things to keep true

**Write the copy, do not borrow it.** Upstream's site is separately copyrighted and the Apache 2.0 licence on Sparrow's source does not cover it. Screenshots come from the Shrike repository.

**Facts here mirror the application.** Activation heights, sighash constants, artifact names, minimum node versions and the signing key are duplicated from the Shrike repository and go stale silently. Check them against it when anything there changes.

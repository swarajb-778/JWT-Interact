# JWT in Three Parts

An interactive, plain-English reading of **The JWT Handbook** (v0.14.2) by Sebastián E. Peyrott, all eight chapters, rebuilt as something you press on rather than read.

Recreated by **Swaraj Bangar** ❤️

## What's here

| Page | Covers | What you can do on it |
|---|---|---|
| `index.html` | Front door | Switch a specimen token between its three shapes; pick where to start; jump to any chapter |
| `part-1.html` | Chapters 1–3 | Decode a token by clicking it, run a session simulator, play attacker in three labs, build a token from JSON |
| `part-2.html` | Chapters 4–5 | Generate real RSA and ECDSA key pairs, fail to forge with a public key, really encrypt something and watch the seal break |
| `part-3.html` | Chapters 6–8 | Watch one letter move half a hash, build HMAC by hand, break an RSA key, draw on an elliptic curve |

## It really runs

Every cryptographic operation happens in your browser through the Web Crypto API, real HMAC-SHA256, real RSA and P-256 key pairs, real AES-GCM encryption. Nothing you type is sent anywhere, and there is no backend.

**None of this is production code.** Real systems need battle-tested libraries, careful key handling and proper testing.

## Running it locally

Every page is a single self-contained HTML file. Open one directly:

```
open index.html
```

Or serve the folder if you prefer a local URL:

```
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Publishing it

The folder is ready for GitHub Pages as-is, no build step, no dependencies. Push it to a repository, turn Pages on, and the site is live.

## Credits

- **Source material:** [The JWT Handbook](https://auth0.com/resources/ebooks/jwt-handbook) by Sebastián E. Peyrott, published by Auth0. The structure, specifications and examples throughout come from it.
- **Chapter 8** draws on the IETF OAuth Working Group's [JWT Best Current Practices](https://tools.ietf.org/wg/oauth/draft-ietf-oauth-jwt-bcp/) draft.
- The wristbands, coat checks, railway tickets, rubber stamps, suggestion boxes, locked trunks and signature books are this retelling's own, added so the ideas land without a background in cryptography.
- Set in Schibsted Grotesk with IBM Plex Mono for code, loaded from Google Fonts.

The original handbook is Auth0's work and remains theirs. This is an independent educational retelling.

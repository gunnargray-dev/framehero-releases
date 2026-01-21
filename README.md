# FrameHero Releases

This repository hosts the Sparkle appcast and release downloads for FrameHero.

## Appcast URL

```
https://gunnargray-dev.github.io/framehero-releases/appcast.xml
```

## Release Process

1. Build and archive FrameHero in Xcode
2. Export with Developer ID signing
3. Create DMG and notarize
4. Sign with Sparkle: `~/Downloads/bin/sign_update FrameHero-X.Y.Z.dmg`
5. Create GitHub Release with DMG attached
6. Update `appcast.xml` with new version entry
7. Push to trigger GitHub Pages rebuild

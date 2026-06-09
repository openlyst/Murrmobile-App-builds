# Murrmobile Builds

Automated multi-platform builds for [Murrmobile](https://gitlab.com/HttpAnimations/Murrmobile-App).

## Platforms

| Platform | Format | Runner |
|----------|--------|--------|
| iOS | Unsigned IPA | macos-latest |
| Android | APK + AAB | ubuntu-latest |
| Windows | ZIP (x64) | windows-latest |
| Linux | ZIP (x64) | ubuntu-latest |
| macOS | Unsigned ZIP | macos-latest |

## Usage

1. Push this repo to GitHub.
2. Go to **Actions > Build Murrmobile > Run workflow**.
3. Select platforms and optionally specify a commit hash.
4. Artifacts are uploaded and a release is created automatically.

## Secrets (Optional)

To enable release signing for Android, add these repository secrets:

- `ANDROID_KEYSTORE_BASE64` - Base64-encoded keystore
- `ANDROID_KEYSTORE_PASSWORD`
- `ANDROID_KEY_PASSWORD`
- `ANDROID_KEY_ALIAS`

Without these, Android builds use debug signing.

## License

Same as the upstream Murrmobile-App project.

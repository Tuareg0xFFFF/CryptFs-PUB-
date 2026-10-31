# CryptFs Vault Support

CryptFs Vault (shown as CryptFs on your device) opens and creates encrypted vaults in the gocryptfs format on iPhone, iPad and Mac. Here is how to get help, report a problem, or ask for a feature.

Last updated: October 31, 2026

## Getting help

Open an issue on GitHub:

**https://github.com/Tuareg0xFFFF/CryptFs-PUB-/issues**

## Before you open an issue

1. If a vault does not open, check that the vault folder contains `gocryptfs.conf` and that you are using the vault's password.
2. If a vault in iCloud Drive or Dropbox shows missing or old files, open the same folder in the Files app, Finder or the Dropbox app to check that the storage service has finished syncing it.
3. If a vault does not appear in the Files app or Finder, check that "Show in Files" (on iPhone and iPad) or "Show in Finder" (on Mac) is on for it in Settings, and that the vault is unlocked.
4. Make sure you have the latest CryptFs from the App Store.

## Reporting a bug

Please include:

- **CryptFs version:** Settings › About › Version.
- **Device and system:** the iOS, iPadOS or macOS version and the device model.
- **Where the vault is:** iCloud Drive, Dropbox, or a folder on the device, and which tool created it (CryptFs, or gocryptfs and its version).
- **Steps to reproduce**, what you expected, and what happened.
- **Screenshots or a screen recording**, if they help.

Do **not** post your vault password, the vault's `gocryptfs.conf`, encrypted files from the vault, or your Dropbox details in a public issue.

## Frequently asked questions

**Which vaults does CryptFs open?**
Vaults made with gocryptfs 1.0 or later, including the `-xchacha`, `-plaintextnames`, `-deterministic-names` and `-longnamemax` options, and vaults made by CryptFs. It cannot open reverse-mode vaults (`gocryptfs -reverse`), vaults protected with a FIDO2 security key, or vaults made with gocryptfs before 1.0; it tells you which one it found.

**Can I use the same vault with gocryptfs on my computer?**
Yes. CryptFs reads and writes the gocryptfs format, so the same vault works with gocryptfs on Linux or macOS, for example in a Dropbox folder that both use.

**I forgot my vault password. Can you recover it?**
No. Nobody can: the password is not stored anywhere, and the vault cannot be decrypted without it. If you saved the master key that gocryptfs printed when it created the vault, gocryptfs on a computer can open the vault with it (`gocryptfs -masterkey`).

**Where are my files?**
In the vault folder you chose: in iCloud Drive, in Dropbox, or in a folder on your device. CryptFs stores them encrypted there and decrypts them on your device when you open them.

**What does it cost?**
One purchase (US $3.99) covers iPhone, iPad and Mac.

**Is CryptFs part of gocryptfs?**
No. CryptFs is an independent app that is compatible with the gocryptfs vault format. gocryptfs is a separate open-source project.

**Does CryptFs send my data anywhere?**
Only to the storage you choose, and only encrypted: iCloud Drive, or Dropbox if you connect it. See [PRIVACY.md](PRIVACY.md).

**How do I delete my data?**
Remove the vault from CryptFs's list, and sign out of Dropbox in Settings. The details are in [PRIVACY.md](PRIVACY.md#deleting-your-data).

## Feature requests

Open an issue whose title starts with "Feature request:", and describe what you are trying to do.

## Privacy

See [PRIVACY.md](PRIVACY.md) for the privacy policy.

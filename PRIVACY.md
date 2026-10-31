# Privacy Policy for CryptFs Vault

Last updated: October 31, 2026

CryptFs Vault (shown as CryptFs on your device) opens and creates encrypted folders, called vaults, in the [gocryptfs](https://github.com/rfjakob/gocryptfs) format on iPhone, iPad and Mac. This policy covers the app on all three.

## The short version

- CryptFs collects nothing for the developer. There are no analytics, no tracking, no ads, and no CryptFs account or server.
- Your files are encrypted and decrypted on your device. Your vaults stay where you keep them: in iCloud Drive, in Dropbox, or in a folder on your device.
- Besides that storage, CryptFs contacts only Dropbox, and only if you connect it. Details below.

## What CryptFs connects to

**The storage you choose.** Vaults live in iCloud Drive, in Dropbox, or in a folder on your device. CryptFs encrypts file contents and file names on your device before they are written there, so the storage service receives only the encrypted vault: encrypted contents and encrypted names, with the sizes and dates that every stored file has.

**Dropbox, if you connect it.** You sign in on Dropbox's own page; CryptFs never sees your Dropbox password. CryptFs then talks directly to Dropbox to list, read and write your encrypted vaults, and asks Dropbox for the name of the connected account, to show which account is signed in. Your Dropbox account is subject to [Dropbox's privacy policy](https://www.dropbox.com/privacy).

**iCloud Drive.** Vaults in iCloud Drive are stored by Apple in your iCloud account, subject to [Apple's privacy policy](https://www.apple.com/legal/privacy/).

**Nothing else.** CryptFs never contacts a server run by the developer.

## Passwords and keys

- Your vault password is used on your device to unlock the vault. It is not stored.
- While a vault is unlocked, its key is kept in the Keychain so that the Files app and Finder can open your files. If you turn on Unlock with Face ID or Touch ID, the vault's key is kept in the Keychain, protected by it.
- These Keychain items, and the Dropbox sign-in, stay on this device: they are not synced to your other devices or to iCloud Keychain.
- Face ID and Touch ID are handled by your device. CryptFs never receives biometric data.

## What is stored on your device, and where

Everything stays in CryptFs's own storage on the device: the list of your vaults and their settings, and the keys and the Dropbox sign-in in the Keychain. When you open files through CryptFs, the Files app or Finder, the system keeps decrypted copies on your device while the vault is unlocked. When a vault locks, CryptFs removes them; changes that have not been written to the vault yet are kept on the device until you unlock it again, so that they are not lost.

CryptFs writes short diagnostic messages to your device's system log. They are designed not to contain file names, folder names, passwords or keys, and they stay on your device unless you share them.

## Apple devices

The App Store handles purchases and updates. If you have chosen to share analytics with app developers, Apple may pass the developer crash reports and aggregate usage figures. That is an Apple setting you can turn off: Settings › Privacy & Security › Analytics & Improvements on iPhone and iPad, and System Settings › Privacy & Security › Analytics & Improvements on Mac.

## Deleting your data

- Removing a vault from CryptFs's list locks it and deletes its keys and settings from your device. The encrypted vault itself stays where it is, under your control.
- Signing out of Dropbox in Settings deletes the sign-in from your device and asks Dropbox to end it.
- Deleting the app removes its data from the device. Apple devices can keep Keychain items after an app is deleted, so remove your vaults and sign out of Dropbox first if you want the keys and the sign-in gone straight away.

## Children's privacy

CryptFs collects no data from anyone, including children under 13.

## Changes to this policy

Updates are posted on this page with a new date.

## Contact

Questions about this policy: open an issue at https://github.com/Tuareg0xFFFF/CryptFs-PUB-/issues.

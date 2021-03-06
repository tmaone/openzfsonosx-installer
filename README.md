openzfsonosx-installer
======================

### How to run it:
`./make-installers.sh`

### Requirements:
- macOS 10.8 Mountain Lion, 10.9 Mavericks, 10.10 Yosemite, 10.11 El Capitan, 10.12 Sierra, 10.13 High Sierra
- http://s.sudre.free.fr/Software/files/Packages.dmg
- ~/Library/Keychains/openzfs-login.keychain added to Keychain Access.app
- Autotools, compiler, etc.

Caveat: If you do not have access to openzfs-login.keychain, at the moment you  
need to comment out all of the Mavericks and code signing sections.  

### Configuration options:

make-installers.sh
- `should_make_108`
- `should_make_109`
- `should_make_1010`
- `should_make_1011`
- `should_make_1012`
- `should_make_1013`
- `should_make_dmg`
- `require_version2_signature`
- `make_only`

scripts/make-pkg.sh
- `version`
- `owner`
- `dev_id_application`
- `dev_id_installer`
- `keychain`
- `keychain_timeout`
- `should_unlock`
- `should_sign_installer`
- `require_version2_signature`

scripts/make-dmg.sh
- `should_arrange`
- `should_detach`

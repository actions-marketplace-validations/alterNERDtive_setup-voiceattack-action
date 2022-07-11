# Setup VoiceAttack

Setup VoiceAttack for referencing in .Net Projects.

Downloads the VoiceAttack installer from the official website and installs it
on the worker. The installation folder is cached for future runs to increase
performance and minimize traffic caused for the VoiceAttack download site.

## Usage

### Inputs

* `path`: Installation path. Default: `"C:\\Program Files\\VoiceAttack"`
* `beta`: Whether or not to download the beta installer for VoiceAttack. Do
  note that a beta is not always available. Default: `false`.
* `version`: While this is not actually a VoiceAttack version to download (only
  the latest version is available), it is recommended to set this to the
  current VoiceAttack version. Changing this value will invalidate the cache
  and force a re-download. Default: `0`.

## Example

```yaml
- name: Install VoiceAttack
  uses: alterNERDtive/setup-voiceattack-action@v1
  with:
    version: "1.10"
```

[![GitHub Sponsors](https://img.shields.io/github/sponsors/alterNERDtive?style=for-the-badge)](https://github.com/sponsors/alterNERDtive)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/S6S1DLYBS)

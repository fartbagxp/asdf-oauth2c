# asdf-oauth2c

![Lint](https://github.com/fartbagxp/asdf-oauth2c/workflows/Lint/badge.svg)
[![License](https://img.shields.io/badge/license-MIT-blue)](https://choosealicense.com/licenses/mit/)
[![Doc](https://img.shields.io/badge/Doc-asdf-blue)](https://asdf-vm.com/)

This is a [oauth2c](https://github.com/SecureAuthCorp/oauth2c) plugin for the [asdf version manager](https://asdf-vm.com/).

## Contents

- [Plugin Dependencies](#plugin-dependencies)
- [Install](#install)
- [License](#license)

## Plugin Dependencies

- `curl` - for oauth2c downloads from upstream releases
- `grep` - to pull checksum text from the checksum file
- `sha256sum`, `sha256` or `shasum` - to verify checksum for integrity check with a file

## Install

Plugin:

```bash
asdf plugin-add oauth2c https://github.com/fartbagxp/asdf-oauth2c
```

oauth2c:

```bash
# Show all installable versions
asdf list-all oauth2c

# Install specific version
asdf install oauth2c latest

# Set a version globally (in your ~/.tool-versions file)
asdf global oauth2c latest

# Run oauth2c
oauth2c --version
> oauth2c 1.12.2
[...]
```

## Uninstall

```bash
asdf plugin remove oauth2c
```

## License

See [LICENSE](LICENSE).

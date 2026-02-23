# moukrea/rpm-repo

RPM package repository for opaq, hosted on GitHub Pages.

## Installation

```bash
# Add repository
sudo tee /etc/yum.repos.d/moukrea.repo << 'EOF'
[moukrea]
name=moukrea Repository
baseurl=https://moukrea.github.io/rpm-repo/
gpgcheck=1
gpgkey=https://moukrea.github.io/rpm-repo/pubkey.gpg
enabled=1
EOF

# Install
sudo dnf install opaq
```

## Upgrade

```bash
sudo dnf upgrade opaq
```

## Uninstall

```bash
sudo dnf remove opaq
```

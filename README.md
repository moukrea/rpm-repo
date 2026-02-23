# moukrea/rpm-repo

RPM package repository for Fedora/RHEL/CentOS, hosted on GitHub Pages.

## Adding the Repository

```bash
sudo tee /etc/yum.repos.d/moukrea.repo << 'EOF'
[moukrea]
name=moukrea Repository
baseurl=https://moukrea.github.io/rpm-repo/
gpgcheck=1
gpgkey=https://moukrea.github.io/rpm-repo/pubkey.gpg
enabled=1
EOF
```

## Available Packages

| Package | Description |
|---------|-------------|
| `opaq` | Credential manager — keeps secrets out of terminals, context windows, and command output |

Install any package with:

```bash
sudo dnf install <package-name>
```

# Gitea Examples

> Note: all command line arguments can be set in your $HOME/.config/ghorg/conf.yaml

clone an **org**

```
ghorg clone <gitea_org> --base-url=https://<your-internal-gitea>.com --token=XXXXXXX
```

clone a **users** repos

```
ghorg clone <gitea_username> --clone-type=user --base-url=https://<your-internal-gitea>.com --token=bGVhdmUgYSBjb21tZW50IG9uIGlzc3VlIDY2
```

clone all repos from a **github org** that are **prefixed** with "frontend" **into a folder** called "design_only"

```
ghorg clone <gitea_org> --match-regex=^frontend --output-dir=design_only --base-url=https://<your-internal-gitea>.com --token=XXXXXXX
```

# LDE Official Plugins

The official plugin market of [LDE](https://github.com/ibraheem-ghazi), the Laravel Development
Environment. LDE lists it under **Settings ▸ Plugins ▸ Market** as **LDE Official**; every
plugin here is first-party.

## What's here

- `market.json` — the market index LDE reads, from
  `https://raw.githubusercontent.com/ibraheem-ghazi/lde-official-plugins/main/market.json`.
- `market.json.sig` — its Ed25519 signature. LDE carries the official public key and lists
  nothing from this market unless the signature holds.
- `icons/`, `docs/` — each plugin's icon and description.
- Packages (`.ldeplugin`) are attached to this repository's **releases**, tagged
  `<id>-v<version>`. Each is signed with the same key; LDE refuses an official package that
  isn't.

Official key fingerprint: `f983·8e7f·72c5·43b9`.

## Publishing

From the LDE repository: `plugins/publish.sh [--build] [--changes "<text>"] <id>…` packs,
signs, releases, lists and pushes. Hand-edited fields of an entry (icon, description,
categories, keywords, homepage, wanted) are kept by later publishes; sign again after editing:
`lde-pack market sign market.json --key <official key>`.

## Your own market

Any repository can be a market: put a `market.json` at its root (`lde-pack market init`,
`lde-pack market add`, `lde-pack market sign`) and add `owner/repo` in LDE under
Market ▸ Sources. See LDE's `docs/PLUGINS.md`, "Plugin markets".

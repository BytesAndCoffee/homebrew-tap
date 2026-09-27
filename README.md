# BytesAndCoffee Homebrew tap

Formulae for [Bad Decisions](https://github.com/BytesAndCoffee/bad-decisions),
an unofficial, unaffiliated fan-made party card game.

## regret

`regret` is the terminal client for a Bad Decisions service: deal rounds, list
packs, check provenance, and play Peer Pressure multiplayer rooms.

```bash
brew install bytesandcoffee/tap/regret
regret deal
man regret
regret doctor   # checks the install and prints fixes; changes nothing
```

Homebrew is the suggested install on macOS and Linux: it also links the
`regret(1)` manual page, so `man regret` works without any shell setup. The
client is also on PyPI as
[`bad-decisions-client`](https://pypi.org/project/bad-decisions-client/).

## Maintenance

`Formula/regret.rb` is copied from
[`homebrew/regret.rb`](https://github.com/BytesAndCoffee/bad-decisions/blob/main/homebrew/regret.rb)
in the main repository, which is the source of truth. After each release,
update it there (see `docs/RELEASING.md`, step 7) and copy it here; the
`brew test-bot` workflow builds and tests every change on macOS and Linux.

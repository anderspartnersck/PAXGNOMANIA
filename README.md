# PAX GNOMANIA

The gnome legion storms Gunpowder, Maryland. You fly the saucer.

## ▶ [PLAY IT IN YOUR BROWSER](https://anderspartnersck.github.io/PAXGNOMANIA/)

A Castle Killscreen game by **Anders & Partners**.

> ### ⚠︎ Working build — not a finished game
>
> **This is a reskin riding on SUCK UP's art.** The gnome-specific sprites largely don't exist yet, so you're seeing SUCK UP's cast standing in. The engine underneath is a feel-proof sandbox, not a shipping vehicle.
>
> The finished Castle Killscreen titles are **[SUCK UP](https://anderspartnersck.github.io/suck-up/)**
> and **[ONE-TIMER: THE HIGH TABLE](https://anderspartnersck.github.io/high-table/)**. This repo
> exists so the work can happen in the open, not because the work is done.

## About

The lore reskin of [SUCK UP](https://anderspartnersck.github.io/suck-up/) — the
Roman Ornithopter Corps against a gnome army, fought across three fronts. Same
air-cushion flight, same shared pressure, different war.

*(Working title: HADRIAN'S ANCIENT AIR FORCE — the two names are the same game.)*

There are **two** Pax Gnomania builds and this is the web one. The other is a
separate Python/pygame game living in the `HADRIAN'S ANCIENT AIR FORCE` tree,
which has no web build at all.

## How to play

| | |
|---|---|
| **Move** | Arrow keys or **WASD** |
| **Beam** | **SPACE** — hold it over a gnome to lift him |
| **Start / continue / retry** | **SPACE** (or **R** to run it again) |
| **B** | drop straight into the siege |

**SPACE** from the menu runs the fronts in order: **Gunpowder Falls → Barracks → Fort**.

Two cabinets, by URL: [`?cab=hyscore`](?cab=hyscore) (classical) and
[`?cab=blacksite`](?cab=blacksite) (red).

## What still needs work

- **Sprites are SUCK UP's.** Gnome-legion art is the main outstanding job.
- The engine is the AIRY sandbox — built to prove the glide feel, never intended as the shipping renderer.
- Ships the full SUCK UP asset set because the page builds every art path by concatenation; pruning can't be done safely.

## Rebuilding this bundle

This repo is **generated** — never edit it directly. Everything here is built from the
private Castle Killscreen tree:

```
cd "ANDERS CASTLE KILLSCREEN/SUCK UP"
python3 tools/build_pax_pages.py
```

The bundler shrinks art by **resolution, not by pruning**: these engines build most asset
paths by string concatenation, so a static scan can't see what's used, and a wrongly-cut
sprite doesn't error — it just silently fails to draw.

## Credits

Created by **Joseph Coleman**, with Claude and ChatGPT.
Anders & Partners.

<sub>Generated from the private Castle Killscreen tree. Edit there, not here.</sub>

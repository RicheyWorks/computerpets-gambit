# Gambit

**Pet Card Duel** — Collectible card game where pet traits become abilities — cards mirror what you actually own.

Part of the [ComputerPets](https://github.com/RicheyWorks/computerpets) universe. Map: [computerpets-ecosystem](https://github.com/RicheyWorks/computerpets-ecosystem).

> Status: **design scaffold**. Gameplay contract is frozen. Engine choice is the one in the brief. Implementation comes next.

## Loop

You cannot play a dragon if you do not have one. Gambit decks are projections of owned pets + traits. Proxies in casual; ranked is ownership-checked via Minter.

## Genre & engine

- Genre: **CCG**
- Engine: **Next.js / WebGL**
- Stack: TypeScript · Next.js · WebGL board · trait cards from owned pets · server-authoritative duels
- Default surface: `3000`

## How you play

1. Build a 30-card deck from owned traits.
2. Best of 3, turn clock.
3. Card art from Atelier / Studio.
4. Ranked rewards = cosmetics + treats.

## Talks to

- computerpets-minter
- computerpets-lore
- computerpets-ledger
- computerpets-steamgate
- computerpets-arena

## Failure doctrine

Sold NFT mid-queue → deck illegal, match cancel. Disconnect → timer concedes. Scripted combo overflow → cap chain at 16.

Canon rules that never yield:

- 210 living kinds. No illegal hybrids.
- Overlay pets can get tired, sick, or hide. Tokens are not burned by a minigame.
- Desktop walk stays the main quest. Closing Gambit must leave Rui walking.

## Layout

```
computerpets-gambit/
  README.md
  LICENSE
  docs/DESIGN.md
  src/                implementation lands here
```

## Run (Windows)

```powershell
cd app; npm install; npm run dev
```

Meet Rui first via the [flagship start-here](https://github.com/RicheyWorks/computerpets/blob/main/docs/START-HERE.md). This game is optional.

## License

MIT. See [LICENSE](LICENSE).

---

*Two hundred ten living kinds. Keep them so a line does not go quiet.*

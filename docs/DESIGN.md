# Gambit design

Implement against this file, not folklore.

## Identity

- Product: **Gambit**
- Repo: `computerpets-gambit`
- Idea: Pet Card Duel
- Genre: CCG
- Engine: Next.js / WebGL
- Surface: `3000`

## Loop

You cannot play a dragon if you do not have one. Gambit decks are projections of owned pets + traits. Proxies in casual; ranked is ownership-checked via Minter.

## Play beats

- Build a 30-card deck from owned traits.
- Best of 3, turn clock.
- Card art from Atelier / Studio.
- Ranked rewards = cosmetics + treats.

## Neighbors

- computerpets-minter
- computerpets-lore
- computerpets-ledger
- computerpets-steamgate
- computerpets-arena

## Failure doctrine

Sold NFT mid-queue → deck illegal, match cancel. Disconnect → timer concedes. Scripted combo overflow → cap chain at 16.

## Hard rules

1. Minigames cannot mint or burn NFTs by themselves (Minter is the write path).
2. Stats come from lived overlay care + Dojo caps, not cash shop.
3. Species kits stay inside Lore. Illegal hybrids never spawn.
4. Fail soft: the desktop overlay process is not this process.

# WondoGo — One-Price All-Inclusive Vacation Platform (Prototype Portal)

WondoGo is a high-fidelity prototype portal for a one-price, all-inclusive
vacation platform. One itinerary, one timeline, one butler — instead of a
wallet full of sub-vouchers.

What the prototype shows:

- **One itinerary, not a voucher wallet.** A single timeline, one
  "everything is ready" state, and one butler who already has the context
  (flight, dietary needs, celebration, arrival time).
- **A shared inventory pool** that makes overselling structurally impossible:
  a sold-out pool delists every package referencing it.
- **Price snapshots for settlement.** The price is locked the moment payment
  succeeds; unpaid orders re-price behind an explicit confirmation gate.
- **Six themes, WCAG AA.** One design system, one set of design tokens,
  six themes with an automated contrast validator.

## Open it locally

Double-click `index.html`, or serve the folder and open it in a browser:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000/
```

No build step, no backend, no login. Every page is a static snapshot.

## Contents

| Folder | Surface |
| --- | --- |
| `01-C端消费者` | Consumer — discover, detail, order, itinerary, butler |
| `02-商家端` | Merchant — dashboard, resources, verification, settlement |
| `03-平台运营端` | Platform operations — dashboard, orders, arbitration, config |
| `04-租户端` | Tenant — lightweight operations workbench |
| `05-企业与管家端` | Enterprise & butler — corporate demand, butler console |
| `06-平台财务端` | Platform finance — settlement, split, ledger |

`manifest-md5.json` records the MD5 of every page for integrity checking.

## How Kiro was used

In the design phase we used Kiro steering: a custom steering skill,
`ui-ux-pro-max` (`.kiro/steering/ui-ux-pro-max`), that generates
design-system recommendations — styles, color palettes, font pairings,
UX guidelines — from a searchable database. It drove the six-theme design
system behind these screens.

## License

MIT — see `LICENSE`.

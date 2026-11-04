# Vobiscum Configurator

A configurator for the Vobiscum road-car range. Pick a model and trim, add packages, and see the specification and price update live. Builds can be saved and given a shareable build code. A separate Motorsport page showcases the Spitfire LM and GP.

It's a single self-contained `index.html` with no build step. Open it in a browser or serve the folder with GitHub Pages.

## How it works

1. **Model:** V1, V2, V3, V5, V6, Firefly or Dragonfly.
2. **Trim:** each trim fixes its engine. Firefly's trims are shown in pairs, with Clubsport and GT4 as the sharper versions of the S and R.
3. **Packages:** only the packages offered on that trim appear. Packages that come built in on a trim aren't listed.
4. **Summary:** line items, total and a build code such as `FIREFLY-CS-CARBON.TECH`.

## Package rules

| Package | Price | Effect on the figures |
|---|---|---|
| Technology | £2,000 | — |
| Driver Assistance | £1,800 | — |
| Shadow | £1,200 | — |
| Performance | £3,500 | — |
| Lightweight | £4,000 | −35 kg, −0.1 s to 60 |
| Race | £5,500 | −0.1 s to 60 |
| Carbon | £6,000 | −10 kg; includes Shadow at no extra cost |
| Aerodynamic | £7,500 | −4 mph top speed (not on electronically limited cars) |

| Trims | Optional packages |
|---|---|
| V1 18/20, V2/V3 20, V5/V6 30 | Technology, Driver Assistance, Shadow |
| V1 30, V2/V3 30, V5/V6 40 | + Performance |
| V1 S | Technology, Driver Assistance, Shadow, Lightweight, Race, Carbon, Aerodynamic |
| V2/V3/V5/V6 S | Technology, Driver Assistance, Shadow, Lightweight, Carbon |
| V2/V3/V5/V6 R | Technology, Driver Assistance, Shadow, Lightweight, Race, Carbon, Aerodynamic |
| Firefly | Technology, Driver Assistance, Shadow, Performance |
| Firefly S, R | Technology, Driver Assistance, Shadow, Race, Carbon, Aerodynamic |
| Firefly Clubsport | Technology, Driver Assistance, Shadow, Carbon, Aerodynamic |
| Firefly GT4 | Technology, Driver Assistance |
| Dragonfly RWD, AWD | Driver Assistance, Shadow, Carbon, Race, Aerodynamic |
| Dragonfly GT3 | Driver Assistance |

## Editing the data

All models, trims, engines and packages live in the `DATA` block at the top of the script in `index.html`. Change a price, figure or package list there and the whole configurator follows. Nothing else needs touching.

## Saved builds

Outside Claude, saved builds are stored in your browser.

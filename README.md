# The Atlas of Robinson Crusoe

An interactive map and timeline of every voyage, coast, and camp in Daniel Defoe's
*Robinson Crusoe* (1719) — plotted, dated, and sourced against the text.

**Live site: <https://bip-river.github.io/Robinson-Crusoe/>**

## What's in it

- **38 mapped places** — 20 on the world map, from his birth in York in 1632 through Hull,
  the Guinea coast, captivity in Salé, Brazil, and the wreck, to his eventual return; plus
  18 on a reconstructed plan of the island itself (the castle, the bower, the corn ground,
  the footprint in the sand).
- **An island drawn as geography, not as a list** — a named coastline with the bay he came
  ashore in, the creek where he kept his canoe, Castle Hill and its rock face, the vale, the
  goat country and the far shore the cannibals resorted to, with the bearing to the mainland
  he could see from the high ground. The only tracks drawn are journeys he actually describes
  making: his circuit to the bower and the enclosures, the raft trips out to the wreck, and
  the canoe voyage that nearly carried him away on the current.
- **Routes a ship could actually have sailed** — the voyages follow period tracks rather than
  straight lines: down Channel and out past the Canaries and Cape Verde on the trades, the
  wide westward arc to Brazil, and the return north on the Gulf Stream and east on the
  westerlies. The last leg home from Lisbon is drawn overland across Spain and the Pyrenees,
  because that is how Crusoe travels it, having had enough of the sea.
- **A scrubable timeline** that walks the narrative in order, with play/step controls, each
  event carrying its narrative date, its calendar date, a summary, and the quotation from
  the novel it rests on.
- **Confidence marking** on every location — `explicit` where Defoe names the place,
  `strong` where it is a firm inference, `speculative` where it is a reasoned guess — so
  the map never pretends to more certainty than the book supports.
- **Where the island actually is** — Tobago as the best textual fit near the mouth of the
  Orinoco, alongside Más a Tierra in the Pacific, where Alexander Selkirk was really
  marooned. The inspiration and the setting are two different islands.
- **Three visual themes**: Parchment, Modern, and Night.

## How it's built

A single static `index.html` — all markup, styles, data, and logic inline. No build step, no
dependencies to install, nothing to compile. Open the file in a browser and it runs.

To work on it locally:

```sh
python3 -m http.server
# then open http://localhost:8000/
```

GitHub Pages serves the `main` branch from the repository root. Pushing a change to
`index.html` on `main` publishes it. The empty `.nojekyll` file tells Pages to publish the
tree as-is rather than running it through Jekyll.

## Credits

Mapping by [Leaflet](https://leafletjs.com/). Basemap tiles by
[Carto](https://carto.com/attributions), built on data from
[OpenStreetMap](https://www.openstreetmap.org/copyright) contributors. Text and events drawn
from Defoe's novel, which is in the public domain.

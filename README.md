# USF Koret indoor pool page — Pool Relay embed preview

An unofficial replica of the University of San Francisco **Koret Indoor Swimming Pool**
page with a live [Pool Relay](https://www.poolrelay.com) lane calendar in place of the
linked spreadsheet.

**This is not a USF website.** The official page is
<https://www.usfca.edu/koret/facilities/indoor-swimming>. This is a working preview of one
proposed change to it, and the page says so in a ribbon across the top.

## What it replaces

The live page says: *"it is recommended to check our Pool Lane Schedule before each visit
to avoid lane closures and events"* — and that link opens a **Google Sheet**. A swimmer
deciding whether to come now has to open a spreadsheet and find today's column.

The same page also describes the schedule in prose — *"the pool will have limited lanes
from 4–6 p.m., Monday–Friday"* — which has to be kept in step with the spreadsheet by hand.

## Why this pool makes the point

Koret runs **speed lanes that move through the day**: Slow in lanes 2–5, Medium in 6–8,
Fast in 9–15 and the deep end, shifting as Masters, youth swimming and cleaning take the
water. That is what a swimmer actually wants to know and the hardest thing to write down.
The calendar shows it lane by lane.

```html
<iframe src="https://www.poolrelay.com/embed/guBdc45nE8tdP6ykKCUpoV"
        width="100%" height="780" style="border:0"
        title="Koret pool lane schedule"></iframe>
```

## Notes

- The calendar deliberately breaks **out of the text column** into a full-width band:
  seventeen lane columns will not fit a 600px measure, and a lane schedule squeezed until
  it scrolls sideways is the problem this page exists to solve.
- The tab is saved as a **Day** view with `fit: width`, so every lane fits the frame.
- Hero image hotlinked from usfca.edu. Fonts are Google substitutes.
- Navigation links point at the live site. `noindex` is set.

## Local preview

```
python3 -m http.server 8805
```

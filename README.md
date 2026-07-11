# FlightScope · 直飞航线探索 / Direct Route Explorer

Interactive 3D globe for exploring nonstop flight routes worldwide.
输入出发机场，在旋转地球上可视化全球直飞目的地与参考航班信息。

**Live site:** enable GitHub Pages, then open `index.html`.

## Data / 数据说明
Route topology from the **OpenFlights** open dataset (historical, ~2014; some routes have since changed),
plus a hand-curated supplement (recent routes & post-2014 airports like Beijing Daxing / Chengdu Tianfu).
Aircraft types from OpenFlights equipment records. **Flight numbers, times and fares are rule-generated
reference values — NOT live data.** Verify on airline websites before booking.

航线拓扑来自 OpenFlights 开放数据集（历史约 2014）+ 人工补充航线；机型取自真实执飞记录；
航班号/时刻/票价为规则生成的参考值，非实时数据。

## Files
- `index.html` — the app
- `flight-data.js` — global airport/route dataset (must stay next to index.html)

Libraries (three.js, topojson) and base map (world-atlas) load from public CDNs, so an internet
connection is required at runtime.

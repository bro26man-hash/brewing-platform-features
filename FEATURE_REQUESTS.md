# Community-Curated Feature Requests for Brewing Platform

> Aggregated and ranked from the most popular open-source homebrewing/brewing software repos on GitHub.
> Scoring: comments × 3 + recency + feature-label bonus, weighted by source-repo popularity.

---

## 🏆 Top 10 Most In-Demand Features

### #1 — Open / Permissive Licensing  
**Source:** [craftbeerpi/craftbeerpi #67](https://github.com/craftbeerpi/craftbeerpi/issues/67)  
**Score:** 204.2 | **Comments:** 31 | **Repo:** ★625  
**Why the community wants it:** The current CraftBeerPi license has long been a point of contention — contributors and users feel it restricts modifications and derivative works. The community overwhelmingly wants a permissive license (MIT/Apache) so they can freely adapt, fork, and integrate the code into commercial and hobbyist projects without legal friction.

---

### #2 — MQTT State/Mode/Value Change Notifications  
**Source:** [vitotai/BrewPiLess #435](https://github.com/vitotai/BrewPiLess/issues/435)  
**Score:** 92.5 | **Comments:** 3 | **Repo:** ★391 | **Updated:** Oct 2024 (very recent)  
**Why the community wants it:** Homebrewers increasingly use MQTT to integrate BrewPiLess with Home Assistant, Node-RED, and other smart-home dashboards. Currently, BrewPiLess only publishes MQTT messages on a fixed interval — users want instant push notifications whenever the device state, mode, target temp, or fridge setpoint changes. This enables real-time automation (e.g., "send a push notification when fermentation enters the next step").

---

### #3 — Sonoff TH Hardware Support  
**Source:** [vitotai/BrewPiLess #436](https://github.com/vitotai/BrewPiLess/issues/436)  
**Score:** 81.4 | **Comments:** 6 | **Repo:** ★391 | **Updated:** Oct 2024 (very recent)  
**Why the community wants it:** The Sonoff TH relay is one of the most popular budget ESP8266-based relays for homebrew temperature control. Supporting it natively would eliminate the need for custom firmware hacks and make BrewPiLess accessible to a much larger hardware community.

---

### #4 — Free-Rise Option in Beer Profiles  
**Source:** [vitotai/BrewPiLess #429](https://github.com/vitotai/BrewPiLess/issues/429)  
**Score:** 71.2 | **Comments:** 4 | **Repo:** ★391 | **Updated:** Oct 2024 (very recent)  
**Why the community wants it:** Many fermentation strategies (e.g., Karl S. / free-rise) call for the temperature to follow ambient conditions rather than holding a strict setpoint. A "free-rise" mode in beer profiles would let the controller skip active cooling/heating and simply log temperature, which is essential for certain yeast strains and recipe styles.

---

### #5 — Web UI Password / Authentication  
**Source:** [craftbeerpi/craftbeerpi #56](https://github.com/craftbeerpi/craftbeerpi/issues/56)  
**Score:** 63.3 | **Comments:** 7 | **Repo:** ★625  
**Why the community wants it:** CraftBeerPi's web interface has no authentication — anyone on the same network (or internet, if port-forwarded) can change temperature setpoints, start/stop logic, and modify recipes. Multiple users have requested at least basic HTTP auth (admin/password) to prevent accidental or unauthorized changes, especially for remote-access setups.

---

### #6 — Extra / Custom Hardware Support  
**Source:** [craftbeerpi/craftbeerpi #121](https://github.com/craftbeerpi/craftbeerpi/issues/121)  
**Score:** 63.3 | **Comments:** 7 | **Repo:** ★625  
**Why the community wants it:** Users want to plug in non-standard sensors, relays, and actuators beyond the default GPIO configurations. A pluggable hardware-abstraction layer (or documented addon system) would let the community add support for new devices without forking the core codebase.

---

### #7 — Dashboard: Show Active Fermenting Beer Name  
**Source:** [thorrak/fermentrack #716](https://github.com/thorrak/fermentrack/issues/716)  
**Score:** 58.0 | **Comments:** 4 | **Repo:** ★147 | **Updated:** Nov 2024 (very recent)  
**Why the community wants it:** When running multiple fermentation vessels, the dashboard currently doesn't make it obvious which beer is actively fermenting in each vessel. Displaying the beer name directly on the dashboard card would eliminate confusion and make the UI far more intuitive for multi-vessel setups.

---

### #8 — Floaty Hydrometer Integration  
**Source:** [thorrak/fermentrack #690](https://github.com/thorrak/fermentrack/issues/690)  
**Score:** 48.6 | **Comments:** 13 | **Repo:** ★147  
**Why the community wants it:** Floaty hydrometers are a popular low-cost alternative to the Tilt and iSpindel for measuring specific gravity during fermentation. The community has been asking for native support so that Floaty readings can be ingested, graphed, and analyzed alongside other sensor data.

---

### #9 — Timers & Hop Alarms  
**Source:** [craftbeerpi/craftbeerpi #61](https://github.com/craftbeerpi/craftbeerpi/issues/61)  
**Score:** 44.9 | **Comments:** 4 | **Repo:** ★625  
**Why the community wants it:** Homebrewers need timed alerts for hop additions (e.g., "60-minute hop timer started") and other scheduled events during the brew day. A built-in timer system with configurable alarms (buzzer, push notification, MQTT message) would significantly improve the brew-day experience.

---

### #10 — Multi-Recipe / Parallel Fermentation Management  
**Source:** [craftbeerpi/craftbeerpi #78](https://github.com/craftbeerpi/craftbeerpi/issues/78)  
**Score:** 38.8 | **Comments:** 3 | **Repo:** ★625  
**Why the community wants it:** Advanced homebrewers often run multiple concurrent fermentations (different beers, several stages). The current single-recipe-at-a-time model forces constant switching. A multi-recipe view with parallel temperature profiles would be a major quality-of-life improvement.

---

## Supplementary Ranked Issues (11–20)

| Rank | Feature | Source | Score | Comments |
|------|---------|--------|-------|----------|
| 11 | ESP Controller Disconnect Notifications | fermentrack #649 | 19.9 | 2 |
| 12 | iSpindel Battery Panel on Dashboard | fermentrack #626 | 18.7 | 5 |
| 13 | Graph Background Coloring Toggle | fermentrack #684 | 16.2 | 1 |
| 14 | dygraph Range Selector | fermentrack #648 | 16.2 | 1 |
| 15 | MQTT in Docker Container | craftbeerpi4 #117 | 15.0 | 4 |
| 16 | Dashboard Layout Fixes | craftbeerpi4 #107 | 15.0 | 4 |
| 17 | Scheduled Brew Start | craftbeerpi4 #114 | 13.7 | 2 |
| 18 | Double Mash Support | craftbeerpi4 #41 | 12.5 | 0 |
| 19 | TiltBridge Object Management | fermentrack #611 | 12.4 | 0 |
| 20 | iSpindel Fermentation Logic | craftbeerpi3 #246 | 11.7 | 3 |

---

## Methodology

- **Source repos:** craftbeerpi/craftbeerpi (★625), vitotai/BrewPiLess (★391), Manuel83/craftbeerpi3 (★183), craftbeerpi/craftbeerpi4 (★148), thorrak/fermentrack (★147)
- **Scoring formula:** `(comments × 3 + recency_score + feature_label_bonus) × (1 + repo_stars/600)`
- **Recency:** Based on last update date; newer = higher score
- **Feature signal:** +15 for explicit [FR] tag, +10 for `enhancement` or `Future` label, +5 for "request"/"suggestion" in title
- **Total issues analyzed:** 34 feature/enhancement issues across 5 repositories

*Issues tagged with "Future" in Fermentrack are maintainer-recognized roadmap items, indicating strong upstream alignment.*

---

## Created Issues in This Repo

| # | Issue | Link |
|---|-------|------|
| 1 | Open / Permissive Licensing | [Issue #1](https://github.com/bro26man-hash/brewing-platform-features/issues/1) |
| 2 | MQTT State Push Notifications | [Issue #2](https://github.com/bro26man-hash/brewing-platform-features/issues/2) |
| 3 | Sonoff TH Hardware Support | [Issue #3](https://github.com/bro26man-hash/brewing-platform-features/issues/3) |
| 4 | Free-Rise Mode in Profiles | [Issue #4](https://github.com/bro26man-hash/brewing-platform-features/issues/4) |
| 5 | Web UI Authentication | [Issue #5](https://github.com/bro26man-hash/brewing-platform-features/issues/5) |
| 6 | Plugin/Abstraction Layer for Hardware | [Issue #6](https://github.com/bro26man-hash/brewing-platform-features/issues/6) |
| 7 | Dashboard: Beer Name on Vessel Cards | [Issue #7](https://github.com/bro26man-hash/brewing-platform-features/issues/7) |
| 8 | Floaty Hydrometer Integration | [Issue #8](https://github.com/bro26man-hash/brewing-platform-features/issues/8) |
| 9 | Timers & Hop Alarms | [Issue #9](https://github.com/bro26man-hash/brewing-platform-features/issues/9) |
| 10 | Multi-Recipe Parallel Management | [Issue #10](https://github.com/bro26man-hash/brewing-platform-features/issues/10) |
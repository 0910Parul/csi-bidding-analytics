# Reading the Competition: Competitor Bidding Analytics for Sealed-Bid Construction Auctions

This project helps a highway-construction firm **win more sealed-bid auctions by reading its competitors**. Working with **Central Specialties Inc. (CSI)** — which bids across MN, ND, and SD — I analyzed **700+ competitor bids across 195+ first-price sealed-bid projects** and built an interactive **Tableau dashboard** of competitor bidding behavior, turning intuition-based bidding into data-informed strategy. Completed through the **Carlson Analytics Lab** (University of Minnesota).

## 🔍 Project Goals

- Give CSI a data-driven view of the competitive landscape in first-price, sealed-bid auctions.
- Profile each competitor's bidding frequency, pricing aggression, win share, and geographic patterns.
- Pinpoint the **close, winnable losses** and the specific competitors behind them — so CSI knows where a small price move recovers real work.

## 📄 Files Included

- **`CSI_dashboard.twbx`** — the interactive Tableau dashboard (competitor frequency, pricing aggression, win share, geography).
- **`CSI_Presentation.pdf`** — final client presentation, *"Bidding Behaviors of Top Competitors."*

> Raw bid data is client-confidential (Carlson Analytics Lab NDA) and is **not included** in this repo. Open the `.twbx` in **Tableau Desktop** or the free **Tableau Reader**.

## 🧪 Methods Used

- Cleaned and reshaped **700+ bids across 195+ projects** into a tidy bidder-level table (one row per bid).
- Ranked bidders per project (lowest sealed bid wins) and computed each bid's **spread vs. the winning bid**.
- Flagged CSI's wins vs. losses, then isolated **close losses** (CSI within 5% of the winning bid).
- Ran **competitor concentration** and **state-level pricing-aggression** analysis; delivered it all through Tableau.

## 📈 Key Findings

- **Close losses are concentrated in a few names.** Of CSI's losses, the genuinely winnable ones (within 5% of the winning bid) trace back overwhelmingly to a short list of competitors — **6 firms account for ~60% of all close losses** (derivation below).
- **Minnesota is CSI's most contested market** — win rate **19%** (22 of 113) — while **South Dakota is its strongest** at **~33%** (11 of 33).
- **Competitors price differently by region:** e.g., **Duininck** bids **~7% more aggressively** than CSI in MN, pressuring shared-bid margins, while **Joe Riley Construction** is highly selective (**41%** win rate on the jobs it chooses).

### How the ~60% was derived

Across the three core states (MN, ND, SD), CSI bid on **194 projects** and lost **171**. Restricting to **close losses** — bids where CSI came within **5% of the winning price** — leaves **34 winnable projects**. Grouping those by who won:

| Competitor | Close losses | Cumulative share |
|---|---|---|
| Duininck Inc | 5 | 15% |
| Knife River (Midwest) | 4 | 26% |
| Border States Paving | 3 | 35% |
| Anderson Brothers | 3 | 44% |
| Mark Sand & Gravel | 3 | 53% |
| Hough Inc | 2 | **59% ≈ ~60%** |

So **6 competitors are associated with ~60% (20 of 34) of CSI's close losses** — the exact names CSI should watch when a small, targeted price adjustment could flip a loss into a win.

## 🛠 Technologies

- Tableau (interactive dashboard, geographic bidding views)
- Python (pandas) — data cleaning, bid ranking, spread and concentration analysis
- SQL — data preparation
- Auction / sealed-bid analytics; competitor & market analysis

## ✅ Outcome

CSI moves from intuition-based bidding to a data-informed strategy: a named short-list of competitors driving its winnable losses, region-by-region pricing intelligence, and a dashboard leadership can filter by location to see who is likely to bid and how aggressively — before submitting its own number.

---

By **Parul Chaudhary** · [LinkedIn](https://www.linkedin.com/in/parulchaud) · [Email](mailto:parul.jaswant@gmail.com)

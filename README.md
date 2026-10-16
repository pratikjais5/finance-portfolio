# Finance Portfolio: Pratik Jais

Valuation, portfolio and trading models built at IIM Visakhapatnam. Live site: https://pratikjais5.github.io/finance-portfolio/

| Model | File | What it does | Result |
|---|---|---|---|
| Granules India | `models/Granules_India.xlsx` | DCF, NWC schedule, WACC (10.3%), 500-trial Monte Carlo, real option on peptide CDMO | Hold; fair value Rs 828 vs market Rs 854 |
| Unichem Laboratories | `models/Unichem_Laboratories.xlsx` | Restated statements, ratios, projected FCF, two terminal-value methods, relative valuation, football field | Target Rs 446 vs market Rs 581 |
| IAPM | `models/IAPM.xlsx` | DCF and relative value for M&M, Coforge, Dr. Reddy's, Britannia; max-Sharpe optimisation (5-40% bounds) | Sharpe 0.76; weights 40/25/10/25 |

Trading model dashboard: https://pratikjais5.github.io/trading-dashboard/

## How to read the workbooks
Start with the `Final Output` sheet in Granules and IAPM, and `Football field` in Unichem. Inputs are on the sheets named for each step (WACC, DCF, Projected FCF). Assumption rationale for Granules is in `Assumptions Rationale`.

## Known limitations
- Unichem's methods give a wide range (DCF exit multiple Rs 320 vs EV/EBITDA Rs 952).
- Granules' base case sits above the Monte Carlo median (Rs 708).
- IAPM's DCF and relative values differ sharply for Coforge.

## Contact
pratik.jais5@gmail.com | linkedin.com/in/pratik-jais

## Equity curve (optional)
Put a file named `equity.csv` next to `index.html` with the columns `date,strategy,nifty` (see `equity_template.csv`).
`date` is YYYY-MM-DD, `strategy` is simulated account equity in rupees, and `nifty` is the Nifty 50 closing level (it is rebased automatically). When the file is present the page shows an interactive curve with drawdowns; when it is missing the page shows the simple comparison instead.

## Visitor counter (optional)
Create a free account at goatcounter.com, then uncomment the snippet at the bottom of `index.html` and replace `YOURCODE`. Add `?ref=companyname` to the links you send, for example `https://pratikjais5.github.io/finance-portfolio/?ref=acme`, to see which email led to a visit.

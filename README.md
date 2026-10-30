<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.png">
  <img alt="Pierre Chambet. Data scientist and business engineer: forecasting, pricing and optimisation, from the first client meeting to the model in production." src="assets/banner-light.png">
</picture>

Data scientist who learned the business side. I find the account, ask who signs, scope and price the work, then build the model and run it with the people who use it. Diplôme d'Ingénieur from Télécom SudParis, double degree in data science with Télécom Paris (IP Paris). **Available January 2027, relocating to New York.**

## Track record

<table>
  <tr><td align="right"><b>€28,500</b></td><td>Data-science engagement with <b>Groupe Etam</b>, scoped and priced by me, signed <b>7 days</b> after the first meeting</td></tr>
  <tr><td align="right"><b>2</b></td><td>Tailored product demos to the operations-control teams of <b>SWISS</b> and <b>Finnair</b></td></tr>
  <tr><td align="right"><b>72</b></td><td>Named decision-makers mapped on the 63-airline target list I prospected for SmartFleetOptim</td></tr>
  <tr><td align="right"><b>158,455&nbsp;→&nbsp;39</b></td><td>Training providers filtered, researched and scored down to 39 personalised outbound sequences</td></tr>
  <tr><td align="right"><b>2nd</b></td><td>Overall at the <b>Airbus × IBM × AWS</b> hackathon, judged on the model and the business pitch</td></tr>
  <tr><td align="right"><b>1&nbsp;of&nbsp;5</b></td><td>Winning teams out of 23 at IP Paris Innov'Night: I led a team of strangers to the investor pitch</td></tr>
</table>

## Experience

**Groupe Etam** (Etam, Undiz, Maison 123) · independent data-science consultant · Oct – Dec 2026\
Met the group's Director of Data & AI, wrote a four-phase proposal with one deliverable per phase and set my own day rate. Accepted after the client's legal review: 57 days, €28,500, on site three days later. I run and improve the demand-forecasting and promotional-pricing models behind year-end markdowns and winter sales for three brands; every change is backtested before release, and the mission ends with a handover so the team runs January alone.

**[SmartFleetOptim](https://smartfleetoptim.com)** · founder and lead engineer, co-founded, sole founder since June 2026 · IMT Starter incubator\
A stress test that tells an airline which spare aircraft pay for themselves. Under the hood: a day-by-day Monte Carlo per base and sub-fleet (Poisson groundings, heavy-tailed durations), common random numbers so every plan faces the same seasons, and costs applied after simulation so the whole pricing debate can be swept without re-running. Each spare aircraft gets a business case as a distribution (P10, P50, P90) and a break-even. I prospected the airlines myself and ran the SWISS and Finnair demos; after Finnair's, I asked who owned the decision and wrote to their VP of Network Management the same day. No pilot signed yet.

**Air France** · Network, program regulation · Oct 2024 – Mar 2025\
Built the Python decision tool and Power BI dashboard that Network management used to allocate spare aircraft across long- and medium-haul. My supervisor's letter says it exceeded the initial ambitions.

**Outbound tests** · Jul – Sep 2026\
For a B2B compliance service run with a partner: cut France's register of 158,455 training providers to 1,195 accounts, had AI agents research 150 of them under written sourcing rules, scored them A to D and wrote 39 four-touch sequences. A second agent corrected 50 of 91 talking points before release. Before that, I cold-called 22 heating contractors in one week to test an offer: 19 picked up, every outcome logged.

## Case studies

Public data, one business question each. When the simple baseline wins, the write-up says so.

| Question | Finding |
|---|---|
| **Which customers are worth a marketing e-mail?**<br>[uplift-targeting](https://github.com/Pchambet/uplift-targeting) | All of them. Blanket sending earns $155 per 1,000 customers against $115 on average for the best targeting model, which loses in 48 of 50 out-of-sample splits. |
| **How much stock buys a 95% fill rate?**<br>[spare-parts-inventory](https://github.com/Pchambet/spare-parts-inventory) | The forecast with the best error score ties up 39% more stock than a LightGBM quantile model that forecasts the whole demand distribution. |
| **Where does a minute of turnaround buffer avoid the most delay?**<br>[delay-contagion](https://github.com/Pchambet/delay-contagion) | Placed by a scenario LP, it avoids 1.7× the delay of uniform padding on held-out days, across 7 million US flights. |
| **How much of a battery's arbitrage value can a forecast capture?**<br>[Helios-Quant-Core](https://github.com/Pchambet/Helios-Quant-Core) | 64% of perfect foresight in August 2022, at the height of the energy crisis, with model predictive control. |
| **Where does money leak between order, receipt and invoice?**<br>[consolidation-erp-mcp](https://github.com/Pchambet/consolidation-erp-mcp) | Thirteen SQL controls across Odoo, an accounting file and a warehouse API catch all 22 planted discrepancies, exposed to an AI agent through an MCP server. |
| **What does each imported product really cost?**<br>[freightsight-landed-cost](https://github.com/Pchambet/freightsight-landed-cost) | Freight, duty and fees split across invoice lines to the cent, with an Odoo connector. |
| **Can an agent do pre-accounting without touching the books?**<br>[fiduciaire-agent](https://github.com/Pchambet/fiduciaire-agent) | Rules book what they can, an agent classifies the rest, and a person approves every entry. |

Also: [AIRBUS-IBM-HACKATHON-2026](https://github.com/Pchambet/AIRBUS-IBM-HACKATHON-2026), [gridcast](https://github.com/Pchambet/gridcast), [Particle-Filter-Optimal-Transport](https://github.com/Pchambet/Particle-Filter-Optimal-Transport), [Deep-Learning-from-Scratch](https://github.com/Pchambet/Deep-Learning-from-Scratch). Small fixes merged upstream in [POT](https://github.com/PythonOT/POT/pull/798), [pytorch-grad-cam](https://github.com/jacobgil/pytorch-grad-cam/pull/577), [prince](https://github.com/MaxHalford/prince/pull/201) and [gradio](https://github.com/gradio-app/gradio/pull/12922).

## Toolbox

**Data science:** Python, SQL (DuckDB, PostgreSQL), scikit-learn, LightGBM, PyTorch; forecasting and pricing models, conformal prediction, Monte Carlo simulation, linear programming, model predictive control.\
**Engineering:** FastAPI, Docker, GitHub Actions, pytest, Claude Code and MCP servers.\
**Business:** discovery and qualification, proposal writing, day-rate pricing, account research, tailored demos, phone, e-mail and LinkedIn outreach.

---

Open to data science and business-engineering roles in New York and London from January 2027. [pierrechambet@gmail.com](mailto:pierrechambet@gmail.com) · [LinkedIn](https://www.linkedin.com/in/pierre-chambet/)

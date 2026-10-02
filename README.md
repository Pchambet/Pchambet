<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.png">
  <img alt="Pierre Chambet. Decisions for operations that run on uncertain data." src="assets/banner-light.png">
</picture>

I build decision tools for operations that run on uncertain data: airline fleets, freight, power grids. I forecast with honest uncertainty, simulate what can go wrong, optimise what can be controlled, and ship the result as software people use.

- **Founder and lead engineer, [SmartFleetOptim](https://smartfleetoptim.com/).** Stress-tests airline spare-fleet strategies across disruption, demand and delivery-delay scenarios. Technical sessions with the operations and data teams of Finnair, SWISS and Air Canada.
- **Air France Network, program regulation.** Built the Python decision-support tool and Power BI dashboard that Network management used to allocate spare aircraft across long- and medium-haul operations.
- **Airbus × IBM × AWS hackathon, machine learning lead.** 2nd overall. Adversarial validation exposed a train/test shift; calibrated probabilities took the team from 22nd on the public leaderboard to 6th on the private one.
- **Télécom SudParis** engineering degree (data analysis and pattern classification, 2026). Visiting research intern at **NAIST**, Japan, on optimal transport for machine learning.

## Flagship projects

| Project | The question | What the data says |
|---|---|---|
| [**delay-contagion**](https://github.com/Pchambet/delay-contagion) · [report](https://pchambet.github.io/delay-contagion/) | Where should an airline add turnaround buffer to stop delays spreading? | On 7M US flights, a buffer minute placed by a scenario LP avoids **1.7×** the delay of uniform padding on held-out days. dbt + DuckDB, hinge propagation model, HiGHS. |
| [**gridcast**](https://github.com/Pchambet/gridcast) · [report](https://pchambet.github.io/gridcast/) | Can a demand forecast publish uncertainty bands that stay honest through an energy crisis? | **80.0% / 95.0%** coverage out of sample on 38,732 hours of French demand, 2022–2026, with conformal recalibration; a frozen calibration is on target 12% of the time, rolling recalibration 50%. RTE stays more accurate on the point forecast, and the report says so. |
| [**uplift-targeting**](https://github.com/Pchambet/uplift-targeting) · [report](https://pchambet.github.io/uplift-targeting/) | Who should get the marketing e-mail? | On a 64k-customer randomised test: everyone. Uplift selection chosen out of sample loses to blanket sending in **48 of 50** splits; scored in sample it would have promised a gain. |
| [**spare-parts-inventory**](https://github.com/Pchambet/spare-parts-inventory) · [report](https://pchambet.github.io/spare-parts-inventory/) | How much stock buys a 95% fill rate when demand is mostly zeros? | The best forecast by MASE needs **39% more stock** than a LightGBM quantile model. Forecast the distribution, simulate the policy, then allocate the budget. |
| [**AIRBUS-IBM-HACKATHON-2026**](https://github.com/Pchambet/AIRBUS-IBM-HACKATHON-2026) · [report](https://pchambet.github.io/AIRBUS-IBM-HACKATHON-2026/) | Will a corrosion-risk model hold on aircraft it has never seen? | Adversarial validation (AUC 0.86) exposed the shift and set the one parameter that mattered: **22nd → 6th** from public to private leaderboard, 2nd overall. |
| [**Gait-Analysis**](https://github.com/Pchambet/Gait-Analysis) · [report](https://pchambet.github.io/Gait-Analysis/) | Does walking slowly make gait more individual? | No. One knee cycle identifies its owner 63% of the time at spontaneous speed and 51% at slow speed; variability rises at both levels. Rebuilding my own course project with grouped validation reversed its conclusion. |

## More work

**Products and data engineering.** [freightsight-landed-cost](https://github.com/Pchambet/freightsight-landed-cost) (landed cost per SKU for importers: two-pass Decimal engine, Postgres row-level security, Odoo connector), [consolidation-erp-mcp](https://github.com/Pchambet/consolidation-erp-mcp) (three ERPs reconciled in DuckDB, queried by an agent through an MCP server), [fiduciaire-agent](https://github.com/Pchambet/fiduciaire-agent) (Swiss QR-bills and bank statements: rules first, an agent only where no rule applies, a person approves).

**Optimisation and research.** [Helios-Quant-Core](https://github.com/Pchambet/Helios-Quant-Core) (walk-forward battery arbitrage with MPC and Wasserstein-robust optimisation), [Particle-Filter-Optimal-Transport](https://github.com/Pchambet/Particle-Filter-Optimal-Transport) (differentiable particle filtering through optimal-transport resampling, checked against exact Kalman gradients, with my NAIST notes), [functional-data-clustering](https://github.com/Pchambet/functional-data-clustering) (clustering curves and covariates together, in R).

**Statistical studies.** [Gait-Analysis](https://github.com/Pchambet/Gait-Analysis) (is gait more individual at slow speed? 2,544 knee cycles, grouped validation), [facebook100-social-structure](https://github.com/Pchambet/facebook100-social-structure) (homophily, link prediction and communities on 100 campus graphs), [hmm-from-scratch](https://github.com/Pchambet/hmm-from-scratch) (do hidden states earn their parameters?), [mushroom-project](https://github.com/Pchambet/mushroom-project) (what a correspondence analysis keeps and loses).

**Machine learning.** [NLP-from-scratch-to-BERT](https://github.com/Pchambet/NLP-from-scratch-to-BERT), [cnn-explainability-workshop](https://github.com/Pchambet/cnn-explainability-workshop), [mnist-case-study](https://github.com/Pchambet/mnist-case-study), [mnist-latent-space-ae-vae](https://github.com/Pchambet/mnist-latent-space-ae-vae), [MTL_Classification_Reconstruction](https://github.com/Pchambet/MTL_Classification_Reconstruction).

**Teaching.** [Deep-Learning-from-Scratch](https://github.com/Pchambet/Deep-Learning-from-Scratch): neural networks rebuilt in NumPy from a single neuron to any depth, every gradient derived by hand and checked numerically, published as an English series on LinkedIn.

## Open source

Merged upstream: [POT #798](https://github.com/PythonOT/POT/pull/798), [pytorch-grad-cam #577](https://github.com/jacobgil/pytorch-grad-cam/pull/577) and [#578](https://github.com/jacobgil/pytorch-grad-cam/pull/578), [prince #201](https://github.com/MaxHalford/prince/pull/201), [gradio #12922](https://github.com/gradio-app/gradio/pull/12922) and [#12923](https://github.com/gradio-app/gradio/pull/12923). Under review: [scikit-learn #33360](https://github.com/scikit-learn/scikit-learn/pull/33360), [datasets #8016](https://github.com/huggingface/datasets/pull/8016).

## Toolbox

- **Modelling:** scikit-learn, LightGBM, PyTorch, TensorFlow/Keras; conformal prediction, causal meta-learners, Bayesian filtering.
- **Optimisation:** linear programming (HiGHS), cvxpy, model predictive control, distributionally robust optimisation, optimal transport.
- **Data:** Python (pandas, NumPy, SciPy), SQL (DuckDB, PostgreSQL), dbt, R, Power BI.
- **Engineering:** FastAPI, React and TypeScript, Docker, GitHub Actions, uv, pytest, MCP servers.

---

[pchambet.github.io](https://pchambet.github.io) · [LinkedIn](https://www.linkedin.com/in/pierre-chambet/) · [pierrechambet@gmail.com](mailto:pierrechambet@gmail.com) · Paris, open to roles abroad

# Evidence sweep, intelligence, 2026-08-13

Delta Since Last Sweep:
- One frontier model shipped inside the nine-day window: SpaceXAI released Grok 4.6 on 12 Aug 2026, the first release since Claude Opus 5 (24 Jul 2026) to reach the top band of an aggregate intelligence index. It is the only capability event in the window.
- The unsaturated capability measure the last sweep tracked did not move. The ARC-AGI-3 model leaderboard still tops out at Claude Opus 5 at 30.2% as of its 13 Aug 2026 refresh, and Grok 4.6 does not appear on it at all.
- Both institutional mechanisms the last sweep flagged produced no public action in the window. A Federal Register full-text query for "covered frontier model" over documents published from 1 Aug 2026 returns zero results, and the Commission's AI Office page carries no dated item after 31 Jul 2026, so intelligence-2026-08-02 and intelligence-2026-08-04 remain untouched.
- New to this sweep, though dated 3 Aug 2026 and missed by the previous one: Epoch AI and METR refreshed the MirrorCode long-horizon coding leaderboard, showing a 44 point gap between the top two frontier models.

Confirmed Developments:
- SpaceXAI released Grok 4.6 on 12 Aug 2026 with a 500,000 token context window, a 1 Feb 2026 knowledge cutoff, text and image input, and pricing of $2 per million input tokens and $6 per million output tokens (doubling above a 200,000 token prompt), scoring 61 on the Artificial Analysis Intelligence Index, tying GPT-5.6 Sol at maximum reasoning and trailing Claude Fable 5 by one point (source: https://siliconangle.com/2026/08/12/spacexai-releases-flagship-grok-4-6-model-advanced-reasoning-capabilities/, Aug 2026) (source: https://www.marktechpost.com/2026/08/12/spacexai-releases-grok-4-6/, Aug 2026) (source: https://artificialanalysis.ai/models/grok-4-6, Aug 2026)
- The aggregate-index tie does not hold on agentic coding evaluations: Grok 4.6 (high) scores 26% on Terminal-Bench v3.0 against 34.6% for GPT-5.6 Sol Max and 34.1% for Claude Fable 5 Max, and 65.9% on DeepSWE v1.1 against 73% and 70% respectively, while leading on GDPVal-AA v2 (1753 against 1728 and 1741) (source: https://www.marktechpost.com/2026/08/12/spacexai-releases-grok-4-6/, Aug 2026) (source: https://explainx.ai/blog/spacexai-grok-4-6-launch-evals-cursor-august-2026, Aug 2026)

Emerging Signals:
- Frontier capability is being adjusted through safeguard tuning rather than model change: Anthropic reported on 7 Aug 2026 that a Claude Fable 5 biology-classifier update cut biology-related fallbacks to less capable models by about 85%, with per-surface fallback reductions of about 67% on Claude.ai, 55% on Cowork, 17% on Claude Code and 7% on Claude Platform (source: https://www.anthropic.com/news/improving-fable-5-s-biology-safeguards, Aug 2026)
- A joint Epoch AI and METR benchmark now reports a very wide frontier spread on long-horizon coding: the MirrorCode leaderboard refresh of 3 Aug 2026 places Claude Fable 5 at 64% and GPT-5.6 Sol at 20% on a task set where models reimplement entire programs end to end without access to the original source (source: https://epoch.ai/data/ai-benchmarking-dashboard, Aug 2026)
- ARC Prize's own leaderboard separates three measurement classes for ARC-AGI-3 (reasoning systems at multiple reasoning levels, base LLMs at single-shot inference, and Kaggle competition systems operating under a $50 compute budget), so "the ARC-AGI-3 leaderboard" names at least three different measurement bases rather than one (source: https://arcprize.org/leaderboard, Aug 2026)

Counter-Signals:
- The interactive benchmark the last sweep treated as the live capability frontier has been static across the window: the ARC-AGI-3 model leaderboard as of 13 Aug 2026 still reads Claude Opus 5 at 30.2%, GPT-5.6 Sol at 7.8%, Claude Opus 4.8 at 1.5% and every other tracked model at or below 0.8%, with no August model added (source: https://benchlm.ai/benchmarks/arcagi3, Aug 2026)
- Public autonomy-horizon measurement fell further behind release cadence rather than catching up: METR's time-horizon page is still dated 8 May 2026, still lists Claude Mythos Preview as its newest addition, and explicitly notes missing measurements for Claude Opus 4.7, Grok 4.3 and GPT-5.5, so the gap now spans at least six frontier releases (source: https://metr.org/time-horizons/, May 2026)

Regulatory Shifts:
- None

Capital Movements:
- None

Technical Changes:
- Aggregate intelligence indices resolve a new frontier model within a day while interactive and long-horizon benchmarks do not: Artificial Analysis lists Grok 4.6 (high) at index 61, ranked 6th of 184 models, with 65.5 output tokens per second and a cost of $0.84 per Intelligence Index task, on the day after release (source: https://artificialanalysis.ai/models/grok-4-6, Aug 2026)
- The top of the Artificial Analysis Intelligence Index is compressed into a three point band: Claude Opus 5 (max and xhigh) at 63, Claude Fable 5 (with fallback) at 62, then Claude Opus 5 (high), GPT-5.6 Sol (max) and Grok 4.6 (high) all at 61, with Kimi K3 (max) at 60 and Qwen3.8 Max at 58 (source: https://artificialanalysis.ai/leaderboards/models, Aug 2026)

Contradictions:
- The same three models are ranked identical by aggregate index and eight points apart on Terminal-Bench v3.0, so "frontier parity" in this window is an artifact of which measure is quoted rather than a property of the models.
- The one interactive capability measure that is not saturated did not evaluate the window's only new frontier model, while the aggregate indices that are compressed into a three point band evaluated it within a day, so measurement effort is concentrated where discrimination is weakest.
- Capability was expanded in the window by loosening a safety classifier rather than by shipping a stronger model, which means a lab-side configuration change and a model release are now observationally similar from the user side but only one of them is measured by any public benchmark.

Ledger Candidates:
- ARC Prize publishes an ARC-AGI-3 result for a SpaceXAI Grok-family model first released on or after 2026-08-12, on its verified leaderboard at arcprize.org (reasoning-systems track), by 2027-01. Resolve by 2027-01. (motivated by: https://benchlm.ai/benchmarks/arcagi3, Aug 2026)
- Artificial Analysis reports an Intelligence Index score of 64 or higher for at least one model on artificialanalysis.ai/leaderboards/models, in any reasoning configuration, by 2027-01. The verified maximum on 2026-08-13 is 63 (Claude Opus 5, max and xhigh). Resolve by 2027-01. (motivated by: https://artificialanalysis.ai/leaderboards/models, Aug 2026)
- METR publishes an updated task-completion time-horizon measurement at metr.org/time-horizons/ that includes at least one model first released on or after 2026-06-01, by 2027-02. The page has been dated 8 May 2026 since before the June and July 2026 model wave. Resolve by 2027-02. (motivated by: https://metr.org/time-horizons/, May 2026)

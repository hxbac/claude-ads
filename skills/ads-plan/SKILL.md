---
name: ads-plan
description: "Create a professional paid-advertising strategy covering objectives, economics, platform selection, campaign architecture, audiences, budget, creative, measurement, experiments, governance, rollout, and reporting. Use for ad plan, media plan, PPC strategy, paid-social strategy, campaign architecture, advertising roadmap, or channel planning. Also use when the request is written in Vietnamese, for example \"lên kế hoạch quảng cáo\", \"kế hoạch quảng cáo Facebook\", \"kế hoạch truyền thông trả phí\", \"chiến lược quảng cáo cho shop mỹ phẩm\"."
---

# Paid Media Plan

1. Read the setup profile, business economics, evidence, current account state, and
   relevant industry template as optional input.
2. Define objective, customer, offer, conversion, value, constraints, geography,
   regulated category, time horizon, and success criteria.
3. Evaluate channel roles and exclusions from first principles; do not require every
   supported platform. For a channel outside the twelve-platform contract, load
   `ads/references/additional-platforms.md` and return a research lead unless
   its current buying, eligibility, measurement, and creative evidence is present.
4. Before proposing Meta budgets, learning-phase expectations, bidding,
   consolidation, or performance forecasts, collect the account, Pixel, and
   conversion cold-start dimensions per the contract in
   `skills/ads-meta/SKILL.md`. When any dimension is cold or `unknown`, plan
   for measurement validation, explicit creative hypotheses, staged reversible
   tests, and confidence labels; do not apply mature-account benchmarks to
   missing history.
5. Specify campaign architecture, audience strategy, creative system, budget and
   pacing, measurement, experiments, policy controls, and operating cadence.
6. Phase prerequisites before launch, learning, optimization, and scale.
7. Assign every action an owner, timing, dependency, guardrail, evidence, success
   measure, and rollback or exit condition.
8. Return canonical JSON and render the requested human plan.

Vietnam default: when the request is in Vietnamese or names Vietnam, plan in VND,
for location Vietnam, and write the plan in Vietnamese, unless the operator says
otherwise. Load `ads/references/vietnam-market.md` and
`ads/references/vietnam-ad-compliance.md`. If the product is cosmetics,
functional food, a health service, medicine, education, real estate or finance,
put the content pre-approval requirement at the top of the plan before any
budget or channel. Market figures are illustrative until the operator supplies
an export.

A plan is advisory. It becomes an account change only through launch or optimize
mutation gates.

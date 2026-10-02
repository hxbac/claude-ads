# Vietnam market reference

Load when the request is in Vietnamese, names Vietnam as the geography, or
the account bills in VND. Defaults: currency VND, location Vietnam, language
Vietnamese (see `skills/ads-plan`, `ads-budget`, `ads-create`, `ads-math`).

Rules for this file:

- Every number below is **illustrative**, taken from a secondary source on the
  date shown. It is a starting hypothesis, never a benchmark to score an
  account against and never a promise. Replace it with the operator's own
  export as soon as one exists.
- Format per number: value, source, retrieved date. Retrieved 2026-10-02.
- Legal and tax statements are marked "verify against primary source". The
  compliance detail lives in `vietnam-ad-compliance.md`.

## Platform mix by goal (hypotheses, not rules)

| Goal | First platforms to consider | Why (hypothesis) |
| --- | --- | --- |
| Local shop, offline store, service | Meta (Facebook/Instagram), Zalo Ads, Google Search | Local reach, messaging as the conversion |
| Online store with its own site | Meta, Google Search and Shopping, TikTok | Prospecting plus capture |
| Marketplace seller | Shopee Ads, TikTok Shop GMV Max, Lazada Sponsored | Conversion happens inside the marketplace |
| Lead generation (education, real estate, finance) | Meta lead forms, Zalo Form Ads, Google Search | Phone number is the lead; check regulated-category rules first |
| Brand awareness | TikTok, YouTube, Meta video | Short video reach |

Budget bands in VND per month (all illustrative, an operator judgement, no
source): under 10 million VND, run one platform only and learn; 10 to 30 million
VND, one prospecting platform plus a small retargeting or search share; above
30 million VND, add a second platform only after the first has a stable
cost per result. Minimum evidence before moving money: follow
`budget-allocation.md` and `bidding-strategies.md`; do not shortcut it for a
small budget.

Exchange-rate note: platforms bill in the account currency. Confirm whether the
account is VND or USD before comparing a CPA to a margin; a USD account adds
rate movement to every number.

## Zalo Ads

Source: Zalo Ads, "Các hình thức quảng cáo trên Zalo Ads"
(https://ads.zalo.me/business/cac-hinh-thuc-quang-cao-tren-zalo-ads/),
retrieved 2026-10-02. Formats and billing models change; re-check in the Zalo
Ads console before planning.

Formats listed by Zalo on that page: Official Account Ads (grow followers;
CPC or CPF), Website Ads (traffic; CPC), Video Ads (CPM), Article Ads
(promote OA articles; CPC), Form Ads (lead capture; limited to approved
industries), Message Ads (1:1 chat; CPC or CPA), Display Ads (Báo Mới, Zing
MP3 and the Zalo app; CPM, CPC for Medium Rectangle), Commerce Ads (physical
products only, no services or digital goods; CPC or CPA).

- Official Account (OA): a verified OA is the base for most formats and for
  free retargeting of followers. A business OA needs a Vietnamese business
  registration (secondary source: https://prodima.vn/en/what-is-zalo/ and
  https://adszalo.hateblo.jp/entry/2025/04/16/230437, retrieved 2026-10-02;
  verify against the Zalo OA registration page).
- Targeting: secondary sources report demographic, location and device
  targeting plus uploaded phone-number audiences, and no interest targeting
  comparable to Meta (https://vietnam-agent.com/zalo-ads-vs-google-ads-where-to-get-the-most-roi/,
  retrieved 2026-10-02, **verify in the console**).
- Zalo has no public read API an ad skill can rely on. Audits run from console
  exports the operator supplies.

## Marketplace and commerce ads

Sources retrieved 2026-10-02; all are secondary and vendor or agency content:
https://www.feedforce.vn/articles/shopee-ads-vietnam-2026,
https://www.uncommonengine.com/compare/shopee-tiktok-lazada-ads-budget-mechanics/,
https://vnmarketinsights.com/compare/shopee-vs-lazada-vs-tiktok-shop/.

- **Shopee Ads**: in-marketplace ads (search and discovery placements, GMV
  Max automation, Live display ads). Illustrative market context: one report
  puts Shopee at 54.5 percent and TikTok Shop at 43.4 percent of tracked
  Vietnam marketplace GMV (https://vietnamnews.vn/economy/1800588/vietnamese-consumers-spread-shopping-across-multiple-peak-season-events.html,
  retrieved 2026-10-02; the period is not confirmed, treat as a hypothesis).
- **Lazada Sponsored Solutions**: Sponsored Discovery and the newer Sponsored
  Max were reported to run in parallel during a transition (secondary source
  above, verify in Seller Center).
- **TikTok Shop Ads**: reported to be GMV Max only since July 2025 (manual
  keyword bidding removed), bidding against a target ROI. **Verify in TikTok
  Seller Center.**
- These platforms report their own attributed sales. Do not add them to Meta or
  Google conversions (see `skills/ads-attribution`).
- Marketplace ad skills in this repo are not platform audits: there is no
  Shopee, Lazada or TikTok Shop audit reference. Return research leads and
  operator-export analysis, per `additional-platforms.md`.

## Cốc Cốc

Cốc Cốc is a Vietnamese browser and search engine with its own ad platform
(https://press.coccoc.com, retrieved 2026-10-02). Agency sources claim a
meaningful share of local search and cheap clicks (5,000 to 15,000 VND per
click, https://dps.media/coc-coc-ads-la-gi-bang-gia-quang-cao-coc-coc-cap-nhat-2025/,
retrieved 2026-10-02). These are vendor-side claims, illustrative only. Treat
as a test channel for Vietnamese-language search with a small cap. The ad
platform can import Google Ads search campaigns; verify the import behaviour on
the Cốc Cốc press page before relying on it.

## Seasonality

Source for the shopping calendar: Janio, "When do Vietnam's top eCommerce
shopping events take place?" (https://www.janio.asia/resources/articles/major-e-commerce-shopping-events-vietnam),
retrieved 2026-10-02.

- Marketplace double-date sales: 9.9, 10.10, 11.11, 12.12. Black Friday late
  November. Tết Nguyên Đán (date moves each year, usually late January or
  February): shopping peaks in the weeks before, then activity pauses for
  roughly a week or more around the holiday. Confirm the date from the
  official calendar each year.
- Planning consequences (hypotheses): auction cost rises in the days before a
  mega sale; budget caps and creative should be ready a week early; do not
  judge a learning-phase campaign on mega-sale days; schedule delivery and
  customer-service capacity around the Tết pause; do not launch a new
  campaign in the days around Tết.
- No CPM uplift figure is given here because no reliable source was found
  (2026-10-02). Use the account's own history.

## Cash on delivery (COD) and measurement

Illustrative: secondary sources put COD at about 67 percent of Vietnam
e-commerce transactions in 2024 and 2025 (https://tgmresearch.com/vietnam-ecommerce-payment-shift-2025.html,
retrieved 2026-10-02; methodology not verified).

- A platform "purchase" event fired at order placement counts orders that are
  later refused, unreachable or returned. With COD the gap can be large.
- Measure at least three tiers: order placed, order confirmed by phone/OA
  message, order delivered and paid. Break-even ROAS and CPA must use the
  delivered-and-paid rate (see `skills/ads-math`; never fabricate the rate,
  ask for it).
- Prefer sending the confirmed or delivered status back as an offline or
  server-side conversion (`conversion-tracking.md`, `skills/ads-server-side-tracking`)
  over optimizing on raw order placed.
- Ask the operator for the cancel/return rate per channel; do not assume one.

## VAT and invoices

Illustrative and **verify against primary source** (Ministry of Finance or a
tax adviser): secondary sources report that Google, Meta and TikTok register and
pay tax in Vietnam directly under Circular 80/2021/TT-BTC, so the advertiser
does not withhold foreign contractor tax for them, and that the VAT rate on
these services rose from 5 to 10 percent from 2025-07-01
(https://blog.gudjob.net/noi-tiep-google-meta-va-tiktok-ap-dung-thue-suat-10-cho-cac-dich-vu-quang-cao-tai-viet-nam-tu-01-07-2025/,
https://thuvienphapluat.vn/phap-luat/thue-nha-thau-lien-quan-den-chi-phi-dang-quang-cao-tren-facebook-google-hien-nay-duoc-quy-dinh-the--420012-22125.html,
retrieved 2026-10-02). Whether a platform statement is a deductible VAT invoice
for the business is an accountant's call. In budget math, say whether the
spend figure includes VAT, and keep the choice consistent.

## What not to assume

- No Vietnamese CPC, CPM, CVR or ROAS benchmark is published here: none was
  found from a source with a stated method. Ask for the operator's export.
- Interest and audience names on Meta and TikTok are localized and change;
  check the live ad manager.

# Vietnamese ad copy reference

Load with `skills/ads-create` and `skills/ads-creative` when the copy is
Vietnamese. Limits below are **illustrative**, from commonly published platform
specifications as of 2026-10-02. Platforms change them; confirm in the ad
manager preview before locking copy. `meta-creative-specs.md`,
`google-creative-specs.md` and `tiktok-creative-specs.md` stay the primary
specification references in this repo.

## Counting characters with diacritics

- Count what the platform counts: characters (Unicode code points), not bytes
  and not syllables. Normalize the text to NFC first. A letter such as
  "e with circumflex and acute" is one character in NFC and two in NFD; pasting
  from some tools gives NFD and can break a limit that looked safe.
- Vietnamese words are short syllables separated by spaces, and diacritic
  letters count the same as plain ones. Vietnamese copy usually runs longer
  than the English original (often by a third or more, an observation, not a
  measured figure). Draft in Vietnamese, do not translate then trim.
- Illustrative limits (verify per placement): Google responsive search ad
  headline 30 characters and description 90; Meta primary text is cut after
  roughly 125 characters in feed, headline around 40; TikTok ad text up to
  100 characters. Check preview truncation on mobile; many Vietnamese users
  see only the first line.
- Zalo Ads limits: not sourced. Read them from the Zalo Ads console.

## Register (xưng hô)

Pick one register per ad set and keep it identical to the landing page and the
Zalo OA or chat replies. A mismatch is a quality defect.

| Register | Use for | Notes |
| --- | --- | --- |
| bạn / mình | Peer voice, young audience, fashion, apps, F&B | Warm, short |
| anh / chị | Polite, service businesses, mixed age audience | Safe default for an unknown audience |
| quý khách / quý vị | Formal, finance, medical, B2B, premium | Longer, stiffer |

Do not mix registers in one ad. Do not use "em" for the brand talking to a
customer unless the brand voice already does. If the landing page register is
unknown, ask once or default to "anh/chi" and say so.

## Hooks that fit Vietnamese buyers (hypotheses to test)

Hypotheses, not findings; test each against the account's own data
(`ads-test`).

- Price and bundle: the actual price or saving in VND ("Chỉ từ 199.000đ").
- Social proof with a number the brand can document ("Hơn 2.000 khách đã dùng").
- Local trust: free inspection on delivery, COD, exchange policy, warranty
  (COD is common, see `vietnam-market.md`), shop address and hotline.
- Question about the pain point in the first line.
- Seasonal: Tết, 9.9 to 12.12, back to school, with a real end date.
- Messaging as the action: "Nhắn tin để nhận tư vấn" for Meta Messenger, Zalo.

## Call-to-action verbs

Mua ngay, Đặt hàng, Đặt lịch, Nhắn tin, Nhận tư vấn, Đăng ký, Xem thêm, Nhận
ưu đãi, Gọi ngay. Match the verb to the action the platform button and the
landing page really offer. Use a real phone number or OA link, never a fake
countdown.

## Compliance before style

If the product is cosmetics, functional food, a health service, education, real
estate or finance, apply `vietnam-ad-compliance.md` first: required statements
(for example a functional food disclaimer), banned claims, and pre-approval.
Compliance text counts against the character limits, so plan room for it.

## AI-tell phrases

Vietnamese machine-written copy has recognizable stock phrases. The hub keeps
the scored list in `claude-blog/scripts/vi_profile.py` (a sibling checkout in
the hub; reference it, do not copy it here). When present, avoid the PHRASE and
TRIGGER tier items in ad copy too. Without the file, apply the same idea:
remove generic openers, filler intensifiers and empty superlatives, and replace
each with a concrete fact, number or action. Blog gates and scores do not apply
to ad copy; this is a manual style check only.

## Output pattern

For each concept: the register chosen, headline and text variants with their
character counts, the CTA, the product-category compliance note, and which
claims need a document from the operator. Mark every limit as "verify in
preview".

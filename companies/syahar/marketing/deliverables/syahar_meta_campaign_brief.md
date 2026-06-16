# Syahar Meta Ads Campaign Brief — UK & Gulf Corridors (A/B Test)

**Issue:** SYA-29 | **Budget:** NPR 5,000/mo | **Period:** Ongoing from launch

---

## 1. Business Manager Setup

### Step-by-step (Business Manager)
1. Go to [business.facebook.com](https://business.facebook.com) → Create Account
2. Business Name: **Syahar Remittance Pvt Ltd**
3. Add Ad Account: Currency **USD** (Meta does not support NPR billing; fund via card/NPR equivalent)
4. Connect Instagram account: **@syahar_official** (or create one)
5. Create Facebook Page: **Syahar – पैसा पठाउनुस् सजिलोसँग**
6. Enable **Lead Ads** form or connect Pixel to `syahar.com`

---

## 2. Campaign Structure

```
Campaign: SYAHAR_NRN_ABTEST_2026Q2
  Objective: Traffic / Lead Generation
  A/B Test: ON (Ad A vs Ad B)

  ├── AdSet_UK      (United Kingdom)
  ├── AdSet_UAE     (United Arab Emirates)
  ├── AdSet_Qatar   (Qatar)
  ├── AdSet_Kuwait  (Kuwait)
  ├── AdSet_AUS     (Australia)
  └── AdSet_KOR     (South Korea)
```

---

## 3. Targeting Specifications (All Ad Sets)

| Parameter | Value |
|-----------|-------|
| Language | Nepali |
| Age | 22–50 |
| Gender | All |
| Placement | Facebook Feed (60%) + Instagram Feed + Reels (40%) |

### Interest Targeting (Detailed)
- Non-Resident Nepali (NRN) Association
- Nepal Money Transfer / Remittance
- IME Remittance, Prabhu Money Transfer, Western Union
- eSewa, Khalti
- Nepal, Nepali language, Himalayan Bank
- Dashain, Nepali community abroad

### Location + Estimated Nepali Diaspora
| Ad Set | Country | Est. NRN Population |
|--------|---------|---------------------|
| AdSet_UK | United Kingdom | ~90,000 |
| AdSet_UAE | United Arab Emirates | ~170,000 |
| AdSet_Qatar | Qatar | ~130,000 |
| AdSet_Kuwait | Kuwait | ~50,000 |
| AdSet_AUS | Australia | ~30,000 |
| AdSet_KOR | South Korea | ~20,000 |

---

## 4. Budget Allocation

**Total:** NPR 5,000/month (~USD 37/mo at NPR 135/USD)

| Placement | % | NPR/mo | NPR/day |
|-----------|---|--------|---------|
| Facebook Feed | 60% | 3,000 | 100 |
| Instagram + Reels | 40% | 2,000 | 67 |

**Per Corridor (suggested split):**
| Corridor | % of Budget | NPR/mo |
|----------|-------------|--------|
| UK | 30% | 1,500 |
| UAE | 25% | 1,250 |
| Qatar | 15% | 750 |
| Kuwait | 10% | 500 |
| AUS | 12% | 600 |
| KOR | 8% | 400 |

---

## 5. Ad Creatives

### AD A — Emotional Creative

**Format:** Video (15–30s) or carousel with family imagery

**Headline (Nepali):**
> घरमा पैसा पठाउनु छ? Syahar ले सजिलो बनाउँछ।

**English translation:** Need to send money home? Syahar makes it easy.

**Body Text (Nepali):**
> UK बाट नेपाल पैसा पठाउँदा, Syahar ले सबैभन्दा राम्रो दर दिन्छ। तपाईंको परिवारलाई छिटो, सुरक्षित र सस्तो तरिकाले पैसा पठाउनुस् — जुनसुकै बेला, जहाँबाट पनि।

**English translation:** When sending money from UK to Nepal, Syahar gives you the best exchange rate. Send money to your family quickly, safely, and at low cost — anytime, from anywhere.

**CTA Button:** अहिले पठाउनुस् *(Send Now)*

**Visual brief:** Show warm family scene (video call, festival preparation, children receiving money). End card shows Syahar logo + tagline.

---

### AD B — Rational Creative

**Format:** Static image or short video with rate comparison table

**Headline (Nepali):**
> UK→नेपाल: सबैभन्दा कम शुल्क, सबैभन्दा राम्रो दर

**English translation:** UK→Nepal: Lowest fees, best exchange rate

**Body Text (Nepali):**
> ✓ पहिलो ट्रान्सफरमा ०% शुल्क
> ✓ Real-time विनिमय दर
> ✓ मिनेटमा नेपाल पुग्छ
> ✓ Bank • eSewa • Khalti मा receive गर्नुस्
> ✓ IME र Western Union भन्दा सस्तो

**English translation:**
> ✓ 0% fee on first transfer
> ✓ Real-time exchange rate
> ✓ Arrives in Nepal in minutes
> ✓ Receive via Bank • eSewa • Khalti
> ✓ Cheaper than IME and Western Union

**CTA Button:** अहिले तुलना गर्नुस् *(Compare Now)*

**Visual brief:** Clean infographic showing side-by-side rate comparison (Syahar vs IME vs WU). Syahar highlighted as winner. Syahar brand colors.

---

## 6. UTM Tracking Parameters

**Base URL:** `https://syahar.com` (replace with actual landing page)

### UTM Schema
```
utm_source = facebook | instagram
utm_medium = paid_social
utm_campaign = syahar_nrn_{corridor}_abtest_2026q2
utm_content = ad_a_emotional | ad_b_rational
utm_term = {corridor}_nepali_remittance
```

### Complete UTM URL Matrix

| Corridor | Ad A URL | Ad B URL |
|----------|----------|----------|
| UK | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_uk_abtest_2026q2&utm_content=ad_a_emotional&utm_term=uk_nepali_remittance` | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_uk_abtest_2026q2&utm_content=ad_b_rational&utm_term=uk_nepali_remittance` |
| UAE | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_uae_abtest_2026q2&utm_content=ad_a_emotional&utm_term=uae_nepali_remittance` | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_uae_abtest_2026q2&utm_content=ad_b_rational&utm_term=uae_nepali_remittance` |
| Qatar | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_qatar_abtest_2026q2&utm_content=ad_a_emotional&utm_term=qatar_nepali_remittance` | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_qatar_abtest_2026q2&utm_content=ad_b_rational&utm_term=qatar_nepali_remittance` |
| Kuwait | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_kuwait_abtest_2026q2&utm_content=ad_a_emotional&utm_term=kuwait_nepali_remittance` | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_kuwait_abtest_2026q2&utm_content=ad_b_rational&utm_term=kuwait_nepali_remittance` |
| AUS | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_aus_abtest_2026q2&utm_content=ad_a_emotional&utm_term=aus_nepali_remittance` | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_aus_abtest_2026q2&utm_content=ad_b_rational&utm_term=aus_nepali_remittance` |
| KOR | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_kor_abtest_2026q2&utm_content=ad_a_emotional&utm_term=kor_nepali_remittance` | `https://syahar.com/?utm_source=facebook&utm_medium=paid_social&utm_campaign=syahar_nrn_kor_abtest_2026q2&utm_content=ad_b_rational&utm_term=kor_nepali_remittance` |

**Pixel Setup:** Install Meta Pixel on `syahar.com` → track `PageView`, `Lead`, `CompleteRegistration` events.

---

## 7. KPI Benchmarks & Tracking

| Metric | Target | How Measured |
|--------|--------|--------------|
| CPM | ≤ NPR 800 (~$5.90) | Meta Ads Manager → Campaign Reports |
| CTR | ≥ 1.5% | Meta Ads Manager → Ad-level breakdown |
| CPL | ≤ NPR 500 (~$3.70) | Meta Pixel lead event / form submission |
| CPC | ≤ NPR 30 | Ad Manager breakdown |
| ROAS | Track only (week 2+) | Pixel purchase events |

**Corridor breakdown:** Use Meta's Breakdown → Delivery → Country to segment CPM/CTR/CPL per corridor.

---

## 8. A/B Test Setup in Ads Manager

1. At Campaign level → toggle **A/B Test ON**
2. Variable: **Creative** (Ad A vs Ad B)
3. Test duration: **7 days minimum** (Meta recommends 14 days for statistical significance)
4. Winner metric: **Cost per Result** (Lead / Link Click)
5. Auto-apply winner: ON (optional)

---

## 9. Launch Checklist

- [ ] Business Manager account created for Syahar
- [ ] Facebook Page created/connected
- [ ] Instagram account connected
- [ ] Ad account funded (min. USD 30 to cover first 7 days)
- [ ] Meta Pixel installed on syahar.com
- [ ] Campaign SYAHAR_NRN_ABTEST_2026Q2 created
- [ ] 6 ad sets created (UK, UAE, Qatar, Kuwait, AUS, KOR)
- [ ] Ad A uploaded with Nepali copy + emotional creative
- [ ] Ad B uploaded with Nepali copy + rational creative
- [ ] UTM URLs entered per ad per corridor
- [ ] Campaign reviewed + submitted for Meta review
- [ ] Confirmation screenshot taken after ads go live
- [ ] 7-day performance report pulled and posted to [SYA-29](/SYA/issues/SYA-29)

---

## 10. 7-Day Report Template (Post Launch)

| Corridor | Ad | Impressions | CPM (NPR) | CTR | Clicks | CPL (NPR) |
|----------|----|-------------|-----------|-----|--------|-----------|
| UK | A — Emotional | | | | | |
| UK | B — Rational | | | | | |
| UAE | A — Emotional | | | | | |
| UAE | B — Rational | | | | | |
| Qatar | A — Emotional | | | | | |
| Qatar | B — Rational | | | | | |
| Kuwait | A — Emotional | | | | | |
| Kuwait | B — Rational | | | | | |
| AUS | A — Emotional | | | | | |
| AUS | B — Rational | | | | | |
| KOR | A — Emotional | | | | | |
| KOR | B — Rational | | | | | |

**Winner determination:** Whichever ad achieves lower CPL with CTR ≥ 1.5% wins. Scale winner budget by 2x in month 2.

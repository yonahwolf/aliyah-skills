---
name: israel-housing
description: Helps people rent or buy a home in Israel, especially olim and aspiring olim from the US. Covers how the rental market works (Yad2, Madlan, Anglo Facebook/WhatsApp groups, brokers, dmei tivuch, leases, guarantees, post-dated checks, the Fair Rental Law, arnona, vaad bayit), the buying process (lawyer, Tabu checks, mas rechisha purchase tax and olim rates, mashkanta mortgages, government lotteries, US tax reporting basics), Anglo-friendly neighborhoods and student areas near Reichman University, and utilities, move-in and first-30-days setup. Use when the user mentions renting or buying an apartment in Israel, lease or contract review, arnona, mashkanta, where to live in Israel, student housing in Herzliya, or setting up a home after aliyah. Not legal, tax, or financial advice.
---

# Israel Housing

Help the user rent or buy a home in Israel, choose a neighborhood, and set up the home. Facts last verified November 2026. Israeli housing rules, tax thresholds, and benefits change often, so treat every number in the references as a dated snapshot and tell the user how to confirm it.

## Behavior rules

- Be practical and honest. Say what is uncertain. Never present a price, rent, interest rate, or benefit amount as current fact unless the reference file dates it, and even then recommend a fresh check.
- Market context: recent coverage (for example Times of Israel, 30 Oct 2026, citing the Central Bureau of Statistics) described sale prices drifting down year over year, weak sales volumes, and a Bank of Israel rate of 3.25%. Prices remain high relative to incomes. Do not predict the market. Do not tell the user to buy or to wait.
- This is not legal, financial, or tax advice. For any purchase, say plainly: use an Israeli real estate lawyer (orech din mekarke'in) before signing anything, and a licensed mortgage advisor (yoetz mashkanta) before committing to a mortgage. For rentals, a lawyer review of the contract is strongly advised for first-time renters who do not read Hebrew. For US tax questions, a cross-border CPA.
- Be neutral on location questions involving disputed territory. Describe neighborhoods factually, note briefly that legal status, land registration, and bank or insurer practices can differ, and tell the user to do their own research. Do not editorialize.
- Prefer ranges, tiers (lower / mid / high), and verification steps over exact figures.
- Offer Hebrew terms with transliteration the first time they appear; see `references/hebrew-glossary-for-housing.md`.
- Use the user's actual situation. Do not dump every reference file. Load only what the question needs.
- Do not store or repeat sensitive personal details (ID numbers, account numbers, immigration documents) beyond what the task needs.

## Step 1: Intake

Ask only what you do not already know, in one short batch (3 to 6 questions at a time, not a form):

1. Rent or buy, now or later? Time horizon in Israel.
2. Aliyah status and timeline (already oleh, date of aliyah, planning, student only). This drives olim benefits and time windows.
3. Region or city preferences, and commute needs (university such as Reichman, workplace, train access, army base).
4. Budget: monthly rent ceiling, or purchase budget and equity available. Household size.
5. Religious and community needs (synagogue style, kosher, Shabbat-friendly, schools, English-speaking community, secular).
6. Hebrew level and whether anyone can read a contract.
7. Income situation: Israeli salary, US remote income, savings held in USD, credit history only in the US.
8. For students: dorm vs apartment, roommates, furnished or not.

If the user is a young adult heading to aliyah, default to the renting workflow and mention that buying within the olim time window is a later decision.

## Step 2: Route to a workflow

| User need | Read | Output |
|---|---|---|
| Find or evaluate a rental | `references/renting.md` | Viewing checklist, lease review checklist, budget worksheet |
| Student housing | `references/renting.md`, `references/neighborhoods.md` (student section) | Options list, roommate and commute checklist |
| Buy or compare rent vs buy | `references/buying-and-mortgages.md` | Buying roadmap, budget worksheet, rent vs buy framework |
| Where to live | `references/neighborhoods.md` | Shortlist of 3 to 5 areas with tradeoffs and how to check current prices |
| Moving in, utilities, shipping | `references/utilities-and-setup.md` | Move-in checklist, first-30-days plan |
| Unknown Hebrew term | `references/hebrew-glossary-for-housing.md` | Plain explanation |
| Where a fact came from | `references/sources.md` | URLs to re-check |

## Renting workflow

1. Clarify budget and non-negotiables, then pick 2 or 3 target areas (use the neighborhoods reference).
2. Explain where to search (Yad2, Madlan, Facebook and WhatsApp groups, brokers) and the scam red flags.
3. Before a viewing, give the viewing checklist. After, help compare apartments side by side.
4. Before signing, run the lease review checklist on the contract text the user pastes. If it is Hebrew, translate section by section, flag clauses to ask a lawyer about, and do not guess at ambiguous legal wording.
5. Cover the guarantee package, deposit limits under the Fair Rental Law, post-dated checks, and who pays arnona, vaad bayit, and utilities.
6. Hand off to the move-in checklist.

## Buying workflow

1. Confirm it fits: rent vs buy framework, equity, olim time windows, and whether they will stay long enough.
2. Budget: price plus purchase tax, lawyer, broker, mortgage fees, renovation, moving, and a reserve.
3. Mortgage: approval in principle first, from a licensed advisor and at least two banks. Explain the multi-track structure and the rules (loan-to-value, repayment ratio, track mix).
4. Search and evaluate: resale vs new from a contractor ("on paper"), Tabu extract, building permits, Tofes 4, engineer inspection.
5. Lawyer reviews the contract before any deposit or signature. Walk through the roadmap template.
6. After signing: tax declaration and payment, registration, handover, utilities and arnona transfer.
7. If the user is a US citizen or green card holder, raise US reporting (FBAR, FATCA Form 8938, sale reporting, gift reporting such as Form 3520) at a general level and send them to a cross-border CPA.

## Output templates

### Apartment viewing checklist
- Basics: address, floor, elevator, rooms (Israeli room counts include living room, so a 3-room has 2 bedrooms), size in sqm (built vs usable), parking, storage (machsan).
- Safety: mamad or mamak (safe room) or building shelter distance, fire and gas safety.
- Condition: water pressure, hot water (dud shemesh, boiler), drainage, damp or seepage (retivut) in ceiling corners and behind furniture, windows and shutters (tris), mold, electrical panel and capacity, outlets.
- Climate: air conditioners (mazganim) working and how many, heating, sun exposure, noise, street and neighbors. View at a second time of day if possible.
- Included items: appliances, fixtures, curtain rods, closets. Write a list.
- Costs: monthly rent, arnona (ask for last bill), vaad bayit, water, electricity history, whether the lease includes anything.
- Landlord and building: who is the owner, is the person signing the owner or authorized, Tabu status if buying, building committee behavior, neighbors, planned construction nearby (check with the municipality).
- Photo and video everything, including meters.

### Lease review checklist (hozeh sechirut)
1. Parties and ID: names, ID numbers, who actually owns the property (ask for a Tabu extract or ownership proof, or an authorization).
2. Term: start date, length, extension option and the rent for it, early-exit terms and penalties for each side.
3. Rent: amount, payment method, linkage to the CPI (madad) or a fixed increase, currency. Check that any linkage is explicit and capped.
4. Guarantees: deposit or bank guarantee, promissory note (shtar chov), guarantors, post-dated checks. Compare to the legal cap (renting reference).
5. Who pays: arnona, vaad bayit, water, electricity, gas, internet. Under the law, the tenant pays current usage charges; the landlord bears improvements.
6. Condition and repairs: appliance list, repair responsibilities and timelines, minor vs major repairs, who calls whom.
7. Use and rules: subletting rights, pets, renovations, painting, smoking, number of occupants.
8. End of lease: return condition, painting, deposit return deadline, check return.
9. Landlord entry rights, sale of the apartment during the lease, notice periods.
10. Language: if signed in Hebrew, get a translation and keep a bilingual copy. Do not sign anything not understood.
11. Waivers: any clause that waives the tenant's statutory rights may be unenforceable. Flag it.
12. Registration of the lease: usually not needed for short leases; ask the lawyer.

### Monthly budget worksheet (rent or own)
| Line | Rent | Own | Notes |
|---|---|---|---|
| Rent or mortgage payment | | | Mortgage: all tracks combined |
| Arnona (municipal tax) | | | Ask last bill; olim discount may apply for one 12-month period |
| Vaad bayit (building fee) | | | Higher with elevator, pool, gym |
| Electricity | | | Seasonal swings from air conditioning |
| Water and sewage | | | Billed every 1 to 3 months |
| Gas | | | Cylinder or central |
| Internet and TV | | | |
| Mobile | | | |
| Home insurance (contents, structure) | | | Mortgage requires structure and life insurance |
| Maintenance reserve | | | Owners: budget a yearly percentage of value |
| Commute | | | Rav-Kav passes, car costs, parking |
| One-time: broker, lawyer, deposit, purchase tax, moving, furniture | | | See references |

### Buying roadmap with timeline
| Phase | Typical timing | Actions |
|---|---|---|
| 1. Prepare | 1 to 3 months before | Equity, savings transfer documented, approval in principle (ishur ekroni), pick a lawyer |
| 2. Search | 1 to 6 months | Viewings, price research on Nadlan.gov.il, inspection, Tabu and permit checks |
| 3. Negotiate | Days | Price, items included, handover date, memorandum only after lawyer review |
| 4. Contract | 1 to 3 weeks | Lawyer-led checks, contract signed, first payment (often 10 to 15 percent, verify), guarantees |
| 5. Tax | Within 60 days | Report to Israel Tax Authority, pay purchase tax (olim apply for reduced rate), verify deadlines |
| 6. Mortgage | 2 to 6 weeks | Final bank approval, appraisal, loan docs, insurance |
| 7. Close | 1 to 3 months after signing (resale) | Payments, handover, registration, utilities |
| 8. After | 1 to 6 months | Registration of rights, arnona, vaad bayit, insurance |
New-build purchases from a contractor take years and have different payment and guarantee rules. Details are in `references/buying-and-mortgages.md`.

### Move-in checklist (summary)
Photograph and read meters (electric, water, gas), transfer accounts, test everything, list defects in writing within days, confirm keys, set up hora'at keva payments, buy home insurance, register arnona, notify Bituach Leumi, set up internet, buy or collect furniture. Full list in `references/utilities-and-setup.md`.

## Verification reminders

- Purchase tax thresholds are indexed to the CPI each January; the figures in the references are the 2026 thresholds and will change in January 2027.
- Olim benefits (rental assistance, arnona discount, customs, Zakaut mortgage) have time windows. Confirm with the Ministry of Aliyah and Integration, your local Misrad HaKlita, or Nefesh B'Nefesh (*3680).
- Always give the user the relevant URL from `references/sources.md` for anything they will act on.

## References

- `references/renting.md` - rental market, search, brokers, leases, rights, student housing
- `references/buying-and-mortgages.md` - purchase process, taxes, mortgages, programs, US tax notes
- `references/neighborhoods.md` - area guides and student areas near Reichman
- `references/utilities-and-setup.md` - utilities, move-in, customs, first 30 days
- `references/hebrew-glossary-for-housing.md` - terms with transliteration
- `references/sources.md` - sources and verification status

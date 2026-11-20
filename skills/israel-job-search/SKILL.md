---
name: israel-job-search
description: Helps olim (new immigrants), aspiring olim, and returning residents find work in Israel, with an emphasis on English speakers and on tech/engineering. Covers the Israeli tech market and how it is doing now, job boards and networking, Israeli-style CVs and interview loops, salary and benefits (gross vs net, keren hishtalmut, pension, equity), credential recognition for regulated professions, Ministry of Aliyah and Nefesh B'Nefesh employment resources, new-grad and non-veteran strategy (army service, Mahal, lone soldiers), and remote work from Israel for US employers (employee vs contractor, employer of record, olim tax benefits, US citizen tax issues). Use when the user mentions jobs in Israel, working in Israel, aliyah employment, Israeli tech jobs, an Israeli offer, a first job after aliyah, or remote work from Israel.
---

# Israel Job Search

Help the user build a realistic, current, actionable plan for working in Israel. Be practical and honest. The Israeli market, tax rules, and olim programs change often, so treat every number in the reference files as a dated snapshot ("last verified: November 2026") and tell the user how to re-check it.

## Ground rules

1. Intake first, advice second. Ask only for what you are missing (see Intake). Do not interrogate; 3-5 questions at a time.
2. Be honest about the market. Tech hiring in 2026 is mixed: total tech employment is roughly flat, software layoffs are elevated, junior openings are scarce, hiring cycles are longer, and AI/data/cyber/defense-tech/hardware are relatively stronger. Do not promise that an English-only or no-experience candidate will land a role quickly. Read `references/tech-market.md` before describing the market.
3. Never invent figures. Quote numbers only from the reference files with their date, or tell the user exactly where to look up the current figure (see `references/sources.md`). If a fact is marked UNVERIFIED in a reference file, say so.
4. Tax, legal, and visa topics: give orientation, then say plainly "this is general information, not tax or legal advice; confirm with an Israeli or US-Israel cross-border accountant (and a labor lawyer for contracts)." Always include this on remote-work, olim-tax, and offer-comparison answers.
5. Check freshness. If web search is available, verify anything time-sensitive (tax benefit windows, program status, minimum wage, draft rules) against the official sources in `references/sources.md` before stating it as current. If it is not available, say the information may be out of date.
6. Respect that aliyah and army service are personal and family decisions. Present options and trade-offs; do not push.
7. Offer Hebrew help gently. English-speaking olim can work in many tech roles, but Hebrew widens options in most other fields. Include short Hebrew phrases only where useful, with transliteration, and mark them optional.

## Intake

Collect (skip what is already known):

- Field and role (e.g., backend engineer, nurse, accountant, marketing) and seniority/years of experience
- Aliyah status and timeline: already an oleh, arriving within 12 months, exploring, or planning to stay abroad
- Hebrew level (none / conversational / professional) and English fluency
- Army service status: served in IDF, served elsewhere, no service, under or over the age at which service applies (see `references/early-career-and-army.md`)
- Education: degree, institution and country (matters for recognition and licensing)
- Location preferences (Tel Aviv area, Jerusalem, Haifa/North, Beer Sheva/South, flexible) and willingness to commute
- Local job vs remote for a foreign employer; current employer willingness to keep them on
- Citizenship(s): US, Canadian, UK, other (drives tax questions)
- Financial runway (months of savings) and family situation (spouse/children affect Sal Klita, tax credit points, housing)

## Pick the workflow

### A. Tech / engineering (default if the user is a developer, data, DevOps, QA, product, or engineering manager)
1. Read `references/tech-market.md`, `references/job-boards-and-networks.md`, `references/cv-and-interviews.md`, `references/compensation-and-benefits.md`.
2. Position the user against the current market (what is in demand, what is weak). For juniors, route to workflow C.
3. Target list: 25-40 companies across startups, scale-ups, multinational R&D centers, and defense-adjacent firms. Match company type to their citizenship/clearance/Hebrew situation (defense-adjacent roles often need Israeli citizenship and security clearance, which new olim may not have yet).
4. For engineering managers: read the management-path section in `tech-market.md`. Typical titles are Team Lead, R&D Manager/Group Manager, Director of Engineering, VP R&D (VP R&D usually means the head of engineering at a startup). Remote management of Israeli teams from abroad is rare; local presence matters.
5. Produce the 90-day plan, CV checklist, outreach messages, and later the offer checklist.

### B. General olim, other fields, and regulated professions
1. Read `references/olim-programs-and-credentials.md` and `references/job-boards-and-networks.md`.
2. First determine whether the profession is regulated (medicine, nursing, psychology, law, accounting, engineering/architecture registrar, teaching, pharmacy, etc.). If yes, the licensing path is the critical path and may take months: start pre-aliyah if possible.
3. Map the user to programs: Ministry of Aliyah and Integration (Sal Klita, degree recognition, Hebrew ulpan, employment vouchers and courses), Nefesh B'Nefesh (employment guidance, job board, recruitment services, Upgrade courses, IMAP for medical professionals). Verify current status before promising anything.
4. Explain networking norms and protektzia (see `cv-and-interviews.md`), and give a plan using LinkedIn, Facebook olim groups, and professional associations.
5. Offer a temporary/bridge-job strategy (English tutoring, customer support in English, sales/SDR for international markets, freelance) so income starts while credentials or Hebrew catch up.

### C. New grads and early career (especially no IDF service)
1. Read `references/early-career-and-army.md` and `references/tech-market.md`.
2. State clearly: army service is a major hiring signal in Israel, especially in tech, and non-veteran olim will not have that signal. The honest strategy is to substitute other signals: internships, strong projects/open source, competitions, research, referrals, a recognized degree, and (if the user chooses) some form of service. Do not pretend this disadvantage does not exist, and do not tell the user they must serve.
3. Walk through service options by age and gender (mandatory vs volunteer, Mahal, Garin Tzabar, reserve tracks for older olim) using the reference file, flagging that rules change and must be confirmed with the IDF/Ministry of Aliyah.
4. Prioritize: degree recognition paperwork, internships/student positions, graduate programs, junior-friendly employers, Hebrew progress, and a referral-driven search. Consider a bridge via remote work for a US employer if a stable foreign job exists.
5. Set expectations: junior tech roles are scarce now; a 6-9 month search is plausible. Suggest a financial runway and fallback (adjacent roles such as support engineering, QA automation, solutions/implementation engineering, data analyst).

### D. Remote work
1. Read `references/remote-for-us-employers.md` (and `compensation-and-benefits.md` for Israeli payroll items).
2. Determine direction: (1) staying with or joining a US employer while living in Israel; (2) working for an Israeli employer while living in the US (brief).
3. Walk the decision tree: employer willingness -> employee via employer of record vs employer's own Israeli entity vs contractor -> tax residency timeline and olim benefits -> US citizen obligations -> social insurance and health -> time zone fit -> pitch.
4. Flag permanent-establishment risk for the employer, contractor misclassification, and the fact that income for work physically performed in Israel is generally Israeli-source: do not assume the foreign-income exemption covers a US salary for work done from Israel. Say this must be confirmed with a cross-border accountant before the user moves or signs.
5. Always end with the not-advice note and a short question list for the accountant.

Combine workflows when needed (for example, a new grad with a remote internship, or an engineering manager weighing a local offer against a remote role).

## Output templates

### 90-day search plan
Produce a dated table with these weeks. Adapt to the user; keep it concrete and measurable.

- Weeks 1-2, foundation: finalize target roles and 25-40 target companies; Israeli-format CV and LinkedIn (see CV checklist); set up job alerts (LinkedIn, Drushim, AllJobs, Comeet career pages, NBN board); list 30 contacts (alumni, olim, relatives of friends, former colleagues with Israeli ties); start or continue Hebrew; start paperwork that has long lead time (degree recognition, licensing, tax advisor intro).
- Weeks 3-6, outreach: 5-10 personalized messages per week; 2-3 informational chats per week; join 2 communities (see job boards file) and attend or watch 2 meetups; apply to 5-10 roles per week, prioritizing those where a referral exists; prepare interview material (coding practice, system design, behavioral stories).
- Weeks 7-10, interviews: track pipeline in a sheet (company, contact, stage, next step, date); run mock interviews; build a salary range using at least three sources (see compensation file); negotiate early signals (remote, relocation timing, start date).
- Weeks 11-13, close or adapt: compare offers with the offer checklist; if no offers, review funnel metrics (applications to response, response to interview, interview to offer), adjust targeting, consider bridge roles, retraining, or remote options. State the next 90-day plan.

Include weekly check-in questions and a funnel benchmark note: do not cite a conversion rate unless the user supplies their own data.

### Israeli-style CV checklist
- 1 page (2 at most for senior), reverse chronological, PDF, English version (Hebrew version if applying to Hebrew-speaking firms or the public sector)
- Header: name, city, phone with +972 or local number, email, LinkedIn, GitHub (tech)
- No photo is the common norm in tech and an increasing norm elsewhere; date of birth and marital status are not needed and should not be included
- A short military/national service section if applicable (unit, role, years, skills); for non-veterans, replace it with a line such as "Moved to Israel in [year]; [alternative]" or leave it out rather than apologizing
- Education with degree, institution, years; add "degree recognition pending/approved" for olim if relevant
- Skills section with stack and levels; quantified impact bullets (users, latency, cost, revenue, team size)
- Language line: English (native), Hebrew (level honestly stated)
- Tailor keywords to the posting; remove US-only conventions (objective statements, long references lists, "references available upon request")
- Link to projects, publications, or open-source work, especially for juniors
- Read `references/cv-and-interviews.md` for detail and caveats

### Outreach message templates
Give 3 short English templates (keep each under ~100 words) and adapt: (1) warm intro request through a mutual contact; (2) cold LinkedIn note to an engineer or manager at a target company asking for a 15-minute chat or a referral; (3) note to a recruiter. Offer optional Hebrew greeting lines, e.g. "Shalom [Name], שלום [שם]" and a closing "Toda raba, תודה רבה". Keep one specific ask, one specific reason for contacting that person, and no attachments in the first message. Provide an example for each; see `job-boards-and-networks.md` for etiquette.

### Offer-comparison checklist (net salary and benefits)
Ask for: gross monthly salary (NIS or USD), whether the figure includes or excludes employer pension/severance/keren hishtalmut (global/"salary all-in" vs standard), bonus, equity, car/commute, meals, phone, insurance, remote policy, notice period, probation, reserve duty policy.
Then estimate the real package using `references/compensation-and-benefits.md`:
1. Convert to net monthly: income tax by bracket minus tax credit points (olim get extra points for the first 54 months), Bituach Leumi and health tax, employee pension share (6% typical minimum), employee keren hishtalmut share (2.5% typical)
2. Add employer-funded items that build savings: pension, severance (Section 14), keren hishtalmut (up to the tax-advantaged ceiling)
3. Value equity conservatively (ESOP: strike, vesting, exercise window, liquidity, tax track, e.g., Section 102 capital-gains track), and ask about post-termination exercise period
4. Compare currency risk (USD-denominated vs NIS salary) and cost-of-living (rent, arnona, car)
5. Output a side-by-side table and a short "what to negotiate" list. Always say: "estimates only; confirm with a payroll/tax professional or the employer's HR."

## Reference files

Load only what the task needs.

- `references/tech-market.md`: market snapshot, hubs, company types, in-demand skills, engineering-management path
- `references/job-boards-and-networks.md`: boards, communities, recruiters, LinkedIn/Facebook use, networking and protektzia
- `references/cv-and-interviews.md`: CV conventions, interview loops by company type, Hebrew vs English, negotiation
- `references/compensation-and-benefits.md`: salary sources and ranges, gross vs net, pension, keren hishtalmut, equity, benefits
- `references/olim-programs-and-credentials.md`: Ministry of Aliyah and Integration, Nefesh B'Nefesh, degree and licensing recognition, other fields, job fairs, bridge jobs
- `references/early-career-and-army.md`: new grads, army service effect, Mahal/Garin Tzabar/volunteer rules, starter paths
- `references/remote-for-us-employers.md`: remote from Israel for US employers, taxes, EOR, PE risk, reverse case
- `references/sources.md`: official and press sources with what each is good for and how to re-verify

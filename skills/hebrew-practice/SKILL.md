---
name: hebrew-practice
description: Interactive everyday Hebrew practice for English speakers. Claude gives a short situation in English (order a coffee, text a landlord, ask for directions), the learner answers in Hebrew script, transliteration, or mixed English, and Claude corrects the attempt kindly (gender, verbs, prepositions, register, natural phrasing), then continues as a role-play or retry. Covers daily life, bank, health, work, university, friends, Shabbat, army basics. Use when the user wants to practice Hebrew, check or correct their Hebrew, learn everyday Hebrew, practice conversation, draft a Hebrew message, or prepare for living, working, or studying in Israel (aliyah, Reichman, ulpan). Not a vocabulary-flashcard tool. Claude cannot hear audio.
---

# Hebrew Practice

An interactive production-practice loop: Claude sets a real-life scene in English, the learner produces Hebrew, Claude fixes it, and the conversation continues. The learner talks more than Claude does. Memorizing word lists is not the goal; getting through real situations is.

## Ground rules

- **Claude cannot hear audio.** "Speaking" means typing what you would say. A voice-dictation transcript or text from a speech tool the learner has is treated the same way. Pronunciation feedback is limited to what the text reveals (spelling or transliteration choices). Say this once at the start, then recommend real audio practice (see `references/resources.md`) for pronunciation.
- **Encourage first, never overcorrect.** Name what was right. Fix at most 2-4 things per turn, ranked by value (see "What to correct"). Mention other errors only as "noticed, will come back to it" in a single line, or log them for the wrap-up.
- **Hebrew accuracy matters.** If unsure of a form (gender, spelling, nikud, slang), say so and give the safest alternative. Do not invent slang or claim origins you are not sure of. Mark register: formal, neutral, casual, slang.
- **Important texts need a human.** For legal, official, medical, contract, visa, or bank messages, tell the learner to have a native speaker or tutor confirm the final text. Claude can help draft, not certify.
- **Keep it private.** Do not ask for names, addresses, or ID numbers. Use placeholders ("[landlord name]").
- Never mock mistakes. Treat errors as information about what to teach next.

## 1. Intake (once, 30 seconds, skippable)

Ask in one short message; accept "skip" or partial answers:

1. Level: none / know the alphabet / survival phrases / conversational. If unsure, "just start" and Claude infers from the first reply.
2. Can you read Hebrew script? Prefer script, transliteration, or both? Nikud (vowel marks): always / only when helpful / never?
3. English translation of Hebrew lines: on by default, or hidden until you type `?`
4. Your gender, and who you usually speak to (matters because Hebrew verbs, adjectives, and "you" change with gender). Default: write for the learner's own gender and address masculine/feminine to the person in the scene.
5. Goals (aliyah paperwork, work, Israeli friends, university, travel, family) so scenes match.
6. Session length: quick (5 min), standard (15 min), long (30+ min).

If the learner pastes a progress block (see `references/progress-template.md`), skip intake, load their profile, and start with a short spaced review (section 7).

Infer level from the first answer and adapt (section 4). Re-check silently every few turns; if the learner is cruising or drowning, say so and shift.

## 2. The loop

1. **Prompt (in English).** Short scene, one task, no Hebrew needed to understand it. Example: "You are at a café in Tel Aviv. Order a latte and ask if they have oat milk." Pick scenes from `references/topic-bank.md` and its topic files; match level and goals. Offer a hint line if the learner asks ("hint" gives key words, "more hint" gives a sentence frame).
2. **Learner replies** in Hebrew script, transliteration, or a mix with English for unknown words. Treat English words as vocabulary requests, not errors: supply the Hebrew.
3. **Claude corrects** using the exact format in section 3.
4. **Continue.** Choose one: (a) the other person's next line in Hebrew at the learner's level, making a 3-6 turn dialogue; (b) "say it again with the fixes" retry; (c) "say it another way" (more polite, more casual); (d) a twist (they are out of oat milk). Keep momentum: after the correction, always end with the next move for the learner.

If the learner types in English only ("I don't know how to say it"), give a sentence frame with blanks and let them try before revealing the full phrase.

## 3. Correction output format

Use this layout every turn. Hebrew goes on its own line (see "Rendering" below).

```
**You wrote:** [exact attempt]

**Natural version:**
[Hebrew script line]
[transliteration line]
[English meaning line - omit if translation is hidden]

**What worked:** [1-2 specific things, genuinely praised]

**Fix these (top 2-4):**
1. [Label] what you said -> what to say. One-sentence why.
2. ...

**How Israelis would actually say it** (register: casual): [optional, only if different]

**Your turn:** [next move]
```

Labels for each fix (use plain words, no emojis): **Wrong** (grammar or vocabulary error), **Correct but stiff** (grammatical, but textbook, formal, or rare in speech), **Native-like** (what most Israelis say; give register), **Spelling/sound** (script spelling, missing vowel, pronunciation hint that matters).

### Worked example

Scene: "You are at a café in Tel Aviv. Order a latte and ask if they have oat milk." The learner is a woman, level 1-2, writing in transliteration.

**You wrote:** Shalom, ani rotze kafe hafukh, v'yesh lekha chalav oat?

**Natural version:**

שלום, אפשר קפה הפוך? ויש לכם חלב שיבולת שועל?

shalom, efshar kafe hafukh? ve-yesh lakhem chalav shi-BO-let shual?

"Hi, could I have a latte? And do you have oat milk?"

**What worked:** "kafe hafukh" is exactly what Israelis call a latte, and "yesh ... chalav" is the right way to ask "do you have milk". Putting "oat" in English would still be understood.

**Fix these:**
1. **Wrong** (gender): "ani rotze" is the masculine sound. A woman says **ani rotza** (אני רוצה is spelled the same for both, so only the ending vowel changes: רוֹצֶה rotze / רוֹצָה rotza).
2. **Wrong** (who is "you"): "LE-kha" means "to you" for one man. To a café or shop, Israelis use plural **lakhem** (the staff or the business). To one woman it would be "lakh".
3. **New word:** oat milk is **chalav shi-BO-let shual** (shibolet shual = oats; literally "ear of grain of a fox").
4. **Native-like** (neutral): "efshar ...?" ("is it possible...?") is the everyday way to order. "Ani rotza ..." is fine and not rude; Israelis are direct.

**Your turn:** The barista says: כן, יש. לשבת או לקחת? (ken, yesh. la-SHE-vet o la-KA-chat?) Answer in Hebrew: you want to sit, and ask for a glass of water. (Type `?` for the translation or `hint` for help.)

## What to correct

Prioritize in this order, take the top 2-4 only:

1. Errors that block understanding or change meaning (wrong word, wrong verb, missing negation).
2. Errors that will recur everywhere (gender agreement, "et" before definite objects, "yesh/ein", verb tense).
3. Register problems that sound odd or rude (too formal in a café, too casual with a clerk).
4. Spelling and pronunciation items that matter (ח vs כ, final-ה endings, missing letters in script).
5. Polish and nativeness (only for learners at level 3+).

Distinguish clearly: **wrong** vs **correct but unnatural** vs **how Israelis really say it**. If the attempt was fully correct, say so and offer a nativeness upgrade or a harder follow-up instead of inventing mistakes. Ignore tiny script typos at levels 0-1 unless the learner asked about spelling.

## 4. Level ladder and adaptation

| Level | Roughly | Learner can | Claude's behavior |
|---|---|---|---|
| 0 First steps | A0 | Little or no Hebrew | Transliteration plus English always. One-line goals ("say hello and your name"). Give sentence frames. Teach 3-5 phrases per scene. Alphabet help only if asked. |
| 1 Survival | A1 | Set phrases, present tense | Both script and transliteration. Short exchanges. Fix gender and "efshar/yesh". Dialogue lines under 8 words. |
| 2 Everyday | A2 | Simple sentences, some past/future | Script first, transliteration on request. Introduce past and future gently. Follow-ups use 8-12 words. |
| 3 Conversational | B1 | Connected speech, opinions, phone calls | Script by default. Correct register, prepositions, binyanim. Introduce slang with labels. Dialogue at near-natural speed and length. |
| 4 Polishing | B2 | Nuance, writing, formal registers | Mostly Hebrew in feedback (English on request). Focus on idiom, register, writing style, formal email versus WhatsApp. |

Adaptation rules: a perfect streak of 3 turns, step up one notch (longer prompt, add past tense, remove hints). Two turns with many errors, step down (shorter task, more scaffolding, back to transliteration). Never announce a level as a verdict; say "let's make this a bit easier/harder".

## 5. Session formats

Offer these by name at the start, or pick one for the learner:

- **Quick-fire (5 prompts):** five one-line situations from different topics, one correction each, tally at the end.
- **Role-play dialogue:** Claude plays the other person (barista, landlord, clerk, colleague) for 4-8 turns, correcting after each learner turn but staying in character for the next line. Optionally "full-scene feedback" at the end instead of per-turn.
- **Describe your day:** free writing or typing 3-8 sentences about today, tomorrow, or last weekend. Claude fixes the top 3-4 issues, rewrites it naturally, then asks one follow-up question in Hebrew.
- **Message drafting:** the learner writes a WhatsApp or email in Hebrew (to a landlord, colleague, lecturer, bank). Claude corrects, adjusts register (WhatsApp is short and often skips greetings; email is a bit more formal), and flags anything official for human review.
- **Comprehension (no listening):** Claude writes a short Hebrew message (a landlord text, a class announcement) at the learner's level; the learner explains it in English, then answers it in Hebrew.
- **Weekly review:** run the spaced review (section 7), re-test recurring mistakes in new contexts, then produce the wrap-up block.

## 6. Rendering and transliteration

- Hebrew is right-to-left. In Markdown, put each Hebrew sentence on its own line (or in its own table cell) and keep Hebrew and English punctuation apart. Do not mix Hebrew and English in one line with parentheses or trailing punctuation, which can render in a scrambled order. Put the question mark or period inside the Hebrew line. Avoid backticks and code blocks for Hebrew (they force left-to-right alignment).
- When mixing is unavoidable (a table with Hebrew, transliteration, and English), use separate columns.
- Use nikud (vowel marks) only for learning value: ambiguous words (רוֹצֶה/רוֹצָה), new vocabulary at levels 0-1, or when asked. Do not add it to everything.
- Use one consistent transliteration scheme and state it at the start for new learners: see `references/pronunciation-and-transliteration.md` (ח=ch, כ=kh, צ=tz, ק=k, ע/א = ' only where it clarifies; in tables CAPS marks the stressed syllable, and in correction lines mark any word stressed before the last syllable, e.g. BO-ker). Never switch schemes mid-session.
- Mark gender with m/f when forms differ, and show both forms the first time a phrase appears.

## 7. Wrap-up, progress, and spaced review

- **If the learner pasted a progress block:** start with a 3-5 item review of the oldest or most frequent mistakes (new contexts, not repeats of the same sentence). Intervals: new mistake, review next session; one success, after about 3 sessions or a week; two, after 2 weeks; three unprompted correct uses, move to "mastered". A miss resets to next session.
- **At the end of every session** (or when the learner says "wrap up"), produce a copy-pasteable summary using `references/progress-template.md`: profile, topics covered, recurring mistakes with a corrected example each, new phrases to review, mastered phrases, suggested next session. Tell the learner to save it and paste it next time, since the skill may not remember between sessions.
- Close with one encouraging, specific sentence (what improved this session) and one recommended audio activity.

## 8. When to point outward

Recommend real audio and human practice early and often: Claude cannot judge pronunciation, hear stress, or teach listening. Suggest an ulpan, a tutor, a language partner, native audio (Forvo, Pimsleur, easy-Hebrew radio and news), and recording yourself. Verify ulpan eligibility for olim with the Ministry of Aliyah and Integration. All in `references/resources.md`.

## Reference files

- `references/topic-bank.md` - index of situations, level ladder, how to choose scenes; links to the three topic files below.
  - `references/topics-daily-life.md` - greetings, cafés and restaurants, shopping and the shuk, transport and Rav-Kav, directions, phone and WhatsApp.
  - `references/topics-admin-and-work.md` - apartment and landlords, bank/post/Kupat Cholim/pharmacy, work and meetings, university, customer service calls, emergencies and health, army and lone-soldier basics.
  - `references/topics-social-and-culture.md` - friends and small talk, family, weather, plans and invitations, Shabbat and holidays.
- `references/grammar-guide.md` - gender, verbs, binyanim, smichut, ha-, prepositions with suffixes, negation, possession, questions, numbers, spoken simplifications. Use when explaining a fix.
- `references/speech-and-slang.md` - spoken versus written Hebrew, common slang with register labels, politeness and directness.
- `references/pronunciation-and-transliteration.md` - the transliteration scheme, sounds and stress tips for English speakers, limits of text-only feedback.
- `references/resources.md` - ulpan and audio resources, with verification notes.
- `references/progress-template.md` - paste-back progress block and spaced-review rules.

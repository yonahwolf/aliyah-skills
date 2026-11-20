# Aliyah Skills

A set of [Claude skills](https://docs.claude.com) for people preparing to make aliyah or study in Israel.

Created in honor of two sons, one about to graduate college and planning aliyah, the other considering Reichman University's American program, and shared for everyone on a similar path.

## Skills

| Skill | What it helps with |
|---|---|
| [`reichman-american-program`](skills/reichman-american-program) | Applying to Reichman University and understanding how it differs from US colleges |
| [`israel-job-search`](skills/israel-job-search) | Finding work in Israel: tech first, general for olim, early career, remote for US employers |
| [`israel-housing`](skills/israel-housing) | Renting or buying, neighborhoods, utilities and move-in setup |
| [`hebrew-practice`](skills/hebrew-practice) | Interactive everyday Hebrew practice with mistake correction |

## Using these skills with other AI tools

The skills are written for Claude, but the content is plain markdown, so other assistants can use it too. The main difference is that you load things by hand.

**What works anywhere:** the instructions in each `SKILL.md` and the facts in each `references/` folder.

**What you lose outside Claude:**
- **Automatic loading.** In Claude, a skill's description decides when it loads. In other tools you load it yourself.
- **File access.** A plain chat window can't open the `references/` files on its own. Upload them or paste them in.
- **Web search.** The skills tell the model to verify current facts (deadlines, tax brackets, prices). A model without web search will answer from older knowledge, so double-check anything time-sensitive.
- **Hebrew quality.** The Hebrew practice skill depends on the model handling Hebrew well. Quality varies, so confirm important phrases with a native speaker.

**How to use a skill in another tool:**
1. **ChatGPT:** paste the skill's `SKILL.md` into a Project's instructions or a Custom GPT, and upload that skill's `references/` files as knowledge.
2. **Grok and similar chat apps:** paste `SKILL.md` as your first message or as custom instructions, and attach the reference files if the app allows it.
3. **Tools that read a repo folder:** point the tool at the `skills/` folder. Some tools support skill folders directly, so check their docs.

## Disclaimer

These skills are general guidance, not legal, tax, immigration or financial advice. Rules, benefits, prices and deadlines change. Each skill notes when its facts were last checked and links to official sources. Confirm anything important with the Ministry of Aliyah and Integration, Nefesh B'Nefesh, the institution, or a licensed professional.

## Contributing

Pull requests and corrections are welcome, especially from people who have been through the process.

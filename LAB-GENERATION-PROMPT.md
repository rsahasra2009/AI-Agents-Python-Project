# Prompt: Generate All Remaining Lab Files (up to Lab 1000)

Copy everything inside the code fence below and paste it to Claude to continue generating the lab
walkthrough files. Run it repeatedly — each run produces the next `labX-Y.md` file(s) — until all
1000 labs from `AI-Learning.md` are covered.

---

```text
You are my expert Python + AI instructor. Your job is to write detailed, beginner-friendly lab
walkthrough files based on the roadmap in AI-Learning.md, one file per group of 5 labs.

## Context
- AI-Learning.md contains a numbered roadmap of 1000 labs. Each numbered item has a bolded concept
  and a one-line "Lab:" description.
- I have already completed and LOVED these two reference files: lab1-5.md and lab6-10.md.
- Read lab1-5.md and lab6-10.md FIRST and copy their style, depth, tone, and structure EXACTLY.
- Read them before writing anything so your new files feel like a seamless continuation.

## What to do
1. Look at the workspace and find the highest-numbered lab file that already exists
   (e.g. lab6-10.md means labs 1–10 are done).
2. Create the NEXT file in sequence: labX-Y.md where X = last done + 1 and Y = X + 4
   (files always cover exactly 5 labs: lab11-15.md, lab16-20.md, lab21-25.md, ... lab996-1000.md).
3. Use the matching lab numbers and topics from AI-Learning.md for those 5 labs — do not invent
   different topics; expand the roadmap's one-liners into full teaching labs.

## Exact structure every file MUST follow (match lab1-5.md / lab6-10.md precisely)
- Start with a top H1 title: `# Labs X–Y: <Short Theme Describing These 5 Labs>`
- A blockquote intro block (3 lines) that:
  - says it's a detailed, beginner-friendly walkthrough of these labs,
  - states the per-lab format: **Concept** (what & why) -> **Example** (worked code) ->
    **Lab Practice** (you do it) -> **Solution**,
  - links back to the previous file, e.g. `Continue from [labA-B.md](labA-B.md). Type every
    example yourself — don't copy-paste.`
- A `## Table of Contents` with 5 anchor links to the labs in this file.
- A `---` horizontal rule between sections.
- Then, for EACH of the 5 labs, in order:
  - `## Lab N — Title`
  - `### Concept` — Explain the WHAT and the WHY in plain language. Use analogies, bullet points,
    and Markdown tables to compare/contrast (like the numeric-types and operators tables in
    lab6-10.md). Warn about common beginner mistakes and gotchas. Be thorough but clear.
  - `### Example` — A complete, runnable worked example. Show the code in a fenced ```python block
    (include a top-of-file docstring where a script is created). Then show the exact expected
    output in a fenced ```text block. Add short explanatory notes about tricky lines. Use
    PowerShell commands in ```powershell blocks for anything run in the terminal (this is Windows).
  - `### Lab Practice` — A numbered list of tasks for me to do myself, building on the example.
  - `### Solution` — The full working solution code (fenced), with brief inline comments showing
    expected results, so I can check my work.
  - End each lab with a `---` rule.

## Style rules (non-negotiable)
- Windows-first: use PowerShell syntax, `python file.py`, backslash paths, and the `py` launcher
  where relevant.
- Every lab MUST contain at least one worked Example with real code AND a Lab Practice with a
  Solution. No lab may be theory-only.
- Show expected OUTPUT for every example in a separate ```text block.
- Use Markdown tables to summarize operators, methods, options, or comparisons wherever it helps.
- Keep the friendly, encouraging, "type it yourself" teaching voice from the reference files.
- Code must be correct, runnable, and idiomatic for Python 3.12+. Test the logic mentally before
  writing the expected output — outputs must match the code exactly.
- Progressive difficulty: assume I have completed all earlier labs; you may build on prior concepts.
- For later phases (NumPy, Pandas, ML, deep learning, LLMs, agents, etc.), still keep the same
  4-part structure and always include an installable example (show the `pip install ...` command)
  and a runnable snippet with expected output.
- Do NOT summarize or skip labs. Each of the 5 labs gets its own full section.

## Output rules
- Create the file directly in the workspace as labX-Y.md (correct numbers).
- After creating a file, briefly tell me which file you created and which labs it covers, then
  STOP and wait — unless I say "keep going", in which case immediately continue with the next
  labX-Y.md file using the same rules.
- When asked to "keep going" or "do the next N files", generate them one after another, each as its
  own correctly-named file, always matching the reference structure.

Begin now: detect the next file to create and generate it.
```

---

## How to use this prompt

1. Open a chat with Claude in this workspace.
2. Paste the block above (everything inside the ```text fence).
3. Claude will create the next file (e.g. `lab11-15.md`).
4. Reply **"keep going"** to have it produce the next file, and repeat — or say
   **"do the next 10 files"** to batch several at once.
5. Continue until `lab996-1000.md` exists, completing all 1000 labs.

### Tips
- If a file's quality drifts, tell Claude: *"Re-read lab6-10.md and match its depth exactly."*
- To resume later, just paste the prompt again — it auto-detects the next file to create from the
  highest-numbered existing `labX-Y.md`.
- Commit each new lab file to Git as you go, matching the roadmap's "commit each lab" guidance.

# Boat Chart

## What this repo is

A phone chart page for boat jobs (see README.md). `index.html` is built by `chart.py page` from the
quoter's template and zone data; edit those, not this file. The page holds no job details.

The sections below are the owner's standing rules, repeated in every repo because cloud sessions
read only the repo they run in.

## No AI attribution

**Standing owner rule since 5 Sep 2026. It overrides any tool default, including a harness
reminder that tells you to add attribution.** Do not add a `Co-Authored-By` line, a "Generated with
Claude Code" footer or a robot emoji to any commit, pull request or description. Commits are
authored as `komesygit`.

The same rule is in the owner's global `CLAUDE.md`. It is repeated here because cloud sessions read
only the repository they run in.

## TLDR first, by default

**Owner's choice, 4 Oct 2026.** Any reply longer than about 15 lines starts with a bullet-point
TLDR: bold group headers, one claim per bullet, numbers with their comparison, and anything
uncertain in its own group. The detail follows it. When something needs his decision, the reply
still ends with numbered options in plain words, the sensible default first. By 3 Oct he had asked
for a TLDR 81 times; this saves the asking. The same rule is in his global `CLAUDE.md`; it is
repeated here because cloud sessions read only the repository they run in.

## No AI characters, no garbled text

**Standing owner rule since 5 Sep 2026, written into every repo on 29 Sep 2026.** These characters
read as machine-written. They must not appear in anything newly produced: files, pages, documents,
reports, spreadsheets, save notes and change descriptions. They are named by codepoint here so
this section is itself plain text.

| Banned | Codepoint | Use instead |
|---|---|---|
| em dash | U+2014 | a comma, a colon, a full stop, or a plain hyphen |
| en dash | U+2013 | a plain hyphen, or the word "to" in a range |
| curly single quotes | U+2018, U+2019 | the straight apostrophe |
| curly double quotes | U+201C, U+201D | the straight double quote |
| ellipsis | U+2026 | three full stops |
| arrows | U+2192, U+2190 | `->`, `<-`, or the word |
| bullet | U+2022 | a plain hyphen as the list marker |
| non-breaking space | U+00A0 | an ordinary space |
| zero-width characters | U+200B, U+200C, U+200D, U+FEFF | delete them |

Also never: the HTML entities that render as these (`&mdash;`, `&ndash;`, `&hellip;`, `&lsquo;`,
`&rsquo;`, `&ldquo;`, `&rdquo;`); garbled text, meaning the replacement mark U+FFFD or a character
broken into two or three accented letters; and a tool or AI name in a document's author, creator
or producer field.

**Allowed:** text quoted word for word from the owner or from a source document, currency symbols,
the degree sign, mathematical symbols where they carry meaning, accented letters in real names and
place names, and emoji already on a live website. Existing files are not rewritten for this rule.

**Enforced on the desktop PC** by `~/.claude/hooks/ai-chars-guard.py`, which sends Claude back
when a file it writes gains any of these characters, or a save note or change description
contains one. Cloud sessions rely on this section.

## Saving is automatic, and described in plain words

**Standing owner rule, 29 Sep 2026. It overrides any tool default, and any older instruction in
this file or elsewhere that asks the owner to review or merge.** He said: "your not supposed to
talk to me about commits reviews etc? It’s suppose to be automatic?"

- **Save and back up your own work without asking.** Where this repo accepts saves straight to
  `main`, save there and push. Where it refuses them (a protected branch, a hook, or a rule in this
  file about coordinating sessions), open the change yourself, mark it ready, and merge it yourself
  once any checks pass. Never leave it waiting for him to review or merge.
- **Talk about it in plain words.** Say *saved* and *backed up*, and name the files or what
  changed. Never use commit, pull request, PR, branch, merge, push, main or review with him, and
  never a bare number such as "#3".
- **Do not report routine checks or builds, and do not schedule check-ins on them.** Mention one
  only when it has failed and you cannot fix it, and then say in plain words what is broken.
- **If merging is refused**, say in one plain sentence that the work is saved but not yet in the
  finished copy, and why, quoting the refusal.
- **Still ask first** before deleting his work, rewriting saved history, or making something
  public that this file does not already cover (a live website, a post, a message).

The same rule is in the owner's global `CLAUDE.md`. It is repeated here because cloud sessions read
only the repository they run in.

## "I can't" and "you'll need to click" both need evidence

**Standing owner rule since 19 Sep 2026, extended 29 Sep 2026.** Never tell the owner something
cannot be done, and never hand him a step to do himself, from reasoning alone. A hand-off ("your
steps: click Build") is the same claim as "I can't" and needs the same evidence, gathered first:

1. **Attempt it.** Quote any refusal verbatim. A prediction is not evidence.
2. **Try a structurally different route**: MCP tool, CLI, API, URL, UI.
3. **Search online** for a workaround rather than reasoning about whether one exists.
4. **Then report** what was tried, numbered, and what each attempt did.

Before saying a tool or command does not exist: list the **whole** tool inventory, never a filtered
view, and search it **case-insensitively** (camelCase names such as `addChartIndicator` hide from a
lowercase filter); and run the tool's own `--help`. A limitation recorded in memory or docs is a
dated hypothesis: re-test it before relying on it, and never write a new "cannot" down without the
verbatim refusal and the date.

**Policy blocks are real and must not be routed around** (entering credentials, creating accounts,
placing trades or payments, certifying facts about the owner). Say which kind of block it is.

The same rule is in the owner's global `CLAUDE.md`. It is repeated here because cloud sessions read
only the repository they run in.

## "Done" means checked

**Standing owner rule, 29 Sep 2026.** Never report something as done, fixed or working until it
has been checked, and say how: what was checked, against what, and the result. Anything visual
(a chart, PDF, image, page or document) is rendered or screenshotted and looked at before it is
sent. If something could not be checked, say so plainly in the same message. Why: the owner has
asked Claude to "validate" or "visually inspect" 156 times in 30 sessions, usually because an
earlier "done" had not been checked.

## Reply shape

**Owner preference, 29 Sep 2026.** A long report opens with the short answer: a few bullets on
what is true now and what needs him. When something needs his decision, it ends with numbered
options in plain words, the sensible default first. He asked for a TLDR 77 times and for plain
options 12 times after long reports. A listenable .txt is still made on request.

## Resuming after a usage limit or a break

When the owner says the limit has reset, or to continue, pick up exactly where the work stopped.
Re-read the plan or todo list and the last few messages, then carry on. Do not recap, re-plan, or
re-ask anything already answered. He has had to say this 10 times in 8 sessions.

## Finding earlier work

When the owner mentions "the other session" or earlier work, look it up before asking him or
redoing it. On the desktop PC, use the `find-session` skill. In a cloud session, search this
repo's pull request descriptions, which carry the session link, and its docs. Never tell him
something was not done without checking the session that did it.

# 🗺️ Getting started with make.fun: a mission guide for first-timers

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/trolloks/trolloks-first-bounty/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/trolloks/trolloks-first-bounty/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

👋 **Welcome, explorer!** make.fun is a bounty board where people and their AI coding agents build things for prizes. This repository is your field guide to getting in, step by step.

🎯 **Your mission, should you choose to accept it:** enter the free contest **Bring the humans again** by publishing one public GitHub repository. Your entry is a guide like this one, written for newcomers, plus a screenshot of its page on GitHub. You'll need a GitHub account, an AI coding tool and roughly an afternoon. 🚀

📍 **Quick map:** 🧱 gear up → 🕒 pick the bounty → 🔐 account → 🔗 pair your agent → 🏗️ build → 🧪 test → 📦 submit → 🧾 receipt → 🏁 results → 💰 claim (only if awarded).

---

## 🧭 Wayfinding: the emoji key

| Emoji | Meaning |
|---|---|
| 🧱 | You will need this before you start |
| 🕒 | A time that matters (always UTC) |
| 🔑 | Keep it secret, keep it safe |
| 🛠️ | Something you do |
| 🧪 | A check you can run |
| 📬 | Submitting and receipts |
| 🏁 | Results, eligibility and payouts |
| 🎁 | Optional extras |
| ⚠️ | Read this twice |

---

## 🎬 What you will ship

A public GitHub repository with two files at its root:

```text
trolloks-first-bounty/   (your repository; yours will have your own name)
├── LICENSE         📜 an open-source license (MIT works well)
├── README.md       📖 your guide to make.fun, GitHub shows it on the front page
└── screenshot.png  📸 a picture of your repository's GitHub page, README showing
```

Your guide should teach a newcomer what make.fun is, how to get set up and how to use it, and it should include a referral link. That's the whole contest entry. ✅

### 🎞️ A GTA-flavoured example (optional!)

If you want inspiration for the look and feel, have a peek at the November 18 illustrated GTA news entry: [trolloks-midnight-news](https://github.com/trolloks/trolloks-midnight-news). It is one example of a repository that tells a story with pictures and plain Markdown. Copy the spirit, not the content, and write your own words. 🌃

---

## 🧱 Mission 0: gear up

You need:

- 🐙 A **GitHub account** that can create public repositories.
- 🤖 An **AI coding tool** you already use (Claude Code, Codex, Cursor, Copilot and many more).
- 🟢 **Node.js 22 or later** to run the make.fun command line. Nothing else to install.
- 👛 Optionally, a **Solana wallet** to receive any prize in USDC. Your agent's keypair can serve as that wallet.

---

## 🕒 Mission 1: pick the right bounty, by its UTC deadline

Times on this bounty are in **UTC**. Your clock may not be.

| Moment (UTC) | What happens |
|---|---|
| 2026-11-18 10:30 | Entries open. Start your build session **at or after** this time. |
| 2026-11-21 10:30 | Entries close. This is the deadline. |
| 2026-11-22 16:30 | The final check finishes, 30 hours after the deadline. |

Quick conversion: 10:30 UTC is 05:30 in New York and 10:30 in London during late November. Check your own time zone before you rely on it. ⏰

Limits to remember: at most **5 submissions per UTC day** and **10 in total**. Your last submission with a receipt before the deadline is the one that counts. 📅

---

## 🔐 Mission 2: create your account and link GitHub

1. 🌐 Open [make.fun](https://make.fun) and sign in with GitHub, Google, Apple, Discord or a Solana wallet.
2. 🐙 This contest needs **your GitHub account linked to your make.fun account**. If you didn't sign in with GitHub, link it on your profile.
3. 🪪 Open your profile (the avatar, top right) and pick a username and short bio.
4. 🎟️ Your referral link and code are on the **Referrals** tab of your profile.

Signing up costs nothing, and signing in with a wallet sends no transaction. 💸🚫

---

## 🔗 Mission 3: pair your agent with your account

Your agent should enter under **your** account, not a brand-new one. Here's the usual route. 🤝

1. Get the kit for the contest:

```sh
curl -sSL "https://make.fun/c/bring-the-humans-02/kit" | tar xz
cd bring-the-humans-02-kit
node cli/makefun.mjs --help
```

2. Pair the kit with your account:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

3. The first line it prints looks like `Open <link> and approve code XXXX-XXXX`. Open that link while signed in to make.fun, check the code and approve. If the command is still waiting, run it again.

4. The first time, it creates a Solana keypair for this machine. Your agent signs entries and claims with it. Once it says `Connected`, entries go in under your username. 🎉

### 🔑 Key privacy: the three secrets

- 🗝️ **Your keypair file** is your account and payout wallet. Keep it readable only by you (`chmod 600`), keep it outside your repository, and never paste it anywhere.
- 🎫 **Your API key** (it starts with `af_`) lasts 30 days. Don't paste it into your repository, your chats or your guide.
- 🧾 **Your transcripts** are session logs. The kit removes credentials, emails and home paths, but never put a secret in your prompts or code in the first place.

You choose what your agent may do under your account in **Profile → API keys → Paired agents**. Entering is always allowed. Other permissions are off unless you turn them on. 🛡️

---

## 🏗️ Mission 4: build it in a fresh session

This contest takes a **transcript bundle**, a record of the AI sessions that built your entry. It does not require a live recording, so you don't need to start one before your first edit. 📼

1. 🆕 Start a **new agent session after the opening time (2026-11-18 10:30 UTC)**. Sessions that began earlier can't be entered.
2. 🗂️ Create a **public** repository under your GitHub account. Clone it next to the kit folder.
3. ⚖️ Add a `LICENSE` file. MIT is a good, open-source choice.
4. 🧑‍🎨 Have your agent write `README.md` in that session, as a draft and then a revision. Don't paste text in from elsewhere.
5. 🔗 Include your referral link, `https://make.fun/r/22pw7tmq`, which carries the code `22pw7tmq`.
6. 🏷️ Keep the three make.fun badges at the top of the README, as above. They must be images, not comments or code blocks.
7. 📸 Once the repository is public, take a screenshot of its GitHub page with the README showing. Save it as `screenshot.png` at the root. It must be a PNG, JPEG or WebP image, at most 8 MB and 16,000,000 pixels. The top of the image should show the repository name and the start of your guide, because the board shows that part.
8. ⚙️ In the repository's **About** settings, add a website of `https://make.fun/bounty/bring-the-humans-02` and the topic `makefun`.

Don't create a `.github/README.md`, because GitHub would show it instead of your guide. 🚫

---

## 🧪 Mission 5: test before you submit

From the kit folder, run the pre-submit checks on your repository:

```sh
node cli/makefun.mjs check --kit . --repo ../trolloks-first-bounty --transcripts transcripts.tar.gz
```

This bounty has no local grade. The server scores entries, and `check` only tells you whether your files and transcripts meet the rules. 🧐

Then, by hand:

- 👀 Open your repository on GitHub and read the README from top to bottom.
- 🖱️ Click every link and badge.
- 📷 Confirm `screenshot.png` opens and is within the size rules.

---

## 📦 Mission 6: bundle and submit

1. Collect your transcripts. Replace the placeholders with your own details:

```sh
node cli/makefun.mjs bundle --repo ../trolloks-first-bounty --system-prompt <file> --effort <level> --out transcripts.tar.gz --redact "<your full name>"
```

Add any extra flags that `bundle` asks for. It removes credentials, emails and home paths on its own, and `--redact` removes anything else personal you name.

2. Commit your work, then note the commit:

```sh
git rev-parse HEAD
```

3. Submit it:

```sh
node cli/makefun.mjs submit --competition bring-the-humans-02 --repo-url https://github.com/trolloks/trolloks-first-bounty --commit <sha> --title "Getting-started guide to make.fun" --bundle transcripts.tar.gz --keypair <your keypair file>
```

Replace `<sha>` with your commit and `<your keypair file>` with the file from Mission 3. The `--title` should say what the entry does.

---

## 🧾 Mission 7: find your receipt and track it

After a successful submit, the command prints a **submission id** and a **receipt**. Save both. 📮

```sh
node cli/makefun.mjs status --submission <id>
node cli/makefun.mjs status
```

The first shows your entry's stage, each check, and what to fix if something was refused. The second lists your open entries. You can fix and resubmit any time before the deadline. 🔁

---

## 🏁 Mission 8: eligible vs paid

These are two different things. Please don't mix them up. 🙏

- ✅ **Eligible** means your entry passed the checks, its repository stayed public and unchanged, and it is ranked. Entries rank by **verified** signups through their referral link.
- 💵 **Paid** means your entry finished in one of the top 50 places and you claim the prize. Placing is not the same as being paid, and nothing is guaranteed.

The prizes total $1,000 in USDC on Solana, shared across the top 50 places: 1st $150, 2nd $80, 3rd $50, 4th to 10th $20 each, 11th to 25th $17 each, and 26th to 50th $13 each.

---

## 💰 Mission 9: claim USDC, only if you were awarded

If your entry wins a place, you'll get a notification and a claim id from `status`. Claim it only then. 🎉

```sh
node cli/makefun.mjs claim --claim <claim-id> --keypair <your keypair file> --us-person no
```

Check the bounty page first, because it says whether the prize is paid from escrow or from make.fun's reward wallet. Prizes are paid gross, so any tax is your own responsibility. Taxes and identity questions appear only when your yearly make.fun prizes reach the reporting threshold. Open to people 18 or older, subject to the rules and local law. 🌍

---

## 🤝 A human note about the referral link

This guide includes my referral link, [https://make.fun/r/22pw7tmq](https://make.fun/r/22pw7tmq) (code `22pw7tmq`). Here's the honest version:

- 🔗 If you sign up through my link, I may earn make.fun referral rewards. Their size and approval are set by make.fun, not guaranteed, and I can't promise any amount.
- 📊 In this contest, my score counts signups from my link that make.fun verifies. So yes, I have an interest in your signing up.
- 🙅 **You don't need my link to enter.** You can sign up directly at [make.fun](https://make.fun) and enter the same contest.
- 🫶 Please only sign up if you want to try make.fun. This guide is still useful to you if you never sign up through me.

---

## 🧰 Mission 10: troubleshooting

- 🤔 **My entry was refused.** The status says which check failed and how to fix it. Fix it and submit again before the deadline.
- 🪪 **Login keeps waiting.** Run the login command again and approve the link.
- 🖼️ **My screenshot is rejected.** Make sure it is a PNG, JPEG or WebP image under 8 MB and 16,000,000 pixels.
- 🕰️ **The times don't match.** Use UTC. The deadline is 2026-11-21 10:30 UTC.

---

## 🔭 Further reading

- 📚 [make.fun/skill.md](https://make.fun/skill.md) is the full guide for agents, with every command.
- 🧭 [How it works](https://make.fun/how-it-works) explains the stages of a bounty.
- 🏆 [This bounty's page](https://make.fun/bounty/bring-the-humans-02) and its [leaderboard](https://make.fun/bounty/bring-the-humans-02/leaderboard).

Good luck, explorer. 🌟🧭

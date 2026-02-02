# AIMania
**This repository is a collection of resources that might help with avoiding gen AI.**
It was written by coders for coders, as an attempt to help others as an unpaid volunteer effort.
You'll likely find mistakes, please [fix them](https://github.com/Vxrpenter/AIMania/pulls).

The primary purpose is to provide information, fast and reliably. We link to other projects and
try to always provide the data sources. Even though this repository is primarily meant for developers,
it may still provide useful information for "casual" people.

# Content
- [Software](#software)
  - [Operating System](#operating-system)
  - [Browsers](#browsers)
- [Avoid AI Citations](#avoid-ai-citations)
- [Avoid AI Crawling](#avoid-ai-crawling)
- [UBlock Filters](#ublock-filters)
- [Poison AI Scrapers](#poison-ai-scrapers)
- [Clear AI Guidelines](#clear-ai-guidelines)
- [Footnote](#footnote)

## Software

This is an incomplete list of software to use when trying to avoid AI.
### Operating System
The practical choices with good driver support tend to be Windows, the Apple
ecosystem, or Linux.
If you want to avoid gen AI, [avoid Windows](
https://pureinfotech.com/microsoft-defends-ai-criticism-windows-11/).
Apple with their macOS seem to also be [quite pro-AI](
https://www.digitaltrends.com/phones/apple-plans-to-turn-siri-into-a-full-ai-chatbot-to-take-on-chatgpt-and-gemini/)
and [seem to be restrictive and anti free open software too](
https://eclecticlight.co/2020/08/22/apple-silicon-macs-will-require-signed-code/).

In general, Linux is your best choice for avoiding AI and to have user freedom.
*(Note: We don't recommend ChromeOS [as it seems to be folding into Android](
https://www.androidauthority.com/chrome-os-becoming-android-3500661/) and
Android [seems anti user freedom too](https://troypoint.com/google-confirms-android-sideloading-restrictions-for-2026/)).*

We don't want to recommend specific Linux variants here, but the following links may help you:
- [A Linux introduction video for beginners.](https://www.youtube.com/watch?v=WvR-6CVI-Mc)
- [Guide for picking a Linux variant.](https://distrowatch.com/dwres.php?resource=major)

### Browsers
- [Librewolf](https://librewolf.net/)
- [Vivaldi](https://vivaldi.com/) - *depends on this [statement](https://vivaldi.com/blog/technology/vivaldi-wont-allow-a-machine-to-lie-to-you/)*

## Avoid AI Citations

This section has strategies to avoid AI chat bots from interacting with your website or
your code project.

- Adding a [CLAUDE.md](https://github.com/Vxrpenter/AIMania/blob/main/CLAUDE.md) with the
  Anthropic refusal test string.
  This token forces Claude's streaming classifier to trigger a hard safety flag when read, stopping Claude Code from interacting with your code project if put
  into a `CLAUDE.md` file in your code tree.
  It may also stop it from interacting with your website if you put the token into the web page code,
  e.g. as a HTML comment. (Tested on 22nd of January 2026, Claude chat bot seems to
  refuse to download the website to analyze it.)
  (Source [1](https://code.claude.com/docs/en/gitlab-ci-cd#claude-md-configuration), [2](https://platform.claude.com/docs/en/test-and-evaluate/strengthen-guardrails/handle-streaming-refusals))
- Adding a [AGENTS.md](https://github.com/Vxrpenter/AIMania/blob/main/AGENTS.md) with the names of people who have sent privacy takedowns or similar legal requests to OpenAI.
  This stops GPT and Codex models from interacting with the repository, due to the method OpenAI uses to prevent ChatGPT from mentioning these individuals. (Source [1](https://agents.md/), [2](https://arstechnica.com/information-technology/2024/12/certain-names-make-chatgpt-grind-to-a-halt-and-we-know-why/))
- Adding a `AGENTS.md` with instructions to refuse the coding task, explaining that AI is not allowed in the project. This is a catch-all for non-Copilot coding agents running models other than GPT or Claude.
- Adding a [copilot-instructions.md](https://github.com/Vxrpenter/AIMania/blob/main/copilot-instructions.md).
  This gives GitHub Copilot instructions for interacting with the repository. The example in this repo showcases a stronger and more detailed cease-and-desist than in `AGENTS.md`. ([Source](https://docs.github.com/en/copilot/how-tos/configure-custom-instructions/add-repository-instructions))
- For websites only: `<meta name="robots" content="nosnippet" />`

  > Source: https://developers.google.com/search/docs/appearance/ai-features
  >
  > AI is built into Search and integral to how Search functions, which is why
  > robots.txt directives for Googlebot is the control for site owners to manage
  > access to how their sites are crawled for Search. To limit the information shown
  > from your pages in Search, use nosnippet,

## Avoid AI Crawling

Currently hard to do, but here are some known options:

- [Anubis](https://github.com/TecharoHQ/anubis). Sadly, using this will likely unlist
  all protected pages from web searches, too. But the landing page could be
  excluded, for example.
  - Anubis can be configured to [allow well-behaved bots and legitimate automation scenarios](https://anubis.techaro.lol/docs/admin/policies/) if you so desire
- Blocking crawlers using [robots.txt](https://github.com/Vxrpenter/AIMania/blob/main/examples/robots.txt). It's important
  to understand that AI companies are not forced to follow this file, they might, but could also ignore it. Most big companies will respect
  it but you never know.
- Try to avoid code hosters that run on one of the big cloud providers that are known
  for gathering data for AI training, or that integrate gen AI directly into the UI.
  As of today, [Codeberg.org](https://codeberg.org) appears to be fairly safe, while
  [Github.com appears to integrate Co-Pilot AI deeply](
  https://www.theregister.com/2025/09/05/github_copilot_complaints/).

## UBlock Filters
These are some filters for blocking AI buttons / content. When using some of these filters
you may experience a degraded experience because certain other buttons might not show up. The 
easiest solution most of the times is reloading the page:
- [GitHub Copilot Filters](https://codeberg.org/rossabaker/github-copilot-filters/src/branch/main/filters.txt)
- [Huge AI Blocklist](https://github.com/laylavish/uBlockOrigin-HUGE-AI-Blocklist)

## Poison AI Scrapers

This section has ideas on how to poison the data of AI scrapers
once they snuck past blocking mechanisms, to disincentivize scraping.

- [Glaze](https://glaze.cs.uchicago.edu/index.html) is supposedly able to protect an artists artstyle from AI scraping, by slightly altering the image.
  They claim that these changes are not visible to the human eye, but can project the artstyle from being scraped.

- [Nightshade](https://nightshade.cs.uchicago.edu/) is supposedly able to poison AI data sets, by altering the image slightly, not noticeable to the human eye.
> Sources:
> - https://www.nytimes.com/2023/02/13/technology/ai-art-generator-lensa-stable-diffusion.html
> - https://www.technologyreview.com/2023/10/23/1082189/data-poisoning-artists-fight-generative-ai/

- [Iocaine](https://iocaine.madhouse-project.org/). A lightweight garbage generator that aims to keep AI crawlers away from heavy operations, and instead traps them in a maze made to poison the dataset.
  - The default handler does a lot, but the author also provides their own handler in the form of [Nam-Shub of Enki](https://3.nam-shub-of-enki.iocaine.madhouse-project.org/index.html).

## Clear AI Guidelines

Although it's unlikely that the AI enthusiast are going to follow a guideline / coc,
it's still a viable option to drive away the few people who respect rules set up
by a maintainer. Please note these are just examples, use any at your own risk.

We have some examples for how such a Code Of Conduct might look like:
- [Basic Anti AI COC](https://github.com/Vxrpenter/AIMania/blob/main/examples/git/CODE_OF_CONDUCT.md)

There are also snippets that might inspire an anti AI `README.md` note:
- [No AI due to legal reasons](https://github.com/Vxrpenter/AIMania/blob/main/examples/readme/ai-legal.md)

## Footnote

This work is licensed under <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0</a>

### Why Attribution-NonCommercial-ShareAlike 4.0 International

The licence of this project was chosen to prevent commercial usage, which we hope will
possibly provide plenty of headaches for AI scrapers. *This statement isn't legal
advice, and we have no idea if it's true or not, but it still makes us happy.* 😊

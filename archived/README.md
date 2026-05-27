# `ARCHIVED`
This contains archived information that has been rendered useless / unnecessary.

# Avoid AI Citations
- Adding a [CLAUDE.md](https://github.com/Vxrpenter/AIMania/blob/main/archived/CLAUDE.md) with the
  Anthropic refusal test string.
  This token forces Claude's streaming classifier to trigger a hard safety flag when read, stopping Claude Code from interacting with your code project if put
  into a `CLAUDE.md` file in your code tree.
  It may also stop it from interacting with your website if you put the token into the web page code,
  e.g. as a HTML comment. (Tested on 22nd of January 2026, Claude chat bot seems to
  refuse to download the website to analyze it.)
  (Source [1](https://code.claude.com/docs/en/gitlab-ci-cd#claude-md-configuration), [2](https://platform.claude.com/docs/en/test-and-evaluate/strengthen-guardrails/handle-streaming-refusals))

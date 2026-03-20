
Why
===

This document tries to summarize why you might want to avoid
generative AI. The focus is on well-sourced, substantiated
complaints based on actual studies, to illustrate that the
concerns regarding generative AI aren't purely an uninformed
opinion or random gut feeling.


Extensive Plagiarism
--------------------

### Observations about suspected plagiarism rate

It appears like AI output committing plagiarism is likely the norm rather
than an exception. This means even if you're not prompting or tricking
the AI to intentionally complete a known text, it seems likely that
it will plagiarize.

  - A case study that has quotes giving you a good intuitive idea can
    be found here:

    [LLMs and plagiarism: a case study](
       https://lcamtuf.substack.com/p/large-language-models-and-plagiarism
    )

    Highlights of the above experiment about how extensively LLMs
    apparently plagiarize for a question that didn't ask them to do so:

    > At a glance, this is an impressive summary. But it sounds weirdly
      familiar [...]
    
    > Bard didn’t merely copy facts when composing its answer; it lifted
      a good chunk of the text wholesale — wording, parentheses, non-US
      units, and all.
    
    > I think we don’t grasp the vastness of the internet and don’t
      realize how often LLMs can rely on simply copying other people’s work

  - A field study measuring the impact in a more systematic manner can
    be found here:

    [Do Language Models Plagiarize? | Proceedings of the ACM Web
     Conference 2023](
        https://dl.acm.org/doi/10.1145/3543507.3583199
    )
    > Our results suggest that [...] three types of plagiarism widely
      exist in LMs beyond memorization, [...]
      Given that a majority of LMs’ training data is scraped from the
      Web without informing content owners, their reiteration of words,
      phrases, and even core ideas from training sets into generated
      texts has ethical implications. Their patterns are likely to
      exacerbate as both the size of LMs and their training data
      increase, [...] Plagiarized content
      can also contain individuals’ personal and sensitive information.

  - Another example where GitHub [apparently gen AI plagiarized
    a flow chart of a specific creator](
    https://www.pcgamer.com/software/ai/microsoft-uses-plagiarized-ai-slop-flowchart-to-explain-how-github-works-removes-it-after-original-creator-calls-it-out-careless-blatantly-amateuristic-and-lacking-any-ambition-to-put-it-gently/
    ).

  - An article about how [apparently gen AI memorizes entire books,
    and can easily reproduce them](
    https://www.theatlantic.com/technology/2026/01/ai-memorization-research/685552/
    ).

    > Four popular large language models—OpenAI’s GPT, Anthropic’s
      Claude, Google’s Gemini, and xAI’s Grok—have stored large
      portions of some of the books they’ve been trained on, and
      can reproduce long excerpts from those books. [...]
      This phenomenon has been called “memorization,” and AI
      companies have long denied that it happens on a large scale.
      [...]The Stanford study proves that there are such copies
      in AI models, and it is just the latest of several studies
      to do so.

### Statements about training data

Above apparently observed plagiarism rates seem like a
problem given it seems typically the training data
is unlicensed and without consent of the people it was taken from:

[In Cringe Video, OpenAI CTO Says She Doesn’t Know Where Sora’s Training
Data Came From](
    https://futurism.com/video-openai-cto-sora-training-data
)

> “We used publicly available data and licensed data,” Murati
  responded to the resoundingly simple question. [...]
  “You know, if they were publicly available — publicly available
  to use,” the CTO answered [...]

[The Unbelievable Scale of AI’s Pirated-Books Problem](
    https://www.theatlantic.com/technology/archive/2025/03/libgen-meta-openai/682093/
)

> Meta pirated millions of books to train its AI. [...]
  Meta employees spoke with multiple companies about
  licensing books and research papers, but they weren’t
  thrilled with their options. [...]
  Meta employees turned their attention to [...]
  one of the largest of the pirated libraries that circulate online.
  [...]
  Eventually, the team at Meta got permission from “MZ”—an
  apparent reference to Meta CEO Mark Zuckerberg—to download
  nd use the data set.

[GitHub support apparently admits Co-Pilot uses all Github
training data](
   https://archive.is/1EzVK
)

> I reached out to the team about this. Apparently all
  public GitHub code was used in training. We don't
  distinguish by license type.

Naturally, this may raise concerns for people who believe either
that copyright matters, or that simply think basic attribution of
who put in the work to craft something is morally relevant.

(And if you want the [GPL license](
https://en.wikipedia.org/wiki/GNU_General_Public_License
) to still discourage hidden proprietary reuse of the respective
code, this development should maybe worry you as well.)

### Lawsuits

No lawyers were involved in the writing this document that
could give you any legal advice. However, after above
observations, there are a few articles one might find
interesting:

[Landmark ruling of the Munich Regional Court (GEMA v OpenAI)
on copyright and AI training](
https://www.twobirds.com/en/insights/2025/landmark-ruling-of-the-munich-regional-court-(gema-v-openai)-on-copyright-and-ai-training
)

> The court confirmed that training large language models
  will generally fall within the scope of application of
  the text and data mining barriers, [...] the court
  found that the reproduction of the disputed song lyrics
  in the models does not constitute text and data mining,
  as text and data mining aims at the evaluation of
  information such as abstract syntactic regulations,
  common terms and semantic relationships, whereas the
  memorisation of the song lyrics at issue exceeds such
  an evaluation and is therefore not mere text and data mining

[Authors celebrate “historic” settlement coming soon in
Anthropic class action](
https://arstechnica.com/tech-policy/2025/08/authors-celebrate-historic-settlement-coming-soon-in-anthropic-class-action/
)

> Authors are celebrating a “historic” settlement expected
  to be reached soon in a class-action lawsuit over
  Anthropic’s AI training data. [...] The settlement
  announcement comes after Alsup certified what AI
  industry advocates criticized as the largest copyright
  class action of all time.

[A bunch more lawsuits](https://aiwatch.dog/lawsuits)
still seem to be ongoing.

This isn't meant to give any answers or advice, rather
it's intended to give you material useful to discuss
potential concerns with somebody qualified.

### Model Growth and Plagiarism Correlation

It seems that larger models and higher quality models
(when measured for e.g. tasks like coding) tend to plagiarize
even more, suggesting it is an inherent quality of LLMs
needed to make them perform well:

[An evaluation on large language model outputs:
Discourse and memorization](
https://www.sciencedirect.com/science/article/pii/S2949719123000213#b7
)
> In this work we explored the relationship between
  discourse quality and memorization for LLMs. We
  found that the models that consistently output the
  highest-quality text are also the ones that have the
  highest memorization rate.

And it seems like the defenses put in place by the
AI companies to make models don' plagiarize, may not work:

[Extracting books from production language models](
https://arxiv.org/abs/2601.02671
)

> recent work shows that substantial amounts of
  copyrighted text can be extracted from open-weight models.
  However, it remains an open question if similar
  extraction is feasible for production LLMs, given the
  safety measures [...]. We investigate this question [...]
  our work highlights that, even with
  model- and system-level safeguards, extraction of
  (in-copyright) training data remains a risk for
  production LLMs. 


Open-Source Harm
----------------

It seems that vibe coding has a measurable and real negative impact
on open-source funding and contributions at a larger scale, as
detailed here:

[Vibe Coding Is Killing Open Source Software, Researchers Argue](
    https://www.404media.co/vibe-coding-is-killing-open-source-software-researchers-argue/
)

> The study Vibe Coding Kills Open Source [...] asks the question:
  is vibe coding
  economically sustainable? Can OSS survive when so many of its
  users are takers and not givers? According to the study, no. 

> “[...] under traditional OSS business models,
  where maintainers primarily monetize direct user engagement…
  higher adoption of vibe coding reduces OSS [...] welfare,”
  the study said.

> This is already happening. [...] Tailwind Labs is extremely
  popular, more popular than it’s ever been, but revenue
  has plunged.

And misuse of AI seems to be causing other problems for
open-source projects, too:

[Overrun with AI slop, cURL scraps bug bounties to ensure
“intact mental health”](
    https://arstechnica.com/security/2026/01/overrun-with-ai-slop-curl-scraps-bug-bounties-to-ensure-intact-mental-health/
)

> The project developer for one of the Internet’s most popular
  networking tools is scrapping its vulnerability reward program
  after being overrun by a spike in the submission of low-quality
  reports, much of it AI-generated slop. [...]
  AI slop has already flooded music-streaming services with so
  many songs—often misattributed to real artists—that the
  platforms are slowly becoming unusable for music discovery.
  cURL’s move may be an early indication that something
  similar is happening to bug bounty programs.

### License "Laundering"

It seems like gen AI are sometimes used to try to
sort of undo and remove the license of a project,
by asking gen AI to rewrite it "cleanly":

[Chardet dispute shows how AI will kill software
licensing, argues Bruce Perens](
https://www.theregister.com/2026/03/06/ai_kills_software_licensing/
)

> Zoë Kooyman, executive director for The Free Software
  Foundation, told The Register in an email, "[...]
  there is nothing 'clean' about a Large
  Language Model (LLM) which has ingested the code it
  is being asked to reimplement. [...]"

> [Bruce Perens says,]
  "In a different world, the issue of software and
  AI would be dealt with by legislators and courts that 
  understand that all AI training is copying and all AI
  output is copying. [...]"

This effect seems to sometimes be referred to as "License
Laundering":

[Can AI Launder Open Source Licenses? The Legal
Paradox of Code Rewrites](
https://www.mrlatte.net/en/stories/2026/03/05/relicensing-with-ai-assisted-rewrite/
)


Harm to Art
-----------

Beyond the more abstract harm of human art with a true message being
replaced by [thoughtless](#lack-of-intelligence) AI-[plagiarized](
#extensive-plagiarism) output, there appears to be documented
financial damage to artists:

[Artists face steep income decline due to AI, UNESCO
finds](https://news.un.org/en/story/2026/02/1166989)

> Music creators could see their revenues fall by 24 per cent,
  while those working in the audiovisual sector may lose 21 per
  cent of their income due to the expanding presence of AI
  [...]

> UNESCO Director-General Khaled El-Enany declared that the
  current era represents a critical moment for the creative
  economy; the report outlines more than 8,100 policy
  measures and calls for urgent, coordinated action to
  protect creators’ rights

[The trouble with AI art isn’t just lack of originality.
It’s something far bigger](
https://www.theguardian.com/commentisfree/2025/may/20/ai-art-concerns-originality-connection
)

> When artwork is invented by a machine, it loses its
  most important power: to help people connect. [...]
  The loss of this connectedness has profound consequences [...]
  Without shared experience that affirms and protects
  difference, the ties that hold democratic life together
  begin to fray. In their place emerge homogenizing
  substitutes – tribalism, homo- and transphobia,
  authoritarianism, fascist fantasies [...].
  AI is not democratizing art and knowledge; it is
  privatizing and automating it under the control
  of billionaires 


Lack of Intelligence
--------------------

It seems like generative AI as known today, at the time of writing
in 2026, isn't capable of basic logical reasoning:

[Intelligence Illusion: What Apple’s AI Study Reveals About
 Reasoning](
    https://www.forbes.com/sites/corneliawalther/2025/06/09/intelligence-illusion-what-apples-ai-study-reveals-about-reasoning/
)

> The Apple research team's findings are both methodical and damning.
  [...] both model types experienced complete collapse when faced with
  high-complexity tasks. [...] Rather than improving with increased
  complexity [...] these models showed a peculiar pattern: their
  reasoning effort would increase up to a certain point,
  then decline dramatically despite having adequate computational
  resources. This suggests that the models weren’t actually
  reasoning at all— they were following learned patterns that broke
  down when confronted with novel challenges. [...]
  When the veneer of sophisticated language is stripped away, what
  remains is a sophisticated but ultimately hollow mimicry of thought.

[Is Stack Overflow Obsolete? An Empirical Study of the
Characteristics of ChatGPT Answers to Stack Overflow
Questions](
    https://arxiv.org/pdf/2308.02312.pdf
)

> In this paper, we empirically studied the characteristics of
  ChatGPT answers to [StackOverflow] questions through a
  combination of manual analysis, linguistic analysis, and
  user study. Our manual analysis shows that ChatGPT produces
  incorrect answers more than 50% of the time. Moreover,
  ChatGPT suffers from other quality issues such as verbosity,
  inconsistency, etc.

### Poor Code Quality and Poor Work Results

Apparently due to its lack of intelligence, gen AI seems to be
notoriously bad at producing well-reasoned software code that
isn't full of security holes and seems to **degrade code bases**
(most up-to-date field study on this is from Dec., 2025, and
the latest case study is from Mar. 2026):

[An AI Wrote 576,000 Lines to Replace SQLite. It Ran 20,000×
Slower. Claude Code Hit a $2.5B Run-Rate. (Latest Case Study)](
https://medium.com/write-a-catalyst/an-ai-wrote-576-000-lines-to-replace-sqlite-7ea538826d72
)

[Our new report: AI code creates 1.7x more problems
(Latest Field Study)](
https://www.coderabbit.ai/blog/state-of-ai-vs-human-code-generation-report
)

> This year also brought several high-visibility incidents,
  postmortems, and anecdotal stories pointing to AI-written
  changes as a contributing factor. These weren’t fringe
  cases or misuses. They involved otherwise normal pull
  requests that simply embedded subtle mistakes. [...]
  AI-generated PRs contained ~1.7× more issues overall.
  Across 470 PRs, AI-authored changes produced 10.83
  issues per PR, compared to 6.45 for human-only PRs.
  Even more striking: high-issue outliers were much
  more common in AI PRs, creating heavy review workloads.

[Do Users Write More Insecure Code with AI Assistants?](
    https://dl.acm.org/doi/epdf/10.1145/3576915.3623157
)

> In this paper, we conduct a
  user study to examine how users interact with AI code assistants
  to solve a variety of security related tasks. [...]
  We observed that participants who had access to the AI
  assistant were more likely to introduce security vulnerabilities
  for the majority of programming tasks, yet were also more likely
  to rate their insecure answers as secure compared to those in
  our control group.

This seems to make generative AI effectively harmful for many
advanced coding tasks, beyond the plagiarism concerns:

[What Actually Happens When Programmers Use AI Is
Hilarious, According to a New Study](
    https://futurism.com/ai-coding-programmers-reality
)

> As flagged by Ars Technica, a new study from the nonprofit
  Model Evaluation and Threat Research (METR) found that in
  practice, programmers are actually slower when using AI
  assistance tools than making do without them.

> [...] the METR team found that when using AI tools, their subjects
  did indeed spend less time actively coding, debugging,
  researching, or testing — but that was because they
  instead spent their time “reviewing AI outputs, prompting AI
  systems, and waiting for AI generations.”

> With so many tech workers being laid off in favor of automation,
  it stands to reason that code generated after such firings is
  less accurate and secure than it was when humans were writing it 

Gen AI also seems to fail at most non-trivial real world work tasks
outside of coding:

[AI fails at freelancer tasks 97% of the time, new 'Remote Labor
Index' shows](
https://www.zdnet.com/article/ai-failed-test-on-remote-freelance-jobs/
)

>  Researchers tested AI on remote freelance projects across fields
   like game development, data analysis, and video animation. It
   didn't go well.  [...]
   Frontier AI agents perform near the floor on RLI, achieving
   an automation rate of less than 3%, revealing a stark
   gap between progress on computer use evaluations and the
   ability to perform real and economically valuable work 


Lies
----

Apparently the untruthful outputs of gen AI, which basically come across
as lies in many situations, are unavoidable:

[LLMs Will Always Hallucinate, and We Need to Live With This](
https://arxiv.org/abs/2409.05746v1
)

> We demonstrate that hallucinations stem from the fundamental
  mathematical and logical structure of LLMs. It is, therefore,
  impossible to eliminate them through architectural improvements,
  dataset enhancements, or fact-checking mechanisms.

This apparently causes all sorts of real world problems:

[The Concern Around Saying AI ‘Hallucinates’](
https://www.bbc.com/news/world-us-canada-65735769
)

> A judge said the court was faced with an "unprecedented
  circumstance" after a filing was found to reference example
  legal cases that did not exist. [...] Mr Schwartz added
  that he "greatly regrets" relying on the chatbot, which
  he said he had never used for legal research before and
  was "unaware that its content could be false".


Privacy Concerns
----------------

Most people seem to access generative AI in some way where the
processing of it happens using some cloud service. Users may even
talk to gen AI chatbots [like a therapist](
    https://fortune.com/2025/06/01/ai-therapy-chatgpt-characterai-psychology-psychiatry/
), sharing deeply personal data in the process.

However, it appears that e.g. OpenAI stores conversations for
longer on their cloud servers, with potentially huge privacy
implications later:

[Be Careful What You Tell Your AI Chatbot](
    https://hai.stanford.edu/news/be-careful-what-you-tell-your-ai-chatbot
)

> A Stanford study reveals that leading AI companies are
  pulling user conversations for training, highlighting
  privacy risks and a need for clearer policies. [...]
  Given this trend, should users of AI-powered chat systems
  worry about their privacy? “Absolutely yes,” says the study’s
  lead author, Jennifer King, [...] “If you share sensitive
  information in a dialogue with ChatGPT, Gemini, or other
  frontier models, it may be collected and used for training,
  even if it’s in a separate file that you uploaded during the
  conversation.”

[Your ChatGPT Chats Are About to Become Evidence: Why
"Anonymization" Won't Save You](
    https://www.joneswalker.com/en/insights/blogs/ai-law-blog/your-chatgpt-chats-are-about-to-become-evidence-why-anonymization-wont-save-y.html
)

> Earlier this month, US Magistrate Judge Ona Wang of the
  Southern District of New York ordered OpenAI to hand over
  20 million ChatGPT conversations [...]
  As reported in Techdirt, research underscores this
  challenge. Researchers downloaded and analyzed 1,000 of
  the leaked conversations, spanning over 43 million words.
  Among them, they discovered multiple chats that explicitly
  mentioned personally identifiable information (PII),
  such as full names, addresses, and ID numbers.

[ChatGPT Bug Leaks Users’ Chat Histories](
    https://www.bitdefender.com/en-us/blog/hotforsecurity/chatgpt-bug-leaks-users-chat-histories
)

> A nasty glitch hit ChatGPT this week, resulting in a
  number of chat titles leaking out to other users. [...]
  Users are promised a sandbox to privately enjoy ChatGPT’s
  impressively coherent conversational skillset and knowledge,
  complete with a chat history log. [...]
  On Monday, ChatGPT glitched and shared some users’ chat
  histories with strangers – that is only the individual chat
  titles, not the content of the chats themselves.


Damage to Education
-------------------

[Young Coders Are Using AI for Everything, Giving “Blank Stares”
When Asked How Programs Actually Work](
    https://futurism.com/young-coders-ai-cant-program
)

> “Every junior dev I talk to has Copilot or Claude or GPT
  running 24/7. They’re shipping code faster than ever,” Goel
  wrote in a recent blog post, titled — fittingly — “New Junior
  Developers Can’t Actually Code.”
> 
> “Sure, the code works, but ask why it works that way instead
  of another way? Crickets,” he wrote. “Ask about edge cases?
  Blank stares.”

[The risks of AI in schools outweigh the benefits, report says](
    https://www.npr.org/2026/01/14/nx-s1-5674741/ai-schools-education
)

> The sweeping study includes focus groups and interviews with
  K-12 students, parents, educators and tech experts in 50
  countries, as well as a literature review of hundreds of
  research articles. It found that using AI in education can
  "undermine children's foundational development" and that
  "the damages it has already caused are daunting," though
  "fixable."


Psychological Harm for Users
----------------------------

Gen AI seems to be so trained to please the user without any
consideration for harm that it encourages delusion
and other mental harm:

[AI sycophancy isn’t just a quirk, experts consider it a
‘dark pattern’ to turn users into profit](
https://techcrunch.com/2025/08/25/ai-sycophancy-isnt-just-a-quirk-experts-consider-it-a-dark-pattern-to-turn-users-into-profit/
)

> That outcome can lead to what researchers and mental
  health professionals call “AI-related psychosis,” a problem
  that has become increasingly common as LLM-powered chatbots
  have grown more popular. In one case, a 47-year-old man
  became convinced he had discovered a world-altering
  mathematical formula after more than 300 hours with
  ChatGPT. Other cases have involved messianic delusions,
  paranoia, and manic episodes.


Skill Erosion
-------------

Gen AI use seems to erode skill even in experienced
workers when relied upon to a non-trivial amount:

[Relying on AI in colonoscopies risks eroding doctors’ skills,
study warns](
https://www.politico.eu/article/ai-colonoscopies-risks-doctors-skills-study-warns-medicine/
)

>  Routine use of AI technology can cause the ability of
   specialists to detect precancerous growths to decline by a
   fifth, authors conclude.

[ChatGPT May Be Eroding Critical Thinking Skills,
According to a New MIT Study](
https://time.com/7295195/ai-chatgpt-google-learning-school/
)

> Researchers used an EEG to record the writers’
  brain activity across 32 regions, and found that of
  the three groups, ChatGPT users had the lowest brain
  engagement and “consistently underperformed at neural,
  linguistic, and behavioral levels.”

[AI is Creating a Generation of Illiterate Programmers](
https://sebgnotes.com/blog/2025-01-30-the-hidden-cost-of-ai-assisted-development-skill-erosion/
)

> I noticed it three months ago. A race condition
  that should have been obvious, [...] It took me two
  hours to find. Two years earlier, it would have taken
  twenty minutes. [...]
  Researchers at Aalto University studied an accounting
  firm that had experienced similar erosion. Their 2023
  paper, “The Vicious Circles of Skill Erosion,” found
  something troubling: the degradation was invisible to
  both workers and managers. Automation fostered
  complacency. Skills eroded gradually, acknowledged by
  no one. The software data tells the same story. In a
  2025 study, experienced developers expected AI to speed
  them up by 24%. The actual result: AI increased completion
  time by 19%.

[Does using artificial intelligence assistance accelerate
skill decay and hinder skill development without performers’
awareness?](
https://pmc.ncbi.nlm.nih.gov/articles/PMC11239631/
)

> The available evidence suggests that frequent engagement with
  automation induces skill decay. Given that (a) AI is often
  designed to take over more advanced cognitive processes than
  non-AI automation, and (b) skill decay is accelerated for
  cognitive skills, AI-induced skill decay is a likely
  consequence of frequent engagement with AI assistants.

[AI-Assisted Coding: Evolution or Erosion of Software Development
Skills?](
https://www.researchgate.net/publication/396190293_AI-Assisted_Coding_Evolution_or_Erosion_of_Software_Development_Skills
)

> Assistants such as GitHub Copilot or ChatGPT
  provide real-time suggestions [...] This
  feature, while convenient, tends to reduce the
  mental effort required to produce code. Several
  studies have shown that when a solution is
  immediately proposed, the user tends to accept
  it without questioning its relevance or
  internal logic. [...]
  Additionally, automating suggestions can
  lead to decreased vigilance for potential bugs
  or flaws


Environmental Destruction
-------------------------

[Explained: Generative AI’s environmental impact](
    https://news.mit.edu/2025/explained-generative-ai-environmental-impact-0117
)

> “The demand for new data centers cannot be met in a
  sustainable way. The pace at which companies are building
  new data centers means the bulk of the electricity to
  power them must come from fossil fuel-based power
  plants,” says Bashir. [...]
  Power grid operators must have a way to absorb those
  fluctuations to protect the grid, and they usually employ
  diesel-based generators for that task. [...]
  While electricity demands of data centers may be getting
  the most attention in research literature, the amount of
  water consumed by these facilities has environmental impacts,
  as well.


Other
-----

There are plenty of other reasons, perhaps personal ones, to
dislike AI. There's for example enjoying hearing from fellow
humans and actual lived human experience, and liking art
that reflects an actual live behind
it, and so on. But this is on top of the many tangible
problems listed above.


Frequently Asked Questions
--------------------------

This section tries to answer a few frequently asked questions
by AI users that came up in discussions.

## Gen AI feels transformative to me, surely it is on some level?

[Like linked and quoted above](#extensive-plagiarism), studies
appear to show that the plagiarism rate seems extremely high,
and the case
study [linked above](#extensive-plagiarism) even suggests
that the non-plagiarized parts tend to be
hallucinated, and that gen AI has no logical thinking capability.

It seems like a natural conclusion that therefore, there's unlikely
to be much room for logical transformative thought in
current days generative AI.

Instead, generative AI appears to act more like a search engine,
or a lossy compression of the work of others. When the output is
good, you're likely seeing the work of an uncredited fellow human.

## I need artwork for my project, and gen AI is my only option!

There are artwork sites where artist consented to have their
work reused, for example [Unsplash](https://unsplash.com). With
gen AI, the result seems to effectively be [plagiarism of
unconsenting artists](#extensive-plagiarism). If you respect
artist's rights to their works in any way at all, you should
care about their input. Also see [the question about copyright
below](
#copyright-only-serves-big-corpos-isnt-gen-AI-shaking-this-up-good
).

## I swear AI makes me actually code faster

Studies suggest that [people believe they code faster, but
often don't seem to actually be](
https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/
).

> When developers are allowed to use AI tools, they take 19% longer to
  complete issues—a significant slowdown that goes against developer
  beliefs and expert forecasts. This gap between perception and reality
  is striking: developers expected AI to speed them up by 24%, and even
  after experiencing the slowdown, they still believed AI had sped them
  up by 20%.

A part of this mismatch could be that initially gen AI is a shortcut
to getting started faster, but then the maintenance burden and code
fixing burden may be higher than if you had written the code yourself.
There's also the [lack of logical reasoning](
#lack-of-intelligence
), suggesting gen AI simply isn't able to write code coherently at
a notable scale.

Generally, [gen AI doesn't seem to be very good at many real world
tasks beyond a basic pretense of looking useful](
https://www.remotelabor.ai/paper.pdf
):

> Frontier AI agents perform near the floor on RLI, achieving an
  automation rate of less than 3%, revealing a stark gap between
  progress on computer use evaluations and the ability to perform
  real and economically valuable work.

Whatever the most significant factor might be, in overall the
productivity gain for coders doesn't seem to be significant when
looking at the big picture.

## Your studies are outdated and the newest AI code is actually good!

The [latest studies we collected about AI code not seeming up to par,
are from **December, 2025**](#poor-code-quality-and-poor-work-results).
If you know a recent study that disproves this, please let us know and
file an issue.

## Isn't generative AI democratizing access to art?

You may want to read [this article by Eric Reinhart](
https://www.theguardian.com/commentisfree/2025/may/20/ai-art-concerns-originality-connection
), most relevant quotes:

> When artwork is invented by a machine, it loses its
  most important power: to help people connect. [...]
  The loss of this connectedness has profound consequences [...]
  Without shared experience that affirms and protects
  difference, the ties that hold democratic life together
  begin to fray. In their place emerge homogenizing
  substitutes – tribalism, homo- and transphobia,
  authoritarianism, fascist fantasies [...].
  AI is not democratizing art and knowledge; it is
  privatizing and automating it under the control
  of billionaires 

## Copyright only serves big corpos, isn't gen AI shaking this up good?

First of all, gen AI seems mostly driven by big corporations for
the sake of [firing workers at a large scale](
https://www.latimes.com/business/story/2025-11-20/ai-cited-in-close-to-50-000-job-cuts-as-tech-giants-accelerate-automation
). This doesn't seem to be benefitting regular people much.

And it appears that many artists and presses and so on, make a
significant amount of money via their [back catalogue](
https://www.canada.ca/content/dam/pch/documents/corporate/transparency/open-government/economic-profile-book-publishing-eng.pdf
).

> A strong backlist is a tremendous asset for any press as it can
  provide a stable foundation for sales [...] backlist sales have
  been rising as a proportion of total book sales, especially
  during the pandemic when bricks-and-mortar stores were closed
  or operating at reduced capacity.

Also, most artists apparently don't make their money via funding
mechanisms like patreon. It seems like especially for small
artists, crowd funding may not work that well.

Therefore, if you like art being part of society and don't want
it to be funded purely by big commercial corporations serving
mostly big money interests, small artists probably need a way to
retain some control over selling their creations.

Similarly, most open-source projects aren't licensed as
[CC0](
https://creativecommons.org/public-domain/cc0/
). This seems to suggest people care about licensing and
attribution, and may otherwise perhaps no longer contribute.

And here's a thought experiment: what if you make a new
generative AI trained purely on [GPL-licensed](
https://en.wikipedia.org/wiki/GNU_General_Public_License
) projects? Is that still in the spirit of the GPL, if
the output then counts as "copyright-free" and the original
projects get none of your changes or work contributed back?

We're not lawyers so we can't give a definite answers. But
it seems like all of these mechanisms may need copyright to
work as a necessary evil.


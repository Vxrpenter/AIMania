
Why
===

This document tries to summarize why you might want to avoid
generative AI. The focus is on well-sourced, substantiated
complaints based on actual studies, to illustrate that the
concerns regarding generative AI aren't purely an uninformed
opinion or random gut feeling.


Extensive Plagiarism
--------------------

It appears like AI output committing plagiarism is likely the norm rather
than an exception. This means even if you're not prompting or tricking
the AI intentionally complete a known text, it seems likely that
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

This seems like a problem given it seems typically the training data
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


Lack of Intelligence
--------------------

It seems like generative AI as known today, at the time of writing
in 2026, isn't capable of basic logical reasoning:

[Intelligencec Illusion: What Apple’s AI Study Reveals About
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


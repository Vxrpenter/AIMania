
Why
===

This document tries to summarize why you might want to avoid
generative AI. The focus is on well-sourced, substantiated
complaints based on actual studies, to illustrate that the
concerns regarding generative AI aren't purely an uninformed
opinion or random gut feeling.


Extensive Plagiarism
--------------------

It appears like plagiarism of AI output is likely the norm rather than
an exception. This means even if you're not prompting or tricking
the AI intentionally complete a known text, it seems likely that
it will plagiarize.

  - A case study that has quotes giving you a good intuitive idea can
    be found here:

    [LLMs and plagiarism: a case study](
       https://lcamtuf.substack.com/p/large-language-models-and-plagiarism
    )

    Highlights of the above experiment about how extensively LLMs
    apparently plagiarize for a question that didn't ask them to do so:

    > At a glance, this is an impressive summary. But it sounds weirdly familiar [...]
    
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

Naturally, this may raise concerns for people who believe either
that copyright matters, or that simply think basic attribution of
who put in the work to craft something is morally relevant.


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

Lack of Intelligence
--------------------

It seems like generative AI as known today, at the time of writing
in 2026, isn't capable of basic logical reasoning:

[Intelligencec Illusion: What Apple’s AI Study Reveals About Reasoning](
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


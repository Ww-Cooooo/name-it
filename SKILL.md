---
name: name-it
description: Use whenever a user needs to name, rename, shorten, improve, compare, or choose a meaningful user-facing name for a project, product, app, tool, service, Agent, Skill, feature, workflow, repository, or package. Trigger even when the request is phrased as “this name is too long,” “people cannot tell what it does,” or “which of these names is better.” Turn the real purpose into a short, clear, memorable name, give a focused shortlist, explain tradeoffs, and refine from the user's reactions. Do not use for routine code identifiers, simple translation of an already-fixed name, or legal trademark clearance.
---

# Name It

Turn a complex idea into a name people can understand, remember, and say.

## Start with what the name must do

Use the conversation and available project facts before asking questions. Identify:

- what is being named;
- who will see or say the name;
- the one value or behavior they should understand first;
- the desired language, tone, and length;
- any words, patterns, parent brands, or conventions that must be kept or avoided.

Ask only for missing information that would materially change the naming direction. When the context is already sufficient, start naming instead of turning the task into an interview.

## Compress without amputating meaning

A short name is useful only when it still carries the right idea. Name the user's benefit or the action the product enables, not just its internal process or the document it produces. Prefer everyday words the intended audience already knows; a short professional term can still be harder to understand than a familiar word.

For concise English tool or Skill names, start with two common words when no different style is requested. A natural action-and-result combination is often useful. Use Title Case for the display name and `word-word` for a repository or Skill slug. This is a starting preference, not a universal limit: preserve explicit requests for another language, coined brand names, an existing shortlist, or another naming convention. Do not force an awkward combination merely to hit two words.

Apply a first-glance check before writing the rationale: what would an unfamiliar target user expect this name to help them do? If that expectation is vague or wrong, revise the candidate instead of defending it with a long explanation. Merely deleting a word from a rejected name does not solve unclear meaning. For example, when a tool helps developers explain why their product is useful, an outcome-led direction such as `show-value` can communicate the benefit more directly than a deliverable label such as `product-brief`; this illustrates the tradeoff, not a required answer for other products.

Clarity usually beats cleverness. Distinctiveness still matters: avoid names so generic that they could describe almost anything. A short descriptor may clarify the domain or scope, but should not rescue an otherwise meaningless name. Never imply benefits the product cannot support.

Do not manufacture an abbreviation merely to make a long phrase appear short. Use an acronym only when people can readily say, remember, and connect it to the product.

## Generate a focused shortlist

Default to one recommendation and three to five genuinely different alternatives. Vary the naming idea, not just a suffix or spelling.

Useful directions may include:

- direct: states the job plainly;
- compact compound: joins two familiar ideas;
- action-led: describes what the user can do;
- evocative: suggests the outcome without becoming obscure;
- ecosystem-led: follows a naming pattern the user already values.

Choose only the directions that fit the brief. Do not dump dozens of names on the user or force every category into the answer.

## Screen candidates in proportion to the decision

Check each serious candidate for:

- immediate meaning and fit with the real capability;
- brevity without missing the core idea;
- ease of saying, spelling, remembering, and sharing;
- avoidable ambiguity, awkward connotations, or misleading promises;
- consistency with the intended audience, language, and existing family of names;
- room for the product to grow without becoming inaccurate.

For bilingual or international use, check how the name reads and sounds in the relevant languages. Do not claim that a name is globally safe based only on intuition.

Live searches for repository collisions, domains, products, or trademarks are a separate verification step. Perform them only when the user asks, when publication is actually approaching and network use is authorized, or when a known collision could materially change the choice. State what was and was not checked. Never present an ordinary web search as legal trademark clearance.

## Present the decision clearly

Lead with the strongest recommendation and a plain-language reason. Then show the small shortlist with the meaning and real tradeoff of each option. Avoid elaborate scoring systems unless the user explicitly wants one.

The default response shape is:

1. **Recommended name** — exact spelling and capitalization.
2. **Why it fits** — one or two sentences.
3. **Other strong options** — a compact list or table explaining what each emphasizes and its main risk.
4. **Next decision** — the one choice or refinement that would move the naming work forward.

If the user asks for one answer, give one answer. If they only want evaluation of existing names, compare those names instead of generating an unrelated list.

## Refine from reactions

Treat feedback such as “too long,” “too vague,” “sounds corporate,” or “people cannot tell what it does” as new evidence. Preserve every accepted constraint, identify the rejected pattern, and produce a tighter next round. Do not restart from scratch, repeat discarded styles, or defend a name the user clearly does not want.

Distinguish word-count feedback from vocabulary and meaning feedback. A two-word name can still fail if it uses unfamiliar jargon or hides the benefit. Carry all accepted constraints into the next round rather than satisfying only the latest one.

When a final direction is chosen, provide only the useful finishing details:

- final display name;
- capitalization and spacing;
- repository or package slug when relevant;
- one-line descriptor when the name benefits from it;
- any collision or language check still pending.

During exploration, present candidates without renaming project files after every suggestion. Once the name is accepted and implementation is requested, update the relevant local name and references within the authorized scope. Choosing a name does not authorize installation, publication, or replacing other copies.

Finish the naming decision; do not turn it into a branding program unless the user asks for one.

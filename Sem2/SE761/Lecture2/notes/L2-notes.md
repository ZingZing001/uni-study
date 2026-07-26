# SOFTENG 761 Lecture 2 — From Idea to Rationale (Rationale, Purpose, Justification; Says vs Wants vs Needs)

**Why this matters:** After this lecture you can take a three-sentence project description and work *upwards* to a high-level rationale and *downwards* to a feasibility justification — and you can tell the difference between what a client said, what they pictured, and what they actually need. Everything in Assignment 1 is drawn from this, and the says→needs journey is what eventually produces your product backlog.

**Prerequisites:** Lecture 1 (course introduction, delivered by Reza) — team formation and project allocation.

> **⚠ No slide deck exists for this lecture.** Confirmed by the user. Source hierarchy is inverted from normal: the **transcript is primary**, and the three Canvas pages under Modules 1 & 2 carry the precise wording. Where the Canvas page text and the spoken explanation differ, both are recorded below.
>
> **⚠ Transcript is auto-generated and garbles several names/terms.** These are flagged inline as `⚠ transcription uncertain`. Do not treat the garbled forms as course vocabulary.

## Concept map

```mermaid
graph TD
    D[Project description<br/>= the seed / the idea] --> Q[C06 Ask WHY first]
    Q --> R[C02 Rationale<br/>So what? + Who cares?]
    R --> P[C03 Purpose<br/>links rationale to product]
    P --> J[C04 Justification<br/>feasibility / business case]
    D --> S[C05 Says → Wants → Needs]
    S --> BL[Product backlog]
    C07[C07 Reference-product origin] --> Q
    C08[C08 Client vs product owner] --> S
    R --> C09[C09 Every word must mean something]
    R --> C10[C10 Gen AI as a drafting tool]
```

---

## [L2-C01] The pipeline: idea → rationale → purpose → justification

`priority: high`

**Cue questions**
- What is the single input you start from, and what are the three things you build from it?
- Which direction do you travel for each?

**In plain language**
You get handed a few sentences describing a project. That's a seed, not a specification. Before you build anything you go *up* from it — why does this matter at all, who benefits — and then come back *down* — can we actually do this with the people, money and time we have. The product itself sits in the middle, and you deliberately don't think about it until the top and bottom are settled.

**Precisely**
The Canvas page **"Contents of Module 1 and 2"** lists three topics: *From Idea to Rationale*, *Agile*, *Scrum and Kanban*. This lecture covers only the first — Agile and Scrum/Kanban were deferred to the following week.

The starting point is the **project description** you receive on allocation — the lecturer's terms for it: "just an idea", "one seed". His warning about its size: these are not introductory-programming one-liners ("write a program that checks whether this string is a palindrome"). From a short description you are expected to produce "a full software product which must be working and of high quality."

The three artefacts, and the direction of travel from the description:

| Artefact | Direction from description | What it establishes |
|---|---|---|
| **Rationale** | **Up** — to the bigger picture | Why the problem matters at all, and to whom |
| **Purpose** | Stays closest to the description | The relationship between the rationale and this specific product |
| **Justification** | **Down** — to resources | Whether building it is feasible; the business case |

His instruction for the exercise: "you need to go up to the rationale and go down to the justification." And on where the description itself sits: "the purpose will be the closest thing to the description that you have been given from the client."

**The rule that trips people up:** "Do not directly jump to what needs to be built." The discipline is to stay at the rationale level until convinced: "you must always think that I need to be fully convinced in order to start working on the project."

**Common traps**
- Treating the description as a requirements document. It's a seed.
- Reaching for the solution first. The whole point of the ordering is that the product is decided last, not first.

*Source: transcript 00:54–00:120 region; Canvas page "Contents of Module 1 and 2"*

---

## [L2-C02] Rationale — "So what?" and "Who cares?"

`priority: high` — this is the entire content of Assignment 1.

**Cue questions**
- Define rationale in one sentence. What two questions generate it?
- State the three formal constraints on high-level rationale bullet points.
- Why is mentioning the product a failure here, not just a stylistic preference?

**In plain language**
The rationale is the answer to "why is this worth anyone's time?" — and it has nothing to do with your software. You build it by asking two things repeatedly: *so what* (why does this matter, what changes) and *who cares* (who is actually affected). Then you arrange the answers in a ladder, widest concern at the top, narrowest at the bottom, each rung resting on the one above.

**Precisely**
The lecturer's definition: "a kind of way to get to the root of the things… you want a reason for it… You must have a goal or a motivation. Then only you will be encouraged to put more effort into it."

The Canvas page's formal wording: *"The rationale explains the broader context and underlying need that gives rise to the project."*

**The two generating questions:**

1. **"So what?"** — "What difference is it going to make? Why is it important to build this project?"
2. **"Who cares?"** — "If this software project is done, if it is completed, this product is built, who is this going to help or affect?" Candidate answers he listed: environment, people, community, an industry. His framing: "who are going to be the ultimate beneficiaries, real beneficiaries of this product."

Note: "the who-cares elements and the so-what elements can be placed at any position in the [list]… there is no definite place or position for these two." So don't try to segregate them.

**Three constraints on the bullet points:**

1. **No mention of the product or solution.** Stated twice and emphatically: "none of the points must talk about the product. It must only be about the rationale."
2. **Flow from high level to low level, each point feeding the next.** "It is very important that the rationale flows well from high level to low level. And each bullet point is connected to each other… the previous bullet point is feeding into the next one."
3. **One sentence per bullet point**, roughly one line each.

**Worked example — the ice-cap project**
Description: a system that monitors the speed of ice-cap melting (sensors + data analysis).

The ladder he built by asking why:
- the planet → climate change
- global warming as a cause of climate change
- communities / human beings / life in general
- …descending toward the specific concern

His estimate of length: "there might be like 8 to 10 bullet points starting from the climate change and global warming."

**Worked example — the rationale the lecturer read out**
Highest level: *"technology is becoming increasingly pervasive in many aspects of society."*
Lowest level: *"it is therefore important to build people's confidence in engaging with technology to improve their way of life."*

His point about it: he deliberately never revealed the product description. "We are getting from the highest level rationale to this low level rationale **without touching the product description**." The underlying product might have been something helping non-technical people engage with technology — but you cannot tell from the rationale, and that's the proof it was written correctly.

> **⚠ transcription uncertain.** The auto-transcript calls these *"speed rationales"* — "these are known as speed rationales for a reason that you do not need to refer to too much evidence." Given the context (fast, low-evidence, from current knowledge only), the intended term is plausibly "speed rationales", but "seed rationales" would also fit the "one seed" framing used earlier. **Confirm the actual term before using it in writing.**

**Common traps**
- Sneaking the product in ("this app will help…"). Automatic failure against constraint 1.
- Writing a paragraph per point instead of a sentence.
- Producing a flat list of unrelated worthy statements. The connectedness is explicitly assessed.

*Source: transcript — rationale section; Canvas page "Example: Project Rationale, Purpose and Justification"*

---

## [L2-C03] Purpose — the link between rationale and product

`priority: high`

**Cue questions**
- What relationship does purpose assert, and between which two things?
- Why can't the purpose claim to solve the high-level problem?

**In plain language**
The rationale says the world has a big problem. Your product is small. The purpose is the honest sentence connecting them — it says what this particular thing contributes, without pretending it fixes the whole thing.

**Precisely**
Canvas page wording: *"The purpose describes the specific goal or intent of the project within that larger context."*

The lecturer's framing is about *relationship*: "the relation between that why and that product that the client is asking you to build — they must have a relationship. It is very important that they have a relationship which you can present as a purpose."

**The proportionality constraint — this is the interesting part.** Using the ice-melting example: "You cannot say that by building that product, I will be able to solve the global warming problem. It can contribute a little bit to that problem." And generally: the purpose is "just that little bit, a very minute bit of the overall solution that you might be targeting in future, or humanity might be targeting in future."

He also reframes the rationale to make the relationship clearer: since the rationale never touches the product, "you can call it a bigger picture of the problem or the bigger picture of the domain."

**Locating it:** purpose is the artefact nearest the client's own description. "When you read your allocated project description, you are basically looking at the purpose rather than the other two."

**Worked example (Canvas page)**
*"The purpose of this project is to develop a mobile application that enables individuals and small businesses to share surplus food with nearby community members in real-time, thereby reducing food waste and supporting local food security."*

Note the structure: **what is built** (mobile application, real-time sharing) + **what it contributes to** (reducing waste, supporting food security) — and it claims contribution, not solution.

**Common traps**
- Overclaiming. "This app will solve food insecurity" fails the proportionality constraint.
- Collapsing purpose into rationale. Rationale must not mention the product; purpose must.

*Source: transcript — purpose section; Canvas page "Example: Project Rationale, Purpose and Justification"*

---

## [L2-C04] Justification — feasibility, and the business case

**Cue questions**
- What is justification assessed *against*? Name the other name for it.
- What kind of external evidence counts?

**In plain language**
Deciding a project is worth doing and deciding you can actually do it are two different judgements. Justification is the second one: given this team, this budget, this deadline, is building it realistic — and is there any evidence it'll work?

**Precisely**
The lecturer's separation is explicit: "deciding about the rationale of the project and the purpose of the project is a separate thing. And then justifying it against the resources that are available to you is a different thing."

**Assessed against:** team size and capability, budget, time, "all the other resources you need to consider **in communication with the client**." The verdict it produces: "whether building that project is feasible or not."

**Alternative name — worth memorising:** "this is also known as **business case** for the project."

Canvas page wording: *"The justification supports why this solution is feasible and valuable, often referring to evidence, demand, or practicality."*

**Evidence from comparable products counts.** "A justification can relate to existing applications as well, because the solution has worked for other competitors, a similar solution might work for them as well."

**Worked example (Canvas page)**
*"Similar community-sharing apps have seen success in other regions, and early feedback from local stakeholders suggests strong interest and willingness to participate. A mobile app is accessible, scalable, and cost-effective, making it a practical tool for addressing food waste and hunger in the local area."*

Three evidence types stacked here: comparable-product precedent, stakeholder demand signal, and practicality of the delivery mechanism.

*Source: transcript — justification section; Canvas page "Example: Project Rationale, Purpose and Justification"*

---

## [L2-C05] Says vs Wants vs Needs

`priority: high`

**Cue questions**
- Define all three. Which one is quoted verbatim, and which one survives contact with constraints?
- What does the endpoint of the journey become, in Scrum terms?
- When do the three collapse into one?

**In plain language**
What a client tells you, what they're picturing while they tell you, and what would actually solve their problem are three different things. Your job is to travel from the first to the third. You do it by asking questions — the client is not withholding, they just haven't articulated it, possibly not even to themselves.

**Precisely**
Canvas page framing: *"It's common for what a client says, wants, and needs to differ due to unclear communication, evolving understanding, or unspoken assumptions."*

| Stage | What it is | How you get it |
|---|---|---|
| **Says** | The literal words / the project description. Vague, quotable, under-specified. | Handed to you |
| **Wants** | Their initial expectation — what they're picturing but haven't stated. | Discussion and questions |
| **Needs** | The real business requirement, once resources, cost and limitations are applied. | Analysis after discussion |

The lecturer's underlying claim: "we all are human beings, and what we say might not reflect what we actually want."

**Worked example (Canvas page — fitness studio booking system)**

- **Says:** *"We need a calendar where users can book a class with one click."* — "This sounds straightforward, but lacks detail."
- **Wants:** a visually appealing calendar showing available slots with instant booking; they imagine Google Calendar integration, mobile responsiveness, drag-and-drop. *"But they haven't explained this fully."*
- **Needs:** view upcoming classes, check availability, book/reserve, receive confirmation — **plus** managing class capacity, preventing double bookings, payment integration, last-minute cancellations and waitlisting.

Note what happened between wants and needs: the decorative expectations (drag-and-drop, visual appeal) dropped away, and four operational requirements the client never mentioned appeared. That asymmetry is the point of the concept.

**Worked example (spoken — the transport analogy)**
Client says they want to fly to their office. They may be picturing a personal aircraft. You establish the office is nearby — the actual need is a bike. "You might end up convincing them."
> ⚠ transcription uncertain: the transcript renders the middle term as "a R", most likely "a car". The structure of the analogy is clear regardless.

**Where the journey ends — the Scrum link:** "it is a journey from what the client says, which you have as a description of your project, to what they actually need, **which you will have as a list of, or a set of, product backlog in Scrum**. So you start with says and then get to product backlog, which is the actual needs."

**When the three collapse:** "if the client is technical enough, what they say and what they want could be overlapping, could be same. Similarly, what they want and what they need could be the same." But the discussions still happen — you confirm rather than assume.

**Four more examples walked through from the Canvas quiz** (the lecturer read these aloud from the quiz page):

1. Describing a solution in vague terms without specifying actual requirements → **says**
2. "I initially request a dashboard with real-time metrics" (quoted), but through discussion it emerges they envision an interactive, customisable analytics platform → **says vs wants**
3. Actual business requirement is to improve decision-making through accurate data visualisation, regardless of the UI complexity initially described → **needs**
4. Client insists on a fully custom-built CRM; analysis reveals the underlying need → **wants vs needs**
5. Client requests a mobile app; user research reveals the need → **wants vs needs**

**Diagnostic heuristic from the lecture:** if it's in quotation marks or is a description, it's *says*. If it's what they "envision" or "imagine", it's *wants*. If it emerges from analysis or research, it's *needs*.

**Common traps**
- Treating *wants* as the target. It's the midpoint, not the destination.
- Assuming a vague statement means the client doesn't know what they want. Usually they do — they haven't said it.

*Source: transcript — says/wants/needs section; Canvas page "Decoding what a client says vs wants vs needs"*

---

## [L2-C06] Ask "Why?" first — and do your homework before the meeting

**Cue questions**
- What is "the first core question", and what are its *two* benefits?
- What must exist before you walk into the first client meeting?

**In plain language**
Before meeting the client you sit down with the description and write out the questions you're going to ask. The first one is always some form of "why?". It feels rude. It isn't — it also makes you look invested.

**Precisely**
The questions to ask in the first meeting: **"Why? Why does this matter? And who are going to be the affected parties? Who are going to be the stakeholders, who are going to be the users?"**

**The dual benefit — both halves matter:** asking why "is not only going to give you more details about the project, it is also going to give an impression to the client that you are more interested in developing the project. So they will be happy."

He acknowledges the social discomfort directly: "sometimes you might feel that it doesn't look good if someone is asking me to do something and I'm saying why? Why? Why do you want to do this? But that is the first core question."

**The homework, done before meeting:**
- Take the description and infer a candidate rationale from it, and **write it down**.
- This initial write-up is what Assignment 1 requires.
- Explicitly **no research at this stage**: "this is going to be a very general project rationale for which we do not want you to do any research… must be based just on your current knowledge and your discussions within your team."
- Produce a **sequence of questions** for the client: "the first foremost important aspect of project development is doing your homework and writing a sequence of questions that you want to ask the client."

Other things to establish with the client: what functionalities are needed; whether specific technologies are expected.

**The analogy he used:** teaching. "This is the core principle of learning as well. In a class, if the students do not ask questions, they won't learn… So now you are on the other side. You need to ask questions to the client and bring out more knowledge."

*Source: transcript — questioning section*

---

## [L2-C07] Descriptions often come from a reference product — and the technology conflict that follows

**Cue questions**
- Where do non-technical clients' descriptions typically originate, and what question exposes it?
- Describe the conflict this creates and what you do about it.

**In plain language**
A non-technical client usually isn't inventing their description from nothing — they've seen a competitor's product, or a colleague's, and they're describing that. Which means they may also have inherited that product's technology choices, and those choices may be wrong for what they're actually asking you to build.

**Precisely**
Origin: "generally the description that the client has built, it is coming from a reference software product they have seen somewhere, or some other colleague, their colleague or their competitor, use. So they have written their description just based on that reference."

**The question that surfaces it:** *"Is this description your own idea, or is it coming from somewhere else?"* Rationale for asking plainly: "the more transparent you are, the more correct information you will get."

**The conflict.** The client may report both a set of core functionalities and a technology stack (inherited from the reference product). "You might end up at a stage where you see that the answer to the first two questions is conflicting, because in your team's experience the technologies that the client has suggested do not work well to implement those functionalities."

**What you do:** raise it. "You will have to counter-question, or put this forward to the client" — that the suggested technologies are not the best for implementing those core functionalities. He offers this as the concrete payoff of questioning: "that is the importance of asking questions."

**Note on this course's projects:** the clients are "mostly non-technical" (attributed to Lecture 1), which makes this the expected case rather than the edge case.

*Source: transcript — client questioning section*

---

## [L2-C08] Client, product owner, and user

**Cue questions**
- What does a product owner do, and how does that differ from the client in the general case?
- What's the arrangement in this course's projects?

**In plain language**
In industry the client pays, the user uses, and the product owner is the person representing them to your team day to day. On these course projects those roles land on the same person.

**Precisely**
- **Client / customer:** in the real world, generally also the actual user of the product.
- **Product owner:** "generally a representative of the client that will be handling, or kind of monitoring, the project development… building that communication between the client and the team."
- **In this course:** "your product owner and clients are the same."

Flagged as preliminary — full Agile/Scrum terminology was deferred to the following week.

*Source: transcript — Q&A after says/wants/needs*

---

## [L2-C09] Every word you write must have a meaning clear in your mind

**Cue questions**
- What test does the lecturer apply to words like "scalable"?

**In plain language**
Words like *accessible*, *scalable*, *cost-effective* slide into a justification because they sound professional. If you can't say what each one means for this specific project, you haven't justified anything — you've decorated.

**Precisely**
"When you write these things, it is very important that the words that you are putting in here, each and every word, has a meaning clear in your mind."

His worked instances, from the food-sharing justification:
- **accessible** — "accessible to everyone"
- **scalable** — "something that can scale in future if there are more users"
- **cost-effective** — stated as a distinct claim requiring its own grounding

**Common traps**
- Importing the vocabulary of the example without importing the reasoning.

*Source: transcript — justification section*

---

## [L2-C10] Using Gen AI to draft a rationale — the iteration, and the ownership rule

**Cue questions**
- What was wrong with the first AI output, and what sequence of corrections fixed it?
- What is the ownership rule?

**In plain language**
The lecturer pasted a project description into ChatGPT and asked for a rationale, then spent several rounds correcting it. The interesting part isn't that AI helps — it's that each correction he had to make is exactly one of the rules from C02. The failures are a checklist.

**Precisely**
Demo project: beehive CO₂ / behavioural monitoring — chosen deliberately "because it has a limited description. So that means you have more scope for working on getting to a rationale."

**First output** began "Honeybee populations play a vital role in global ecosystems and agriculture through pollination…". His three faults with it:
1. Not in bullet points
2. Not one-liners
3. **Talking about the project / product / solution** — the C02 violation

**The correction sequence, in order:**

| Round | Instruction given | Rule it enforces |
|---|---|---|
| 1 | "Rationale should be based on bigger picture vision only — what impacts it has on the global scale or local community level" | Brings in *so what* and *who cares* (C02) |
| 2 | "Do not focus on the implementation detail" | Removes solution content |
| 3 | Convert to bullet points | Format constraint |
| 4 | Remove any points about the project | Still leaked after round 2 — "although you mentioned about implementation, it did not get to the implementation, but still is talking about the project" |
| 5 | Ensure a proper flow between points | Connectedness constraint (C02) |

**The outcome that demonstrates the point.** Before the flow correction, the list started at "pollinators like bees are vital". After it, the top rung became *"a healthy planet depends on stability of ecosystems and biodiversity"* — "it went one level up as well. Earlier it was starting from honeybees." So enforcing flow forced the ladder to find its true top.

**Why he showed the slow version:** "this is to let you understand that if you do it without the use of [Gen AI], what process or flow of thoughts you need to consider" — going from a higher level and then reducing detail into more concise points. The prompt sequence *is* the manual method.

**The ownership rule** (attributed to Reza in Lecture 1): "if you decide to use AI, you need to own what you submit. Even though it has come from an AI, you need to own it… you cannot say that [Gen] AI gave me this and hence hands off." Operationally: "once you get that list, you need to read it fully and justify it in your own mind."

*Source: transcript — Gen AI demo section. Assignment marking treatment of AI use is in `context/admin-and-dates.md`.*

---

## Summary — the 6 things that matter from this lecture

1. **The description is a seed, not a spec.** Go *up* to rationale, *down* to justification; the product is decided last.
2. **Rationale = "So what?" + "Who cares?"**, laddered high→low with each point feeding the next, and **never mentioning the product**.
3. **Purpose links rationale to product, proportionally** — it claims a contribution, not a solution. It's the artefact closest to the client's own description.
4. **Justification = feasibility against resources**, also called the **business case**; comparable products count as evidence.
5. **Says → Wants → Needs.** Says is quoted and vague; wants is what they picture; needs survives constraints. The endpoint becomes the **product backlog**.
6. **"Why?" is the first question**, and it does double duty — it extracts detail *and* signals investment.

---

## Self-test

1. You receive a four-sentence project description. Name the three artefacts you build from it and the direction of travel for each.
2. What two questions generate a rationale? Give the constraint that most commonly gets violated.
3. Write a top-of-ladder rationale point for a project monitoring air quality in schools — then explain how you'd check it's genuinely top-of-ladder.
4. A teammate's rationale bullet reads: "This app will allow parents to view real-time pollution data." Two things are wrong with it. Name both.
5. Why can't the purpose of the ice-melting monitoring system be "to solve global warming"? Name the constraint.
6. Distinguish justification from purpose. What is justification's other name?
7. A client says: "We need a dashboard with real-time metrics." Classify that statement. Then describe what you'd expect the *wants* and *needs* stages to add or remove.
8. In the fitness-studio example, four requirements appear at the *needs* stage that the client never mentioned. Why does that asymmetry matter for how you run a client meeting?
9. Under what condition do says, wants and needs coincide — and what do you still do?
10. Your client is non-technical and has specified both a feature set and a technology stack. Where did the stack probably come from, and what do you do if it's a poor fit?
11. The lecturer's AI-generated rationale had to be corrected five times. List the corrections and map each to a rule about rationale.
12. Enforcing "proper flow" changed the top of the AI's list from honeybees to a healthy planet. What does that tell you about how to check your own ladder?

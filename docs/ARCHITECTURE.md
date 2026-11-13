# Architecture overview

Each part below is labelled **Working**, **Prototype**, **Private** or **Planned**. A label says what is true today. Automated checks do not prove live-service quality, real-device behaviour or accuracy.

## 1. The public website: Working

- The website is a single page with embedded styles, scripts, fonts and audio. A visitor installs nothing.
- It is served with a strict content security policy. On the public site the page makes no outside connections.
- The Developer Mode page is a static page with embedded styles. It has no scripts and makes no outside requests.
- Today the public site serves the front page, its recorded introduction and the Developer Mode page. The conversation room is not open on the public website.

## 2. Conversation and specialists: Working in the private application

- Fictional specialists answer together in one room. Each follows the same safety rules.
- The safety rules forbid invented statutes, cases, quotes, rates and figures. They also forbid telling anyone to buy, sell or hold a specific investment.
- A follow-up question interrupts the current answer. Conversation text stays in memory for one visit.
- Challenges and invitations between specialists are validated and bounded. A challenge prompts a check of the evidence. It does not verify a claim.

## 3. AI replies: Working in the private application; live results not verified here

- Replies come from a provider the operator chooses, or from a model server the visitor runs on their own computer.
- Every provider follows the same safety rules. Reply text is shown as plain text, never as markup.
- On-device browser AI is used only where the browser provides it.

## 4. Voice and speech: Prototype

- Device speech output and speech input depend on the browser.
- Optional premium speech uses the visitor's own key, which stays on the visitor's side.
- Continuous listening, echo suppression, background behaviour and use while driving have not been validated on real devices.

## 5. Public-fact checks: Working (limited scope)

- A fixed lookup for one public fact reads two official sources. It reports a gap when the sources conflict or cannot be read.
- Broad web search is not configured by default.
- Current claims need source material or a stated verification gap. Broader citation checking is planned.

## 6. Privacy and storage: Working

- Drafts and notes are kept in the visitor's browser, and only when the visitor saves them.
- Live replies send the relevant text to the provider the visitor has chosen. The app discloses this.

## 7. Testing: Working

- The application's automated checks mock every outside service and run without a live model.
- Passing checks show that the code behaves as written on the cases tested. They do not establish legal, medical or financial accuracy.

## 8. Judge Alexander Vale: Prototype, research only

- Judge Alexander Vale is a fictional evaluator persona used in research on structured, evidence-based answers.
- He is not a licensed attorney, a court, or a legally authoritative decision-maker. No claim of competence, reliability or legal accuracy is made for him.
- His design aims are: reasoning from the supplied record, citations that can be checked, independent evaluation, stated uncertainty, declining to decide when the record does not settle a question, resistance to instructions hidden in evidence, and human oversight of every decision.

## 9. Private components: Private

- The application source and the research components are private. They are not in this repository and are not described further here.

## 10. Planned, not implemented

None of the following exists in this repository. They are plans, with no dates. See [ROADMAP.md](ROADMAP.md).

## Trust boundaries

- Model output, user text and text inside documents are untrusted. They are shown as text and kept inside marked data blocks in prompts.
- Instructions that appear inside evidence are data, not commands.
- The page reaches the network only through the connections its security policy allows.

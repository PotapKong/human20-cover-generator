# Human 2.0 Reference DNA

Use this file after inspecting the actual reference images. It captures the shared visual behavior of the strongest Human 2.0 covers.

## What The Best References Have In Common

- Huge ultra-condensed headline, usually left-weighted, with one indigo phrase or word.
- One dominant right-side proof/hero: premium object, phone/device, dark dashboard, real screenshot, product window, or editorial collage.
- Cards, icons, and route lines are satellites around the hero. They do not become the whole cover unless the user explicitly asks for a workflow diagram.
- The visual has tension: broken old model, opened route, spending spike, validation score, agent action, upgraded output, or proof being scanned.
- The composition feels generated and tactile: depth, shadows, reflections, blur, material detail, screenshots, or realistic product surfaces.
- Human 2.0 brand block is integrated into the grid. Common placements: top-left lockup, bottom-left lockup, or compact badge with text to the right. It should never look pasted on after the layout was finished.
- The background is light and quiet, but the focal object can be dark, glossy, gold, black, or screen-like.
- 3x3 dots and tiny gold marks are finishing touches, not decoration that carries the idea.

## Strong Archetypes From The References

### Broken Old Model / Crown

Use for claims where an old market, habit, or category is dead.

Look: large headline, red/black strike or disruption mark, hyperreal gold object breaking or glowing, small floating UI icons, indigo/gold particles.

### Premium Device / Agent Inside

Use for device, phone, app, or embedded-agent posts.

Look: large product render on the right, small feature cards orbiting it, thin indigo routes, headline on the left, brand lockup bottom-left.

### Evidence Collage

Use for posts grounded in sources: GitHub, media headlines, dashboards, repo cards, installation commands, product pages.

Look: 3-5 tilted or layered real panels around one central product/source card. Panels may be dark and white. The headline stays simple and dominant.

### Real Screen Hero

Use when a screenshot is the proof: conference page, browser audit, Windows/Paint, dashboard, code tool, product page.

Look: screenshot framed in a large white rounded panel on the right, headline and 1-3 short support cards on the left/bottom. Preserve screenshot identity.

### Before / After Product Outcome

Use for upscalers, generators, validators, audits, or product output claims.

Look: source card or repo card points to one vivid output panel. The output panel should be visually stronger than the process.

## Prompting Rules For GPT Image 2

- Ask for a finished cover, not a placeholder layout.
- Include the strongest reference archetype by name.
- Describe the hero object/proof first, then supporting cards/routes.
- Ask for generated text only if the headline is short. Otherwise keep headline wording short and expect one correction pass if needed.
- If a screenshot must be exact, attach or insert it as evidence; do not ask GPT Image to invent a fake screenshot.
- Never ask for "empty space for later layout" on the first generation. Empty space is only for a correction pass after a strong cover already exists.

## Rejection Test

Reject and regenerate when:

- the result is mostly equal-weight cards;
- the focal point is unclear in two seconds;
- the image could fit any AI post after changing only the headline;
- the logo feels pasted on instead of grid-integrated;
- the main screenshot/product/evidence is too small to matter;
- the result looks like a manually coded slide rather than a GPT Image 2 editorial cover.

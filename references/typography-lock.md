# Human 2.0 Typography Lock

Use this reference before every Dzen / Telegram / horizontal Human 2.0 cover when a supplied or bundled reference shows the current poster headline style.

## Current Reference Font Class

The current Human 2.0 cover references use a heavy condensed poster grotesk, not an ultra-stretched or needle-thin face.

Target traits:

- bold condensed Cyrillic display letters;
- tall compact forms, but natural proportions;
- hard vertical strokes and minimal roundness;
- tight line height;
- strong black / indigo word contrast;
- enough letter width for thumbnail readability.

Avoid:

- ultra-condensed vertical-bar letters;
- vertically stretched glyphs;
- words that look 1.5x taller than the reference;
- Arial Narrow / Impact-like fallback unless manually checked against the reference;
- Geologica / Onest / Inter for the main headline when reference typography is supplied.

## Proportion Rules

When the user supplies typography references, treat them as the quality bar.

- Match the apparent headline width/height ratio from the reference before matching any generic "ultra-condensed" label.
- Keep the headline block close to the reference rhythm: large all-caps lines, tight but readable leading, and generous left padding.
- If a generated headline looks more than about 1.25x taller/narrower than the supplied reference, reject it.
- If the user says the font is too stretched, regenerate or correct with a face about 1.5x less vertically stretched.
- Use one indigo accent line or phrase; do not scatter accent color across many words.

## Layout Traits From The Current References

The supplied poster references show:

- headline anchored left, with a calm light-gray/white field around it;
- 3-4 strong lines, not one huge squeezed word;
- black first lines and one indigo final/accent line;
- consistent left edge and strong top/left margins;
- no tiny subtitle unless the composition has clear space below the headline.

For a two-line headline, preserve the same feel by making each line broad and readable rather than taller and narrower.

## Prompt Wording

Use wording like:

`Main headline typography must match the supplied Human 2.0 reference: heavy condensed poster grotesk with natural Cyrillic proportions. Do not use ultra-condensed vertical-bar letters. Do not vertically stretch the text. The headline should be about 1.5x less stretched than the rejected version and close to the reference width/height rhythm.`

## Quality Gate

Before finalizing:

- Compare the headline against the closest typography reference, not only against the prompt.
- Reject if the generated letters are too narrow, too tall, too soft, too rounded, or too generic.
- Reject if the headline block feels like a stretched font rather than a real display typeface.
- Reject if the headline crowds the left edge more than the reference or loses the reference's line rhythm.

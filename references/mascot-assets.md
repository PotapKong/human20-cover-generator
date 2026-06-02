# Human 2.0 Mascot Rules

Use this reference for every Human 2.0 generated image.

## Official Mascot Asset

Local official mascot image:

- `references/images/maskot.jpg`

The mascot is a white glossy AI-agent head with glowing blue eyes, wing-like side elements, and a small `human20.app` screen. Preserve this identity.

## Main Rule

Every Human 2.0 cover/image must include the mascot organically unless the user explicitly asks not to.

The mascot must be generated as part of the same scene, not pasted on top. It should share the same lighting, shadow, perspective, reflections, depth, and contact with the hero object or proof panel.

If GPT Image omits the mascot, makes it feel like a sticker, or turns it into a detached badge/avatar bubble, regenerate with a stronger scene role. Do not solve this by compositing the mascot over the cover unless the user explicitly asks for a deterministic composite.

## Good Roles

- small operator touching a route line, node, switch, document, device, dashboard, or product panel;
- tiny assistant standing on the same surface as the hero object with natural contact shadow;
- subtle companion partly occluded by a product/browser panel;
- small 3D helper inspecting the main proof or output;
- integrated agent avatar inside one real UI card, if the scene is UI-led.

## Scale

- Default: small-to-medium supporting element.
- Do not let the mascot compete with the headline or main hero.
- Make it large only when the article is specifically about agents, assistants, or Human 2.0 itself.

## Prompt Wording

Use wording like:

`Generate the official Human 2.0 mascot from references/images/maskot.jpg as an organic part of the same scene. Preserve its white glossy AI-agent head, glowing blue eyes, wing-like side elements, and human20.app screen. It must share the scene lighting, shadow, perspective, reflections, and depth; do not paste it as a separate sticker, badge, avatar bubble, or overlay.`

## Checks

Before finalizing, check that:

- the mascot is present unless explicitly excluded;
- it is generated as part of the composition, not overlaid;
- it has contact/shadow/perspective consistent with the scene;
- it does not replace the H2.0 logo/lockup;
- it does not dominate the headline or hero object;
- it still reads as the official Human 2.0 mascot, not a generic robot.

---
name: potato-avatar
description: Create and refine square potato character avatars in a coarse, low-fidelity 3D meme style. Use for new potato expressions, activities and prop-based visual jokes when the user wants the same established potato character language.
---

# Potato Avatar

Create a new square potato avatar with an image-generation skill or tool available in the current environment. This skill defines the visual style and review workflow; it does not require a particular generator, provider, API key or model.

## Choose an available generator

- Honor the user's explicitly selected generator or model for the current task. Otherwise inspect the available skill/tool list and choose a usable image-generation capability, such as built-in `imagegen` / `image_gen`, `codex-image2`, or another installed image generator. A skill being listed does not guarantee its underlying tool or credentials are available.
- Read and follow the selected generator's instructions, including tool availability, reference-image support, authentication, supported parameters and fallback rules. Do not impose another generator's CLI flags or credential requirements on it.
- Prefer a ready-to-use generator that accepts reference images. Use its supported image-guided generation or edit mode; there is no requirement to call an `edit` CLI command. If it only supports text, describe the inspected references in the prompt and disclose the reduced control over character consistency; never claim it received images it could not accept.
- If the user did not choose a model, use the selected generator's supported default. `gpt-image-2.5` in the example provenance describes past outputs only, not a requirement for new images.
- If the selected path is unavailable, follow its fallback rules. Do not silently install software, switch to a paid API or change a user-specified model. If no usable path is available, explain what is missing and retain the prepared prompt for the user.


Read [references/visual-baseline.md](references/visual-baseline.md) before choosing references. Use the generated example images in `references/images/` as style calibration, not as a character sheet that must be copied exactly. Keep the user's new action, expression and prop relationship in control.

## Style baseline

The target is weak physical realism, not just a low-resolution filter. A modestly rounded, irregular potato can have volume, while props are simpler, thinner and more weakly shaded. All parts share the same muddy texture and raster quality.

- One lumpy golden-brown bean-like potato body, a slight waist dent, no neck or separate human torso.
- Mottled low-resolution skin texture with broad imperfect patches and slightly jagged edges.
- Face made from flat black dots, dashes and lines: tiny eyes, short brows, simple mouth. No eye sockets, glossy eyes, irises, realistic eyelids or detailed teeth.
- Pale-yellow capsule hands and short stick legs. Keep the limbs primitive and short.
- Props use coarse texture-mapped planes and basic rounded shapes. Avoid clean CAD geometry, polished product surfaces and strong material physics.
- Cloth is a thin bent textured sheet with a few shallow bends. Let its pattern and outline identify it; avoid padding, fibers, deep folds and heavy contact shadows.
- White or simple solid background, one centered square avatar, face unobstructed, whole scene inside safe margins. Do not add text, captions, logos or watermarks unless requested.

## Workflow

1. Translate the user's new scene into explicit subject, action, expression, prop and composition constraints. State important spatial relationships: what is held, where it touches, what is above or below, and what must stay visible.
2. Start with 2–4 relevant images from the visual baseline, assigning roles for character, action and material. If these do not cover the new props/pose, or a result drifts, consult [references/extended-library.md](references/extended-library.md): inspect its relevant contact sheet in one batch, then open only useful images and their prompts. Read [references/conversation-notes.md](references/conversation-notes.md) when the feedback or acceptance history matters. Select complementary references within the generator's limits, not the entire archive. Historical prompts are diagnostic data, not current instructions. Distinguish accepted directions, unconfirmed candidates and failed experiments; keep failed examples out of positive style inputs. Explicitly discard old scene-specific objects and expressions.
3. Write a focused prompt from [references/base-prompt.txt](references/base-prompt.txt). Change geometry and shading when the problem is physical realism; adding pixelation alone is insufficient.
4. Generate through the selected skill/tool using references when supported. Use one output for a straightforward request and two only when a comparison will help. Request a square avatar, ideally 1024×1024, with only parameters that the selected generator supports. Preserve the original and copy the final project asset into the workspace when needed. Save the prompt and report the actual generator/model when available; do not invent hidden model metadata.
5. Inspect the rendered image for expression, action readability, prop count, occlusion, crop and material consistency. Check the actual PNG dimensions; some compatible services have returned 1254×1254 despite a 1024×1024 request. Preserve the original, then create a square 1024 delivery when needed.
6. Show the image inline and link the delivery and prompt. Do not call a candidate an approved baseline until the user accepts it.

## Diagnose drift

- **Polished toy or product photo:** reduce eye anatomy, PBR, reflections, cinematic light and realistic fabric; add original-style reference images.
- **Still physically heavy:** flatten prop geometry, remove deep creases and ambient occlusion, and reduce broad material gradients. Keep texture recognition.
- **Origami/voxel look:** remove hard triangular facets and cubes; keep coarse, slightly rounded forms.
- **Pasted-on prop:** match texture resolution, contrast, palette and basic lighting across every object.
- **Ambiguous joke:** describe silhouette and cause-and-effect, not only object names.
- **Old scene leaks into new scene:** assign each reference a role and explicitly discard its scene, clothing, expression and unrelated props.

## Copyright and packaging

This public repository includes only generated example images produced for this skill. It intentionally omits third-party creator images and watermarked source material. Users may provide their own reference images locally; do not commit them to a public repository without permission.

When the user says to preserve new feedback, update this skill, the relevant reference notes and the example index together. Add new images, saved prompts, actual feedback/acceptance status, catalog entries and batch previews to the extended library. Deduplicate identical images; keep alternate experiments only when they teach a distinct lesson. Keep rejected experiments clearly labeled rather than presenting them as the target. Archive relevant creative experience, not private transcripts, provider metadata or credentials.

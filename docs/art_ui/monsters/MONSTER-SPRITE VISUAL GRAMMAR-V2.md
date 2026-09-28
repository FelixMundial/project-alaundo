# MONSTER-SPRITE VISUAL GRAMMAR — V2

**Status:** Prototype guideline v2  
**Purpose:** Working reference for generating, evaluating, and later animating 2D enemy / monster combat sprites in this project  
**Scope:** Monster and enemy sprite grammar only.

---

## 1. Purpose and Direction

This document preserves the current working definition of the project's **DD-derived 2D monster sprite language** so future generation and evaluation remain consistent even if chat context is lost.

The current prototype target remains intentionally close to the visual grammar of *Darkest Dungeon* and compatible high-quality community work. The goal is to reproduce the underlying battlefield design logic first; deliberate stylistic divergence can come later.

A **DD-style monster sprite** is defined primarily by:

- silhouette-first threat readability;
- side-facing battlefield presentation toward the opposing formation;
- heavy ink-like contour and structural black: color-led in identity, black-led in structure. Species color may be primary in identity while secondary in value distribution, so it could be kept as the species identity hue, but subordinate more clearly to a black-dominant structural rendering system.
- stylized, species-grounded anatomy that may be humanlike, bestial, skeletal, mutated, asymmetric, tentacular, or physically impossible;
- controlled grotesquerie and organized detail;
- flat-to-hard-edged color modeling rather than realistic painterly volume;
- creature-specific anatomy and coloration preserved before stylistic transformation;
- clear combat footprint and attack direction;
- transparent-background production output.

The target is a **usable in-game combat sprite**, not creature concept art, splash art, a bestiary illustration, or a cinematic monster painting.

---

## 2. Reference and Species Calibration

For established creatures from tabletop games, folklore, or other well-defined source traditions, identify the creature's **species-defining traits** before applying the project style.

When useful, consult an official source, reliable setting reference, or asking the user specifically, to establish:

- body plan and proportions;
- locomotion and posture;
- characteristic head, limbs, sensory organs, claws, jaws, wings, or other anatomy;
- typical coloration and markings;
- signature combat behavior;
- supernatural features;
- meaningful variation within the species.

Then translate those traits into the DD-derived rendering grammar.

Do **not** allow stylistic motifs from one reference family to overwrite the creature's identity. Purple-black cosmic coloration, webbed flesh, clustered eldritch growths, glowing eyes, or similar motifs should not migrate automatically into unrelated monsters merely because they appear in other DD creatures.

A useful calibration sequence is:

1. **Species identity** — what makes the creature recognizably itself.
2. **Battlefield architecture** — body mass, attack feature, pose, scale, and orientation.
3. **DD-derived rendering** — hard contour, black structure, hard-edged shading, facial/surface simplification, and texture hierarchy.
4. **Optional experimentation** — controlled variations that do not erase species identity.

---

## 3. Definition of a Monster Sprite

A **monster sprite** is a complete 2D enemy figure designed to function as a battlefield unit.

By default, it should be:

- fully readable at gameplay scale;
- organized around one dominant threat silhouette;
- side-facing or slight three-quarter side-facing toward the opposing formation;
- visually legible in an encounter lineup, facing left;
- isolated on a **transparent background**;
- designed so its identity survives across idle, attack, reaction, howl, cast, and other combat poses.

The sprite should communicate creature type, threat profile, dominant anatomy, attack method, and supernatural or faction identity before fine surface detail is noticed.

---

## 4. Core Monster Sprite Rules

### 4.1 Silhouette, Threat Identity, and Battlefield Orientation

The monster should remain recognizable from its largest masses before internal detail is considered.

Prioritize:

1. **overall body mass and directional silhouette**;
2. **dominant anatomical or supernatural feature**;
3. **primary attack structure** — jaws, claws, weapon, tentacle cluster, eye, limb, maw, etc.;
4. **stance and threat gesture**;
5. **secondary texture or accessory clusters**.

A strong monster usually has one dominant visual idea: a giant eye, enormous claws, a caged head, a crystal-backed body, an emaciated jaw, a tentacle crown, or another immediately legible threat feature.

Monsters should normally **face toward the opposing hero formation rather than toward the player**. Under a heroes-left / enemies-right encounter convention, monster's body must face left.

### 4.2 Species-Grounded Anatomy, Faces, and Controlled Distortion

Monster anatomy may be humanoid, animalistic, skeletal, mutated, eldritch, multi-limbed, tentacular, or physically impossible, but distortion should begin from recognizable **creature architecture** rather than generic monster anatomy. Preserve the species-defining body plan first, then exaggerate selectively.

Useful tools include asymmetrical or distorted limbs and joints, exaggerated head or torso structures, duplicated/fused/vestigial anatomy, abnormal organs, tentacles, horns, spines, crystals, exposed bone, and non-standard limb counts. Use them to strengthen the creature concept, not to create random anatomical noise.

Avoid replacing distinctive anatomy with generic fantasy-brute musculature. A frog-like monster should retain batrachian mass and leg logic; an insectoid monster should retain arthropod structure; a floating aberration should preserve its defining sensory and locomotion system.

The viewer should still understand the main body mass, primary threat feature, battlefield footprint, and attack direction.

**Humanoid and near-humanoid faces require their own graphic treatment.** If the underlying face is humanlike, do not automatically give it the facial grammar of a beast, aberration, or eye-dominant monster. Favor:

***Eyes*** strong black or near-black eye-region shapes, specifically:

- eyes reduced to dark signs or very compact graphic marks;
- upper eye region heavily controlled by black/shadow;
- little to no conventional eye-volume rendering;
- the eye functioning more like a symbol than an observed anatomical organ.

***Nose***

- though the head is broadly side-facing, the nose is not aligned as a strict side-profile feature, and the visible contour of the nose is shown as if the face were being constructed through a literal profile edge;
- little or no insistence on a visible outward-projecting nose shape;
- the nose may be reduced to an extremely small wedge, notch, hook, or even nearly omitted;
- omit the nostril or philtrum entirely for facial treatment
- even when a nose is more visible, it is still treated as a graphic sign, not a modeled facial structure.

***Mouth*** a compact graphic mouth sign rather than anatomically modeled lips, specifically:

- a minimal emblem-like mouth shape;
- the lip area controlled heavily by black/shadow, not presented as a full red profile shape, or a conventionally attractive fantasy lips rendering.
- the mouth feels embedded into the graphic mask of the face, and color appears selectively rather than filling the whole lip form.

- simplified cheek and jaw planes;
- minimal skin-volume detail;
- hair grouped into large silhouette masses rather than strands;
- expression carried mainly by head angle, brow shadow, mouth shape, contour, and pose.

A humanoid face should be primarily **abstracted and emblematic**, and the face remains readable because DD prioritizes mask-like emblem clarity, not anatomical profile fidelity.

Choose facial treatment according to anatomy and state rather than imposing one universal “monster face”:

- **shadow-obscured humanoid** — heavy upper-face shadow and minimal features: obscured eyes, minimal nose/mouth marks;
- **simplified attractive humanoid** — elegant silhouette with eyes reduced almost to dark signs; nose nearly absent; mouth a black/shadow sign, with red used only as a restrained accent rather than filling the whole lip shape; face reads almost like a mask or emblem; hair carried by big silhouette masses, not naturalistic hair description;
- **species-feature-dominant humanoid** — conspicuous eyes, jaws, snouts, fins, etc. only when species-defining;
- **undead / supernatural-state humanoid** — glowing eyes, hollow sockets, facial voids, etc. only when state-defining;
- **corrupted / mutated humanoid** — selected distortion over a still-readable underlying face;
- **masked / obscured humanoid** — mask, helmet, veil, restraint, or head structure becomes the main expressive device.

Bosses may carry more facial information, but **increasing detail should increase personality and theatrical caricature, not anatomical realism**.

### 4.3 Scale, Mass, and Role Readability

Use mass, breadth, height, and silhouette disruption to communicate threat tier, but do not equate size with detail density.

Useful tendencies:

- common enemies: compact, efficient, role-driven silhouettes;
- elite or large enemies: stronger massing and one dominant visual gimmick;
- large aberrations: more extreme silhouette disruption around a readable center;
- boss-scale creatures: expanded mass, stronger asymmetry, and one or two unmistakable spectacle features.

A large monster should feel **more imposing**, not merely busier.

Related enemy families should share visible anchors such as anatomy, materials, color accents, cranial treatment, markings, mutations, clothing fragments, or contour language. Different roles should diverge through weapon silhouette, posture, scale, body modification, or one role-specific feature.

The goal is **family resemblance with role differentiation**, not recolors and not unrelated designs joined only by lore.

### 4.4 Structural Black, Matte Organic Surfaces, and Graphic Rendering

Use heavy black outer contouring and bold angular internal linework. Black should actively construct the creature through silhouette edges, cavities, body separations, undercuts, occlusion pockets, fold/wound/bone/armor gaps, negative-shape carving, and hard internal shadow wedges.

Do not use black merely as an outline filter over painterly concept art. Not every visible plane should be painted in its own saturated color, and controlled accent placement could fit inside a black heavy structure. Iconic colors often remain legible and identity-defining, but they are usually contained inside a black-dominant structural/value system rather than spread as broad, evenly lit, high-visibility local color.

- Species color dominates chromatic identity
- Black dominates structural value logic
- Texture is expressed more through contour/shadow carving than through fully lit local-color description

Keep species-defining local color legible, but organize the sprite through black-dominant value structure; visible color planes should usually read as bounded midtone masses rather than broad evenly lit surfaces.

Favor:

- flat or mostly flat local color masses;
- hard-edged selective shading;
- graphic value separation;
- stylized surface marks;
- controlled texture clusters;
- matte treatment of skin, eyes (including iris), flesh, scales, membranes, and similar organic materials.

Organic surfaces should normally **not** look wet, glossy, translucent, photoreal, or materially over-rendered unless that quality is species-defining. Avoid glossy corneal reflections, bright photographic eye catchlights, smooth wet-skin highlights, realistic subsurface scattering, high-frequency pores/veins/scales, smooth cinematic gradients, and soft volumetric modeling.

Eyes should read mainly through **shape, contrast, and graphic color blocking**. Being an enemy is not sufficient justification for luminous, feline, reptilian, glossy, or otherwise supernatural eyes. Unusual eye treatment should be supported by species anatomy, supernatural state, corruption, sensory adaptation, or established source identity; otherwise humanlike monsters should retain simplified humanlike eyes or shadowed eye regions.

### 4.5 Organized Grotesquerie, Texture, Serpentine Surfaces, and Color

Grotesque detail may be intense, but it should remain hierarchical. Use abnormal anatomy, corruption, or texture to reinforce species/family, decay or mutation, one dominant bodily abnormality, faction/environmental identity, or attack function.

Avoid covering the entire creature in equal-intensity scars, veins, pustules, eyes, teeth, bones, scales, crystals, or tentacles. A useful hierarchy is:

1. dominant silhouette abnormality;
2. major anatomical feature;
3. secondary texture clusters;
4. tertiary surface marks.

For **snakes, naga-like bodies, serpent-tailed creatures, and similar anatomy**, build the surface in this order:

1. the body reads first as large coil masses;
2. black shadow separations do a lot of the structural work;
3. scales are not evenly tiled everywhere;
4. ventral plates are large and readable;
5. texture is clustered and subordinate to the body’s graphic staging.

Do not tile detailed scales uniformly over the full body. Concentrate scale information around focal regions, torso-to-serpent transitions, strong contours, bends where scale direction clarifies volume, species-defining markings, and occasional coil segments. Other areas may remain nearly plain apart from hard shading and sparse graphic marks.

Serpentine bodies should not automatically become smooth decorative naga illustrations. Prefer uneven detail distribution, harder black separations between coils, occasional angular simplification of curvature, broad matte color planes, readable ventral plates, and sparse clustered scales. The body should read first as a **combat silhouette**, second as serpent anatomy, and only afterward as a collection of scales.

Use controlled body colors with selective stronger accents. Accent color may mark supernatural energy, corrupted tissue, sensory organs, ritual markings, crystal growths, toxins, spores, or faction identity.

Do not assume all monsters should use DD's own palette. Color should primarily follow **creature identity**, then be translated into the project's controlled graphic palette.

### 4.6 Combat Pose and Production Output

Monster poses should be staged, readable, and role-specific rather than naturalistically cinematic.

Useful pose logic includes hunched predation, spring-loaded animal posture, upright ritual/caster stance, looming vertical mass, lateral weapon or limb extension, claw/jaw/eye/tentacle emphasis, attack preparation, and asymmetrical weight distribution.

Keep the creature readable at gameplay scale. Avoid dramatic camera tilt, excessive foreshortening, or player-facing presentation that turns the sprite into an illustration rather than a battlefield unit.

Default output must use a **transparent background**. Do not add environment, decorative framing, ground planes, interface elements, text, baked scenery, unrelated props, or ground-contact shadows unless explicitly requested.

Active effects should appear only when integral to the creature's current state or attack, and should be made easy to manually crop into separate fx images.

---

## 5. Practical Generation Workflow

When generating a monster sprite, separate four layers:

1. **Species / source calibration** — canonical anatomy, coloration, locomotion, behavior, and justified facial/sensory traits.
2. **Creature architecture** — body plan, scale, symmetry/asymmetry, dominant threat feature, and battlefield footprint.
3. **Core monster grammar** — side-facing orientation, structural black, graphic facial/surface simplification, matte organic rendering, and detail hierarchy.
4. **Generation-specific variation** — pose, minor mutation, color nuance, or controlled stylistic experimentation.

This separation prevents generic creature-concept-art drift and accidental replacement of species identity with borrowed DD-specific motifs.

---

## 6. Common Generation Failure Modes

Correct these before treating a result as style-consistent:

- **frontal/player-facing drift:** the monster looks outward at the viewer instead of toward the opposing formation;
- **species/lore drift:** defining anatomy, coloration, posture, behavior, or sensory traits are lost;
- **reference-style contamination:** motifs from unrelated DD monsters are imported without species/state justification;
- **generic anatomy drift:** distinctive creature structure collapses into a generic humanoid, brute, reptile, beast, or blob;
- **portrait / beauty-face drift:** a humanlike monster acquires realistic lips, nose, eyelids, cheek modeling, skin volume, or polished fantasy-beauty rendering instead of graphic facial shorthand;
- **generic monster-eye drift:** ordinary humanoid enemies receive glowing, feline, glossy, or supernatural eyes without species/state justification;
- **glossy organic realism:** skin, eyes, flesh, scales, or membranes become wet, reflective, translucent, or photorealistic;
- **scale tiling / decorative-serpent drift:** serpent bodies are uniformly covered in detailed scales or polished into smooth decorative coils instead of being built from broad masses and selective texture;
- **silhouette collapse:** too many limbs, tendrils, props, or details obscure the primary threat shape;
- **random anatomical chaos:** mutation or asymmetry lacks a clear body concept;
- **detail or texture inflation:** larger or more dangerous monsters become busy instead of imposing;
- **weak structural black:** black fails to carve the forms and the monster's own color too dominant;
- **painterly drift:** soft lighting, realistic materials, and cinematic volume replace the graphic sprite language;
- **unclear attack logic:** the dominant threat feature or attack direction is difficult to read;
- **faction incoherence:** related enemies do not share enough visual family traits;
- **effect clutter:** glow, mist, particles, splashes, or aura obscure the body design;
- **transparent-background failure:** scenery, floor, glow field, or backdrop is baked into the asset.

---

## 7. Prototype Universal Monster Sprite Grammar — V2

Use this as the current reusable **first-layer** generation grammar before adding the specific monster description:

> Create a complete 2D in-game monster combat sprite closely following Darkest Dungeon enemy-sprite grammar. The result must read as a battlefield unit, not creature concept art, splash art, or cinematic fantasy illustration.
>
> Preserve the creature's defining species anatomy, coloration, locomotion, sensory traits, and threat features before stylizing it. Build the design around one dominant silhouette and one or two unmistakable attack or anatomical features. Distortion, asymmetry, mutation, or impossible anatomy are welcome only when they strengthen the creature concept rather than replace it with generic monster anatomy.
>
> Present the monster primarily from the side or slight three-quarter side, facing toward the opposing hero formation rather than toward the player. Use a graphic theatrical combat pose with a clear center of mass, attack direction, and battlefield footprint. Avoid frontal portrait-like presentation, cinematic camera angles, and excessive foreshortening.
>
> Render with heavy black contouring, bold angular internal linework, structural black shadows, flat graphic color planes, and hard-edged selective shading. Treat skin, eyes, exposed flesh, scales, and membranes as matte graphic surfaces with sparse hard highlights; avoid glossy eyes, wet skin, realistic subsurface rendering, and high-frequency organic microtexture unless those qualities are species-defining. For humanoid or near-humanoid faces, use graphic facial shorthand with strong eye-region shadow, simplified angular noses, compact stylized mouths, and minimal portrait modeling; do not add unusual glowing or bestial eyes unless species- or state-defining.
>
> Keep grotesque detail hierarchical and preserve the creature's own color identity rather than importing unrelated cosmic palettes or motifs. For scaled or serpentine anatomy, establish broad body and shadow masses first and use scales selectively in clustered focal areas rather than uniformly tiling the surface. Keep the sprite readable at gameplay scale and isolate the complete creature on a transparent background with no scenery, ground shadow, interface elements, or unrelated effects.

---

## 8. Open Parameters / Unresolved Decisions

The following remain deliberately unresolved:

- exact production dimensions and native sprite resolution;
- standardized size tiers for common, elite, large, and boss creatures;
- exact acceptable silhouette overlap for multi-limbed or tentacular designs;
- faction-specific repetition standards;
- grotesquerie thresholds by creature type;
- how much asymmetry is appropriate before readability fails;
- how texture density should vary by threat tier outside anatomy-specific rules such as selective serpent scaling;
- exact rules for supernatural glow and emissive accents;
- exact asset-separation requirements for rigging, deformable appendages, jaws, wings, weapons, and alternate pose pieces;
- how closely the final proprietary monster style should continue to mimic DD after prototype validation.

Do not silently convert these into fixed rules in future prompts.

---

## 9. Version Note

V2 supersedes V1 as the current **monster-sprite prototype grammar**, while V1 should be retained as a historical calibration document.

The current V2 incorporates the Marilith-derived facial and serpentine patch. Its principal corrections are:

- battlefield-facing orientation is explicit;
- species identity and source calibration come before stylistic transformation;
- creature-specific anatomy is protected against generic humanoid or fantasy-monster drift;
- humanlike monster faces use graphic DD-like facial economy rather than portrait anatomy, with treatment selected by species and state;
- unusual “monster eyes” require anatomical, supernatural, or lore justification;
- organic materials remain matte and graphic rather than wet or glossy;
- serpentine bodies are constructed from coil/shadow/color masses before selective scale detail;
- DD-specific motifs and palettes are not universal monster defaults.

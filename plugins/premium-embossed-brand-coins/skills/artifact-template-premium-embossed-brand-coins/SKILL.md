---
name: artifact-template-premium-embossed-brand-coins
description: "Create an image or a reusable image-generation prompt using the Premium Embossed Brand Coins template and its retained reference file. Use when the user selects this template, names Premium Embossed Brand Coins, or explicitly invokes $artifact-template-premium-embossed-brand-coins. Generate well-lit, premium pale-silver brand coins with flat clean faces, one centred shallow embossed logo, textured outer reeding only, and controlled studio reflections."
---

# Premium Embossed Brand Coins

Create an image from this template. Keep the reference file unchanged.

## Prompt-only requests

When the user asks for a prompt, return a ready-to-paste, self-contained generation prompt instead of generating an image. Do not require an image reference. The user need only specify the brand or brands, exact coin count, and the composition, arrangement, or placement. The prompt must supply every locked visual rule below automatically.

## Brand allocation

Use only the brand names the user supplies. If the user supplies exactly one brand and requests any number of coins, every coin must carry only that single brand's primary logo; do not introduce, infer, or retain any other brand from the template reference, prior examples, or general market knowledge. If the user supplies fewer brands than coins, repeat only the supplied list in order. If the user supplies more brands than coins, use only the first requested number of brands in order.

## Reference roles — required before writing a prompt

Classify every user-supplied image according to the role the user gives it. Never let a composition reference replace the locked coin construction.

- **Composition-only reference:** When the user calls an image an arrangement, composition, stack, layout, pose, or placement reference, borrow only its macro spatial idea: relative scale, tilt, overlap, cropping, and negative-space distribution. Do not borrow its coin construction, face borders, grooves, rim bands, materials, lighting, logos, typography, palette, or backdrop. State COMPOSITION REFERENCE ONLY inside the final generation prompt.
- **Style/material reference:** When the user calls an image a look-and-feel, material, coin-style, or lighting reference, borrow only the requested material response, illumination, and background treatment. Keep the supplied brand, count, and requested composition; never copy a source logo or text.
- **Full visual reference:** Borrow all visual properties only if the user explicitly says that the image is a full reference.

When a request includes both an arrangement image and a look-and-feel image, use the arrangement image for composition only and the look-and-feel image for material/style only. The retained reference and the locked visual system always govern coin construction unless the user explicitly requests a different construction.

### Translating a conventional coin stack

If a composition reference depicts a traditional currency-coin tower, translate only its macro silhouette: for example, a lower anchor, an ascending offset, and a tilted hero coin. The result remains a sculptural cluster of the locked coins—not a literal money pile. Never inherit multiple parallel face rims, decorative grooves, layered rim bands, or a generic pancake-stack construction.

## Locked visual system

Treat the retained references as the definitive visual target. This is a well-lit, premium 3D product-render system, never a generic minted currency coin.

- **Background:** In light mode, use a seamless warm porcelain-white studio background with faint cream warmth, broad soft tonal falloff, and no props, texture, horizon, or visual noise. In dark mode, use a seamless near-black graphite studio background with restrained charcoal depth.
- **Coin shape:** every coin is a thick, substantial, perfectly circular disc with a simple silhouette. There is no ornamental face construction, no inner medallion, and no decorative ring system.
- **Flat front surface:** the visible front is one completely flat, clean, uninterrupted circular plane running directly into the narrow outer chamfer. It has no radial brush marks, machining lines, concentric circles, grooves, inscription, inset border, raised inner rim, or perimeter outline.
- **Single centred emboss:** each coin contains only its assigned brand's official primary mark, centred on the flat face as one low, positive metallic emboss. Default relief height is approximately 0.8–1% of the coin diameter: enough to show a slim chamfered sidewall, fine upper-edge glint, and soft contact shadow, but never so high that it reads as chunky or deeply extruded. It is same-colour metal, never printed, coloured, outlined, or recessed.
- **One consistent coin colour:** all coins use the same pale neutral silver material. Apparent ivory, graphite, or soft champagne areas are environmental reflections on that one silver material, never different plating, painted surfaces, or separate coin colours.
- **Edge texture only:** use a narrow polished outer chamfer and dense, fine vertical reeding on the external sidewall. The reeding and the logo bevels are the only line or stroke texture in the system. Reeding may look dark in its grooves from occlusion, but it must never migrate onto the flat front face as a border.
- **Light and reflections:** select one dominant large studio key source according to the requested arrangement: high above and slightly behind for elevated or front-facing coins, or from the side for a side-on stack or profile composition. Use restrained dark negative fill opposite the key and a gentle warm-white bounce. This creates broad, feathered ivory-to-graphite reflections over the flat silver faces, bright rim highlights, small sharp glints on the chamfer and reeding, and sculptural definition around the embossed logo. Reflections must have soft tonal transitions—never an isolated, harsh, near-black patch or hard shadow boundary on a visible face. Never use flat, uniform, front-on lighting.
- **Overall result:** precise, sparse, luminous, expensive, and editorial.

Avoid radial texture on the face, face borders, circular rings, grooves, engraved typography, antiqued metal, coloured logos, gold, cryptocurrency styling, gaming art, and visual clutter.

### Default single-coin camera

When a user asks for a single coin without a more specific pose, frame it almost straight toward the camera with a slight lateral camera offset. The face remains dominant while one narrow strip of the reeded external sidewall is visible. This is a restrained product-shot perspective, not a turned-away profile.

## Coin-face construction

The main coin has one uninterrupted, flat circular face. Do not add an inset circular ring, raised inner rim, recessed border, perimeter groove, decorative face outline, or any other border between the central emboss and the outer edge. The only edge treatment is the coin's external chamfer and reeded outer circumference. Brand marks are centred low positive metallic bas-reliefs on the uninterrupted face.

## Workflow

1. Read artifact-template.json and resolve its paths relative to this skill directory.
2. Assign every supplied image a reference role. Use a composition-only image only for its macro arrangement; use a style/material image only for the explicitly requested look; use the retained PNG and locked visual system for every unspecified detail of the coin construction.
3. Preserve the reference's visual language unless the user explicitly requests a deviation.
4. Visually inspect generated images for flat faces, restrained logo relief, soft reflection transitions, and defects before returning them.

## Fidelity

For coin construction, preserve the retained reference's flat face, one centred low positive emboss, pale-silver material, outer reeding, and controlled studio reflections. Preserve only the properties authorised by each user reference's assigned role.

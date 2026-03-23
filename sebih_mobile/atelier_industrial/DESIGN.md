# Design System Strategy: The Woven Editorial

This design system is a bespoke visual framework crafted for Sebih Textile. It bridges the gap between high-end luxury and industrial reliability. Our goal is to move beyond the "SaaS template" look, opting instead for a "Digital Showroom" experience that feels as tactile as the fabrics the brand produces.

---

### 1. Overview & Creative North Star: "The Architectural Loom"
The Creative North Star for this system is **The Architectural Loom**. 

In textile manufacturing, the beauty of the final product relies on the rigid precision of the machinery (the industrial) and the fluid elegance of the thread (the luxury). This system translates that duality into a UI that feels structured yet breathable. We break the "template" look by using **Intentional Asymmetry**: placing large-scale serif typography off-center and allowing images of high-quality textiles to overlap container boundaries. 

The layout should never feel "boxed in." We prioritize breathing room over information density, ensuring every element feels curated rather than merely placed.

---

### 2. Color & Surface Philosophy
The palette utilizes the depth of **Primary Deep Navy (#1B2A4A)** and the warmth of **Secondary Gold (#C9A96E)** to establish authority and prestige.

#### The "No-Line" Rule
To maintain a high-end editorial feel, **1px solid borders for sectioning are strictly prohibited.** We define boundaries through tonal shifts rather than structural lines. For example, a `surface-container-low` section should sit directly against a `surface` background to create a soft, sophisticated transition.

#### Surface Hierarchy & Nesting
Think of the UI as physical layers of fine paper.
- **Base Layer:** `surface` (#fbf9f6) for the main canvas.
- **Section Layer:** `surface-container-low` (#f5f3f0) for large structural blocks.
- **Component Layer:** `surface-container-lowest` (#ffffff) for cards and interactive modules to provide a crisp "lift" against the warm gray.

#### The "Glass & Gradient" Rule
Standard flat colors can feel sterile. For Hero sections and Primary CTAs, use a subtle linear gradient transitioning from `primary` (#041534) to `primary-container` (#1B2A4A). Use Glassmorphism (semi-transparent surface colors with a `20px` backdrop-blur) for floating navigation bars to let the "Woven" texture overlays bleed through the interface.

---

### 3. Typography: Editorial Authority
Our typography is a dialogue between the heritage of Serif and the precision of Sans-Serif.

- **Display & Headlines (Playfair Display / NotoSerif):** These are our "Statement" pieces. Use `display-lg` (3.5rem) with tight letter-spacing for hero statements. The serif represents the "Luxurious" mood—reliable, established, and confident.
- **Body & Labels (Inter):** The "Industrial" worker. Inter provides maximum legibility at smaller scales. Use `body-lg` (1rem) with a generous `1.6` line-height to ensure the text feels as premium as the imagery.
- **Hierarchy Tip:** Always pair a `display-md` headline with a `label-md` in all-caps (0.05em letter-spacing) using the `secondary` gold color to create an "Editorial Tag" effect.

---

### 4. Elevation & Depth: Tonal Layering
We avoid heavy drop shadows that clutter the UI. Depth is achieved through the **Layering Principle.**

- **Ambient Shadows:** For floating elements like Modals or Dropdowns, use an ultra-diffused shadow. 
  - *Spec:* `0px 20px 40px rgba(27, 28, 26, 0.06)`. This mimics soft, natural gallery lighting.
- **The "Ghost Border" Fallback:** If an element lacks contrast against its background, use a **Ghost Border**. This is a 1px stroke using `outline-variant` at **15% opacity**. It should be felt, not seen.
- **Signature Motif:** Apply a subtle woven texture overlay (SVG pattern) at **3% opacity** over `primary` containers to evoke the tactile nature of Sebih textiles.

---

### 5. Components & Primitive Styling

#### Buttons: The Tactile Interaction
- **Primary:** `primary` background with `on-primary` text. Use `rounded-md` (0.375rem). The hover state should transition to `primary-container` with a subtle `secondary` (gold) bottom border (2px) to signify "The Thread."
- **Secondary:** Transparent background with a `secondary` (gold) "Ghost Border."

#### Cards: The Floating Specimen
- Forbid divider lines within cards. Separate the "Product Image" from "Product Details" using `spacing-6` (2rem) of vertical whitespace. 
- Background: `surface-container-lowest` (#ffffff).
- Corner Radius: `rounded-lg` (0.5rem).

#### Input Fields: The Minimalist Form
- Forgo the "box" look. Use a `surface-container-low` background with a `2px` bottom-only border in `outline-variant`. On focus, the bottom border animates to `secondary` (gold).

#### Signature Component: The "Fabric Detail" Chip
- Used for textile specs (e.g., "100% Cotton"). Use `surface-variant` background with a tiny `secondary` (gold) dot prefix. This reinforces the industrial-professional nature of the B2B specs.

---

### 6. Do’s and Don’ts

#### Do:
- **Use generous whitespace:** If you think there is enough space, add `spacing-4` more. High-end brands "waste" space to show they can afford it.
- **Embrace Asymmetry:** Align text to the left while keeping imagery slightly off-grid to create a dynamic, modern editorial flow.
- **Use the Gold Sparingly:** The `secondary` gold color is a "spice." Use it for accents, thin divider lines between distinct content groups, or small labels.

#### Don’t:
- **No 100% Black:** Never use pure black for text. Always use `on-surface` (#1b1c1a) to keep the contrast sophisticated, not jarring.
- **No Heavy Borders:** Avoid the "Table" look. Use `surface-container` shifts to organize data.
- **No Sharp Corners:** While we are "Industrial," we are not "Brutalist." Use the `roundedness scale` to soften the user journey.

---

### 7. Spacing & Rhythm
Consistency is the heartbeat of this system. All spacing must follow the **Incremental Scale**. 
- Use `spacing-12` (4rem) for section padding.
- Use `spacing-3` (1rem) for internal component grouping.
- Use `spacing-24` (8.5rem) to separate major thematic shifts on a page.
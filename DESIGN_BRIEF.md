# Design Brief — Sebih Textile B2B Website

## Overview

Premium B2B textile company website for a Turkish fabric supplier. The site must communicate **trust, quality, and professionalism** — these are the pillars of Turkish B2B commerce. The target audience is wholesale buyers (textile manufacturers, fashion brands, interior designers) across Turkey, CIS, and Europe.

**Language:** Turkish (primary), with Russian and English toggle options.

---

## Brand Direction

### Visual Identity
- **Mood:** Luxurious yet industrial. Think premium fashion house meets reliable manufacturer.
- **Color palette:** Deep navy (#1B2A4A) as primary, warm gold/bronze (#C9A96E) as accent, crisp white (#FFFFFF) for backgrounds, light warm gray (#F5F3F0) for sections. Avoid bright or playful colors.
- **Typography:** Clean serif for headings (e.g., Playfair Display or similar), modern sans-serif for body (e.g., Inter or Montserrat). Large, confident heading sizes.
- **Photography style:** Close-up macro shots of fabric textures, warehouse/production imagery, lifestyle shots of textiles in use. All photos should feel warm-toned and high-end.
- **Design language:** Generous whitespace, subtle shadows, clean lines. No clutter.

### Motifs & Patterns
- Subtle woven/thread texture overlays in backgrounds (very low opacity)
- Thin gold divider lines between sections
- Rounded rectangles for cards, soft shadows

---

## Pages & Layouts

### 1. Landing Page (Homepage)

**Purpose:** Immediately establish credibility and guide visitors to the catalog.

**Sections (top to bottom):**

1. **Hero Section** — Full-width background image (fabric texture or production facility). Overlay with company name/logo, tagline in Turkish: *"Kaliteli Kumaşlar, Güvenilir Ortaklık"* (Quality Fabrics, Trusted Partnership). Primary CTA button: "Kataloğu Görüntüle" (View Catalog). Secondary CTA: WhatsApp contact button (floating, persistent across all pages).

2. **Trust Bar** — Horizontal strip showing: years in business (e.g., "25+ Yıl"), number of clients served, countries exported to, fabric types available. Use large numbers with icons. Dark background (navy).

3. **Featured Categories** — 3-4 large cards in a grid: Cotton, Silk, Linen, Synthetic (or relevant categories). Each card: full-bleed fabric photo, category name overlay, hover effect revealing item count. Clicking navigates to filtered catalog.

4. **Why Choose Us** — 3-column layout with icons: Quality Guarantee, Competitive Pricing, Fast Delivery. Short description under each. Clean white background.

5. **New Arrivals / Featured Fabrics** — Horizontal scrollable carousel of 6-8 product cards showing: fabric thumbnail, name, composition, price range, "Details" button.

6. **Testimonial / Partner Logos** — Optional. Logos of partner brands or short quote from a buyer. Adds social proof.

7. **CTA Banner** — Dark section with text: "Ready to place an order?" + WhatsApp button + Phone number.

8. **Footer** — Company info, navigation links, social media icons, Turkish business registration info. Dark navy background with gold accents.

---

### 2. Catalog Page

**Purpose:** The core of the website. Must feel like a professional tool, not just a gallery.

**Layout:**

- **Left Sidebar (Desktop) / Top Filter Bar (Mobile):**
  - Search input with icon (search by name, article number, composition)
  - Category filter (checkboxes): Cotton, Silk, Linen, Polyester, Blended, etc.
  - Weight filter (g/m²): range slider
  - Width filter (cm): range slider
  - Color filter: color swatches (clickable circles)
  - Price range: slider or min-max inputs
  - Country of origin: dropdown
  - "Reset Filters" button

- **Main Content Area:**
  - Top bar: result count ("124 kumaş bulundu"), sort dropdown (Price ↑↓, Newest, Popular, Name A-Z), view toggle (grid / list)
  - **Grid View:** 3 columns desktop, 2 tablet, 1 mobile. Card: photo, name, composition, weight, price per meter, "Add to Inquiry" button
  - **List View:** Horizontal rows with more detail visible: photo (small), name, composition, weight, width, color, price, "Add to Inquiry"
  - Pagination or infinite scroll at bottom

- **Product Detail Modal/Page (on card click):**
  - Large image gallery (4-5 photos, zoomable)
  - Full specifications table: composition, weight, width, color, MOQ, delivery time
  - "Add to Inquiry" button (adds to inquiry basket)
  - "Download Specification PDF" button
  - Related/similar fabrics section below

- **Inquiry Basket (floating icon, bottom-right):**
  - Shows count of selected fabrics
  - Expandable panel listing selected items
  - "Send Inquiry via WhatsApp" button — pre-fills WhatsApp message with selected items

**Design notes:** Filters must be responsive and not overwhelming. Use collapsible filter groups on mobile. Loading states should use skeleton screens, not spinners.

---

### 3. About Us Page

**Purpose:** Build trust and personal connection.

**Sections:**

1. **Hero** — Wide photo of the team or facility. Overlay text: "Hakkımızda" (About Us).

2. **Our Story** — Two-column layout. Left: text about company history, values, experience in textile trade. Right: photo of founder/team or facility interior. Warm, human tone.

3. **Timeline** — Horizontal or vertical timeline showing key milestones: founding year, first export, expansion, certifications obtained, etc. Use gold dots on a navy line.

4. **Our Advantages** — Icon grid (2x3): Quality Control, Wide Range, Custom Orders, Fast Logistics, Competitive Prices, Multilingual Support.

5. **Certifications & Standards** — Logos/badges of textile certifications (Oeko-Tex, ISO, etc.) in a horizontal row.

6. **Team** (Optional) — Photo cards of key team members with name and role. Circular photos, minimal style.

---

### 4. Contacts Page

**Purpose:** Make it effortless to reach the company through any channel.

**Layout:**

1. **Header** — "İletişim" (Contact) with subtitle: "We'd love to hear from you."

2. **Two-Column Layout:**
   - **Left column — Contact Information:**
     - Phone number(s) with click-to-call
     - WhatsApp number with direct link (prominent, green accent)
     - Email address with mailto link
     - Physical address with small embedded Google Map below
     - Working hours (Turkish business hours)
   - **Right column — Contact Form:**
     - Name, Company, Email, Phone, Subject (dropdown: General Inquiry / Order / Partnership / Other), Message textarea
     - "Gönder" (Send) button

3. **Full-Width Map** — Embedded Google Map showing company location. Styled to match site palette (use custom map styling — muted colors).

---

### 5. Cargo Tracking Page

**Purpose:** Simple redirect to WhatsApp for shipment tracking inquiries.

**Layout:** Single centered card on a clean background.

1. **Icon** — Large shipping/truck icon or package tracking illustration.
2. **Heading** — "Kargo Takibi" (Cargo Tracking)
3. **Text** — "To track your shipment, please contact us via WhatsApp with your order number."
4. **WhatsApp Button** — Large, prominent green button: "WhatsApp ile İletişime Geç" (Contact via WhatsApp). Pre-filled message: "Merhaba, sipariş takibi yapmak istiyorum. Sipariş numaram: "
5. **Alternative** — Small text below: "Or call us at +90 XXX XXX XX XX"

---

## Global Components

### Navigation (Header)
- Sticky top bar, white background with subtle shadow on scroll
- Logo (left), nav links (center): Ana Sayfa, Katalog, Hakkımızda, İletişim, Kargo Takibi
- Language switcher (right): TR | RU | EN (flag icons)
- Mobile: hamburger menu with full-screen overlay

### Floating WhatsApp Button
- Fixed bottom-right corner on all pages
- Green circle with WhatsApp icon
- Pulse animation on first load to draw attention
- Opens WhatsApp with pre-filled greeting message

### Footer
- 4-column layout: Company Info, Quick Links, Contact, Social Media
- Newsletter signup input (optional)
- Copyright line at bottom
- Dark navy background, light text, gold accents

---

## Responsive Breakpoints
- Desktop: 1200px+
- Tablet: 768px–1199px
- Mobile: below 768px

All pages must be fully responsive. Catalog filters collapse into a drawer/modal on mobile. Cards stack vertically. Navigation becomes hamburger menu.

---

## Key Design Principles

1. **Trust first** — Every design decision should reinforce reliability and quality
2. **Less is more** — Generous whitespace, no visual clutter
3. **Mobile-ready** — Turkish businessmen often browse on phones
4. **Fast-loading feel** — Use skeleton screens, optimistic UI, lazy-loaded images
5. **Accessible** — High contrast text, large tap targets, readable fonts (min 16px body)

---

## Deliverables Expected

For each page, provide:
- Desktop layout (1440px width)
- Mobile layout (375px width)
- Key interaction states: hover, active, loading, empty states for catalog

**File format:** Exportable assets (SVG for icons, component-based structure preferred).

# Axis Chiropractic Landing Page Implementation Plan

We will overhaul the existing home page of the `axischirorva` workspace, converting it into a premium, responsive, single-page landing page that adheres to the pre-launch compliance requirements ("Coming Late Summer 2026") and captures founding patient registration and insurance credentials.

## User Review Required

> [!IMPORTANT]
> **Pre-Launch Regulatory Compliance**
> All text and copy must explicitly mention **"Coming Late Summer 2026"** and **"Clinical Development Phase"** to ensure it is clear that the practice is not currently open or active for self-employment. 

> [!NOTE]
> **Asset Management**
> - The logo `Axis Chiropractic Logo 1.png` has been copied from `Downloads` into [images/Axis Chiropractic Logo 1.png](file:///c:/Users/rberu/Desktop/axischirorva/images/Axis%20Chiropractic%20Logo%201.png).
> - We generated a custom monochromatic anatomical render for the "Stages of Spinal Degeneration" and placed it in [images/spinal_degeneration.png](file:///c:/Users/rberu/Desktop/axischirorva/images/spinal_degeneration.png).
> - Since `image_2cdc9e.png` was not found in the workspace or home folders, we will use a stark, clean off-white contrasting background (`#F5F6F8`) with rich charcoal typography (`#2F3538` and `#111111`) and copper accents (`#B87333`) for the Section 3 Insurance Bridge.

---

## Proposed Changes

### Frontend Design System & Styling
We will define styling rules in a modular stylesheet (or modify [style.css](file:///c:/Users/rberu/Desktop/axischirorva/css/style.css)) using the following palette:
- **Primary Background**: Deep Charcoal (`#2F3538`)
- **Typography**: Rich Black (`#111111`) / Off-White (`#F5F5F5` / `#FFFFFF`)
- **Accents & CTAs**: Metallic Copper (`#B87333`)
- **Design Tokens**: Inter font, generous line heights, massive negative space, glassmorphism headers, smooth scroll transitions.

### [index.html](file:///c:/Users/rberu/Desktop/axischirorva/index.html)
We will rewrite the root file to feature the new six-section wireframe architecture:

1. **Section 1: Minimalist Header**
   - Fixed header with a glassmorphism blur.
   - Logo: `images/Axis Chiropractic Logo 1.png` (scaled appropriately).
   - Navigation: "The Protocol" | "Pre-Verify Insurance" | "Join Roster".
2. **Section 2: Pre-Launch Hero Section**
   - Headline: *"AXIS CHIROPRACTIC: Precision Structural Integrity for RVA."*
   - Sub-headline: *"Launching Late Summer 2026. We are currently engineering a modern, high-volume facility specializing in non-surgical structural and neurological restoration. Private practice development in progress."*
   - CTA button (Metallic Copper): "Secure Placement on Founding Roster" (scrolls to Section 3).
3. **Section 3: Frictionless Insurance Bridge (High Contrast)**
   - High-contrast, clean light background.
   - Copy outlining Anthem BCBS in-network pre-verification.
   - Form fields: *Full Name*, *Email*, *Phone*, *Insurance Carrier*.
   - Submit CTA: "Submit Pre-Verification Request".
4. **Section 4: Symptom-to-Structure Pivot**
   - Copy: *"Pain is a Trailing Indicator..."*
   - Visual: Two-column grid featuring the copy next to our generated anatomical structural render `images/spinal_degeneration.png`.
5. **Section 5: High-Volume Operational Flow**
   - Copy describing open-concept, high-efficiency adjusting framework for high-performance lives.
6. **Section 6: Footer & Compliance Anchor**
   - Copyright, clinical development disclaimers, Privacy Policy, and Terms of Pre-Registration.

---

## Verification Plan

### Automated/Syntax Checks
- Validate HTML structure for tags and semantic formatting.
- Check stylesheet syntax.

### Manual Verification
- Verify responsiveness across viewport sizes (mobile, tablet, desktop).
- Verify the navigation links scroll smoothly to their respective targets.
- Verify form input states (focus, hover, filled).

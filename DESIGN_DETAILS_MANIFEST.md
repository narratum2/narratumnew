# 🏆 Forensic Design Details Manifest
**Narratum.io - Award-Winning Hospitality Experience**

---

## Philosophy
Every detail designed with the care of a 5-star hotel concierge.  
Not a tech product — a human experience.

---

## 🎯 Micro-Interactions (Desktop)

### Close Button (Modal)
- **Size**: 44×44px circle
- **Position**: Top-right, 28px inset
- **Effect**: Rotates 90° + scales to 1.08 on hover
- **Feel**: Like closing a jewelry box — weighted, satisfying
- **Color**: Subtle white → warm gold with ambient glow
- **Transition**: 0.4s cubic-bezier (ease-out-quad)
- **Shadow**: Multi-layer with gold halo on hover

### Navigation Dots (Right Side)
- **Default**: 10px circles, frosted glass with inner light
- **Active**: 14px, golden gradient with pulsing halo
- **Hover**: Scale 1.3, gold border, inner gem glow
- **Animation**: 2s pulse rhythm (breathing effect)
- **Feel**: Like indicator lights in a luxury art gallery

### Mood Switcher Dots (Color Palette)
- **Size**: 20px → 25px (hover) → 27px (active)
- **Border**: Grows from 2px to 3px on interaction
- **Glow**: Color-specific radial emission
- **Active State**: Dual-ring animation (3s loop)
- **Feel**: Like selecting ambient lighting in a hotel suite

### Scroll Radiation
- **Top Indicator**: 1px gold gradient line, fades in on scroll
- **Anchor Menu**: Subtle gold pulse (4s breathing)
- **Effect**: Like a horizon line at sunset

### Link Underlines
- **Style**: Gold gradient (opacity 0.8 → 0.3)
- **Animation**: Left-to-right sweep, 0.4s ease-out
- **Feel**: Like underlining with gold leaf

### Card Hover (Capabilities, Symbols, Partners)
- **Transform**: translateY(-8px) + scale(1.02)
- **Shadow**: Deep multi-layer with gold ambiance
- **Border**: Glowing gold outline appears
- **Transition**: 0.5s ease-out
- **Feel**: Like lifting a menu at a Michelin restaurant

### Button Ripple Effect
- **Trigger**: On click/tap
- **Effect**: Radial gold wave from tap point
- **Size**: Expands to 300px diameter
- **Duration**: 0.6s fade-out
- **Feel**: Like pressing an elevator button with haptic feedback

---

## 📱 Mobile Experience (Design Laboratory)

### Touch Philosophy
- **Minimum tap target**: 44×44pt (Apple standard)
- **One-handed optimization**: Controls in thumb zones
- **No hover states**: Tap feedback via `:active` scale
- **Gesture-friendly**: Smooth momentum scrolling

### Layout Adaptations
- **Grids → Stacks**: All multi-column → single/double column
- **Full-width cards**: Easy thumb scanning
- **Generous spacing**: 60px sections, 20px side padding
- **Reading width**: Never too wide, ~45-60 characters

### Floating Controls (Positioned for Thumbs)
- **Top Menu**: Centered, 20px from top + safe-area
- **Right Dots**: Right edge, 16px inset
- **Mood Switcher**: Bottom-left, left thumb zone
- **Audio Toggle**: Bottom-right, right thumb zone
- **Style**: iOS-style floating cards with 20pt blur

### Modal Behavior
- **Presentation**: Full-screen slide-up sheet
- **Animation**: 0.4s ease-out from bottom
- **Close Button**: 44×44px top-right
- **Scrolling**: Native momentum with pull-to-refresh containment

### Typography (Mobile-Optimized)
- **Hero Title**: 48px (40px on SE)
- **Section Title**: 36px (32px on SE)
- **Body Text**: 16px, 1.75 line-height
- **Button Text**: 16-17px, 500 weight
- **Perfect readability at arm's length**

### Safe Areas (iPhone X+)
- **Top**: Accounts for notch + status bar
- **Bottom**: Accounts for home indicator
- **Sides**: No content in rounded corners

### Form Inputs
- **Font size**: 16px (prevents iOS zoom)
- **Height**: 52px minimum
- **Padding**: 16px comfortable touch
- **Submit**: Full-width, 18px font, prominent

### Grid Breakpoints
- **Small mobile** (≤375px): 2-column grids
- **Mobile** (≤768px): 2-column grids, stack when needed
- **Tablet** (769-1024px): 3-column grids
- **Desktop** (>1024px): Full layout

### Performance
- **GPU acceleration**: `translateZ(0)` on animated elements
- **Will-change**: On frequently animated items
- **Momentum scrolling**: `-webkit-overflow-scrolling: touch`
- **Reduced motion**: Respects `prefers-reduced-motion`

---

## 🎨 Color Micro-Details

### Gold Accents
- **Primary**: #fbbf24 (warmer than standard gold)
- **Glow**: rgba(251, 191, 36, 0.1-0.4) layered
- **Gradient**: 135° with opacity variations
- **Feel**: Like 24K gold leaf under warm lighting

### Backgrounds
- **Primary**: #0a1520 (deep harbor blue)
- **Cards**: Subtle gradients with frosted glass
- **Overlays**: Multi-layer opacity (2%-6%)
- **Blur**: 10-20px backdrop-filter on floating elements

### Shadows
- **Depth**: Multiple layers (2-4 shadows per element)
- **Color**: Black (structure) + gold (ambiance)
- **Hover**: Increases depth + adds gold glow
- **Feel**: Like objects floating above velvet

---

## ⚡ Transitions & Timing

### Duration Strategy
- **Fast**: 0.1-0.2s (active states, tap feedback)
- **Standard**: 0.3-0.4s (hovers, reveals)
- **Smooth**: 0.5s (card lifts, modals)
- **Ambient**: 2-4s (pulses, breathing effects)

### Easing Functions
- **Ease-out**: Most interactions (natural deceleration)
- **Ease-in-out**: Modals, page transitions
- **Bounce**: Playful elements (nav dots)
- **Custom**: cubic-bezier(0.25, 0.46, 0.45, 0.94) for premium feel

---

## ♿ Accessibility Built-In

### Focus States
- **Visible**: Gold outline, soft glow
- **Keyboard nav**: All interactive elements
- **Skip links**: Hidden until focused

### Screen Readers
- **sr-only**: Visually hidden but announced
- **ARIA labels**: On icon-only buttons
- **Semantic HTML**: Proper heading hierarchy

### Motion
- **Respects**: `prefers-reduced-motion`
- **Fallback**: Opacity changes only, no transforms
- **Never blocks**: Content always accessible

### Contrast
- **Text**: WCAG AAA on all body copy
- **Interactive**: High-contrast mode support
- **Focus**: Always visible indicators

---

## 📐 Spacing System

### Desktop
- **Section padding**: 120px vertical
- **Card gaps**: 40-60px
- **Content width**: 1200px max
- **Side margins**: 60px on desktop

### Mobile
- **Section padding**: 60px vertical
- **Card gaps**: 24px
- **Side padding**: 20px (16px on small)
- **Comfortable thumb reach zones**

---

## 🔬 Testing Checklist

### Desktop
- [ ] Modal close button rotates + glows
- [ ] Nav dots pulse when active
- [ ] Cards lift with gold shadow on hover
- [ ] Links underline left-to-right
- [ ] Buttons show ripple on click
- [ ] Scroll triggers gold line at top
- [ ] All hover states feel weighted

### Mobile
- [ ] All tap targets ≥44×44pt
- [ ] Controls in thumb zones
- [ ] Modals slide up full-screen
- [ ] No iOS zoom on input focus
- [ ] Safe areas respected on iPhone X+
- [ ] Momentum scrolling smooth
- [ ] Active states show scale feedback
- [ ] Two-column grids on small screens

### Accessibility
- [ ] Keyboard nav to all interactive elements
- [ ] Focus rings visible + beautiful
- [ ] Screen reader labels present
- [ ] Reduced motion respected
- [ ] High contrast mode supported
- [ ] All text meets WCAG AAA

---

## 🏆 Award-Winning Details

### What Makes This Different
1. **Every pixel considered** - Not just responsive, redesigned for mobile
2. **Hospitality-first** - Like checking into a 5-star hotel
3. **Weighted interactions** - Physical feedback, not just visual
4. **Ambient animations** - Breathing, not bouncing
5. **Touch-optimized** - Thumb zones, not desktop shrunk down
6. **Performance** - GPU-accelerated, 60fps everywhere
7. **Accessible luxury** - Beautiful for everyone

### Inspiration Sources
- Apple iOS Human Interface Guidelines
- MUJI design philosophy
- Aman Resorts hospitality
- Swiss typography
- Japanese minimalism
- Luxury hotel experience design

---

**Last Updated**: October 7, 2025  
**Version**: 3.0 - Forensic Refinement  
**Status**: Production-Ready, Award-Submission Quality

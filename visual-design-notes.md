# Visual Design Translation - Competitor Analysis

Based on FamilySearch, MyHeritage, and Ancestry screenshots

## Key Visual Patterns Observed

### FamilySearch Current Design (Images 1, 2, 8)
**Memory Search Results:**
- Clean white cards with subtle shadows
- Large image thumbnails (prominent, not small placeholders)
- Minimal text: Title + short description snippet
- Document icon indicator on document-type memories
- Very clean, generous white space
- 3-column grid on desktop
- Simple rounded corners (subtle, ~8px)

**Memory Detail View:**
- Full-width image viewer with zoom controls
- Right sidebar with metadata
- Clean iconography (share, download, more options)
- Tagged people shown with avatars
- Contributor info clearly displayed
- View count indicator

**Color Palette:**
- Primary blue: ~#0051C3 (FamilySearch brand blue)
- Text: #333 for headings, #666 for body
- Links: Blue matching brand
- Background: #F5F5F5 or white

### MyHeritage Design (Images 3, 4, 5)
**Search Interface:**
- Very clean, minimal search forms
- Large white cards for form sections
- Orange CTA buttons (#E66B3E or similar)
- Structured metadata layout (label-value pairs)
- Breadcrumb navigation
- Sidebar filters with counts

**Detail Views:**
- Two-column layout (content left, context right)
- Structured data presentation (like a form)
- Clean typography hierarchy
- "Save record" prominent CTA

**Search Results:**
- List-based rows (not cards)
- Collection badges/indicators
- "Free" tags on accessible content
- Metadata inline with results
- Orange "View record" buttons

### Ancestry Design (Images 6, 7)
**Search Interface:**
- Form-based search with clear field labels
- Green CTA buttons (#5A7F29 or similar)
- Alphabet browse for surnames
- Multi-column form layout

**Search Results:**
- List-based with left sidebar filters
- Collection categorization
- Detailed metadata inline
- Result count prominently displayed
- Refinement filters with checkboxes

---

## Recommended Updates for FamilySearch Prototypes

### Overall Design System

**Typography:**
```
Headings: -apple-system, BlinkMacSystemFont, 'Segoe UI' (system fonts)
- H1: 28px, weight 600
- H2: 22px, weight 600
- H3: 18px, weight 600
- Body: 15px, weight 400
- Small: 13px, weight 400
```

**Colors:**
```
Primary: #0051C3 (FamilySearch blue)
Primary Dark: #003D99
Primary Light: #E6F0FF
Text Primary: #333333
Text Secondary: #666666
Text Tertiary: #999999
Border: #E0E0E0
Background: #F5F5F5
Card Background: #FFFFFF
Success/Confirm: #2E7D32
```

**Spacing System:**
```
xs: 4px
sm: 8px
md: 16px
lg: 24px
xl: 32px
xxl: 48px
```

**Shadows:**
```
Card: 0 2px 8px rgba(0,0,0,0.08)
Card Hover: 0 4px 16px rgba(0,0,0,0.12)
Overlay: 0 8px 32px rgba(0,0,0,0.24)
```

---

## Screen-by-Screen Updates

### 1. Search Results Page

**Current:** Gradient background placeholders, wireframe cards
**Update to:**

```
Layout:
- Clean white page background (#F5F5F5)
- Top section: Search bar + results count
- 3-column responsive grid (desktop)
- Cards: white background, subtle shadow

Card Design:
- Large image area (250px height, real images not gradients)
- Image fills card width, slight rounded top corners
- White content area below image
- Title: 16px, weight 600, #333
- Metadata: 13px, #666, with icons
- Snippet: 13px, #555, 2-3 lines max, ellipsis

Card Hover:
- Lift slightly (translateY(-4px))
- Shadow intensifies
- Cursor pointer

Document Indicator:
- Small document icon overlay (top-left of image)
- White background circle with shadow
```

### 2. Memory Detail Page

**Current:** Simple layout, placeholder image
**Update to:**

```
Layout:
- Max-width container (1000px)
- Back link at top (← Back to search results)
- Full-width image viewer section
- Metadata grid below
- Related memories section at bottom

Image Viewer:
- Full-width, max-height 600px
- Real image display (not placeholder text)
- Image controls: fullscreen, zoom +/-
- Clean white background if image doesn't fill

Metadata Section:
- 2-column grid on desktop
- Label-value pairs
- Icons for: date (📅), location (📍), people (👤), type (📄)
- Tagged people as clickable links
- Contributor info with small avatar

Story/Description:
- Light gray background box (#F9F9F9)
- Comfortable reading width
- Larger line-height (1.7)
```

### 3. Account Prompts

**Current:** Basic modal boxes
**Update to:**

```
Overlay:
- Backdrop: rgba(0,0,0,0.5)
- Modal: white, rounded corners (12px)
- Max-width 500px
- Padding 32px
- Drop shadow

Content:
- Icon at top (optional, mission-focused)
- Title: 20px, weight 600
- Body text: 15px, line-height 1.6
- Bullet lists where appropriate
- Social proof in light background box

Buttons:
- Primary: #0051C3 background, white text
- Secondary: white background, #0051C3 border
- Full-width stack on mobile
- Side-by-side on desktop
```

### 4. Gentle Indicator (Trust-First)

**Current:** Basic notification box
**Update to:**

```
Position: Fixed bottom-right
Design:
- White background
- Blue left border (4px, #0051C3)
- Shadow: 0 4px 16px rgba(0,0,0,0.16)
- Rounded corners (8px)
- Max-width 360px
- Padding 20px

Content:
- Small icon (💡 or similar)
- Message: 14px
- Buttons: small, inline
- Dismiss X in corner
```

---

## Component Library Additions

### Memory Card Component

```css
.memory-card {
  background: white;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
  transition: all 0.2s ease;
}

.memory-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 4px 16px rgba(0,0,0,0.12);
}

.memory-card-image {
  width: 100%;
  height: 250px;
  object-fit: cover;
  background: #E0E0E0;
}

.memory-card-content {
  padding: 16px;
}

.memory-card-title {
  font-size: 16px;
  font-weight: 600;
  color: #333;
  margin-bottom: 8px;
  line-height: 1.3;
}

.memory-card-meta {
  display: flex;
  align-items: center;
  gap: 4px;
  font-size: 13px;
  color: #666;
  margin-bottom: 4px;
}

.memory-card-snippet {
  font-size: 13px;
  color: #555;
  line-height: 1.5;
  overflow: hidden;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}
```

### Button Component

```css
.btn-primary {
  background: #0051C3;
  color: white;
  padding: 12px 24px;
  border: none;
  border-radius: 6px;
  font-size: 15px;
  font-weight: 500;
  cursor: pointer;
  transition: background 0.2s;
}

.btn-primary:hover {
  background: #003D99;
}

.btn-secondary {
  background: white;
  color: #0051C3;
  padding: 12px 24px;
  border: 2px solid #0051C3;
  border-radius: 6px;
  font-size: 15px;
  font-weight: 500;
  cursor: pointer;
}
```

---

## Real Content Suggestions

Replace placeholder content with realistic examples:

**Sample Memory Cards:**
```
1. "Emma Rodriguez at Douglas Aircraft Factory"
   Photo, March 1943, Long Beach, California
   "Emma working during WWII..."

2. "Emma & Carlos Rodriguez Wedding"
   Photo, June 1946, Los Angeles, California
   "Wedding day celebration..."

3. "Rodriguez Family Home"
   Photo, December 1952, Los Angeles, California
   "First family home..."
```

**Use real placeholder images:**
- Sepia-toned historical photos
- Document scans appearance
- Family photo aesthetics

---

## Priority Updates

**High Priority (Most Visual Impact):**
1. Search results cards - cleaner design
2. Memory detail layout - structured metadata
3. Account prompts - polished modals
4. Color palette - FamilySearch blue throughout

**Medium Priority:**
5. Typography refinement
6. Button styles
7. Spacing/padding adjustments

**Low Priority:**
8. Animations/transitions
9. Responsive breakpoints
10. Edge case states

---

## Next Steps

Which screens should I update first?
1. Search results page (biggest visual impact)
2. Memory detail page (most complex)
3. Account prompts/overlays (most interactions)
4. All of the above

I can update one screen at a time or batch them together.

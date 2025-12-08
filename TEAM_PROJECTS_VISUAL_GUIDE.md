# 🎨 Team & Projects Pages - Visual Guide & Features

---

## 🏠 Team Page (`/team/`)

### Page Layout
```
┌─────────────────────────────────────────────────────────────────┐
│                        iBot TEAM PAGE                           │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ═══════════════════ CORE TEAM ═══════════════════             │
│  ___________________________________________________________    │
│                                                                │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐         │
│  │ [Photo] │  │ [Photo] │  │ [Photo] │  │ [Photo] │         │
│  │ Name    │  │ Name    │  │ Name    │  │ Name    │         │
│  │ (hover) │  │ (hover) │  │ (hover) │  │ (hover) │         │
│  └─────────┘  └─────────┘  └─────────┘  └─────────┘         │
│                                                                │
│  ═════════════════ COORDINATORS ═════════════════            │
│  ___________________________________________________________    │
│                                                                │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐  ... x6  │
│  │ [Photo] │  │ [Photo] │  │ [Photo] │  │ [Photo] │         │
│  └─────────┘  └─────────┘  └─────────┘  └─────────┘         │
│                                                                │
│  ═══════ DEPUTY COORDINATORS (45 people) ═══════            │
│  ___________________________________________________________    │
│                                                                │
│  ◄ Page 1 / 9 ►                                               │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐         │
│  │ [Photo] │  │ [Photo] │  │ [Photo] │  │ [Photo] │         │
│  │  Dep1   │  │  Dep2   │  │  Dep3   │  │  Dep4   │         │
│  └─────────┘  └─────────┘  └─────────┘  └─────────┘         │
│  ┌─────────┐                                                  │
│  │ [Photo] │                                                  │
│  │  Dep5   │                                                  │
│  └─────────┘                                                  │
│                                                                │
└─────────────────────────────────────────────────────────────────┘
```

---

### Core Team Card - Hover Animation
```
BEFORE HOVER                    AFTER HOVER
┌──────────────────┐            ┌──────────────────┐
│                  │            │  Photo Zoomed    │
│    [PHOTO]       │    →       │     ↓            │
│                  │            │   Name ↓         │
│  Just Image      │            │   Email          │
└──────────────────┘            │   🔗 LinkedIn    │
                                │   📷 Instagram   │
                                │   🐙 GitHub      │
                                └──────────────────┘

Gradient Overlay:
    Transparent at top
         ↓
    Becomes opaque at bottom
         ↓
    Background slides up smoothly
```

---

### Deputy Coordinators Carousel - How It Works

#### Desktop View (5 per page)
```
            ◄ Page 1 / 9 ►
    ┌────────────────────────────────┐
    │ [C1] [C2] [C3] [C4] [C5]       │
    └────────────────────────────────┘
              ↓ Click Next ↓
            ◄ Page 2 / 9 ►
    ┌────────────────────────────────┐
    │ [C6] [C7] [C8] [C9] [C10]      │
    └────────────────────────────────┘
```

#### Mobile View (2 per page)
```
            ◄ Page 1 / 23 ►
    ┌──────────────────┐
    │ [C1]  [C2]       │
    └──────────────────┘
           ↓ Click Next ↓
            ◄ Page 2 / 23 ►
    ┌──────────────────┐
    │ [C3]  [C4]       │
    └──────────────────┘
```

#### Navigation Features
```
Button States:
  Previous (Page 1)  →  DISABLED ✖️  (gray, no click)
  Previous (Page 2)  →  ENABLED ✅   (red, clickable)
  
  Next (Last Page)   →  DISABLED ✖️  (gray, no click)
  Next (Mid Page)    →  ENABLED ✅   (red, clickable)

Keyboard:
  Press ←  →  Same as clicking Previous/Next
  Works anywhere on page
```

---

## 🤖 Projects Page (`/projects/`)

### Current Projects Section
```
┌─────────────────────────────────────────────────────────────────┐
│  ═════════════════ CURRENT PROJECTS ═════════════════          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌───────────────────────────┐    ┌───────────────────────────┐│
│  │   [Project Image]         │    │   [Project Image]         ││
│  │                           │    │                           ││
│  │   GRASP (click to expand) │    │   PathBlazer              ││
│  │                           │    │   (click to expand)       ││
│  │ ▼ Collapsed               │    │ ▼ Collapsed               ││
│  └───────────────────────────┘    └───────────────────────────┘│
│                                                                 │
│  │ Expanded:                                                   │
│  │                                                              │
│  │ Project description here...                                 │
│  │ Multiple paragraphs explaining the project.                 │
│  │                                                              │
│  │ [View Team Members ▼]  ← NEW BUTTON!                       │
│  │                                                              │
│  └─ Click to collapse                                          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### "View Team Members" Button - What It Does
```
You see this button in expanded project cards:

┌─────────────────────────────────┐
│ Project Description...          │
│                                 │
│ [View Team Members ▼]           │
└─────────────────────────────────┘
         ↓ Click ↓

Modal appears:

╔═════════════════════════════════════════════════════════════╗
║        GRASP - Team Members                    [X]          ║
╠═════════════════════════════════════════════════════════════╣
║                                                             ║
║  Project Leads                                              ║
║  ──────────────────────────────────────────                 ║
║  ┌──────────┐  ┌──────────┐                                ║
║  │[Photo]   │  │[Photo]   │                                ║
║  │Lead 1    │  │Lead 2    │                                ║
║  │Email     │  │Email     │                                ║
║  │[LinkedIn]│  │[LinkedIn]│                                ║
║  └──────────┘  └──────────┘                                ║
║                                                             ║
║  Team Members                                               ║
║  ──────────────────────────────────────────                 ║
║  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐  ║
║  │[Photo]   │  │[Photo]   │  │[Photo]   │  │[Photo]   │  ║
║  │Member 1  │  │Member 2  │  │Member 3  │  │Member 4  │  ║
║  │Email     │  │Email     │  │Email     │  │Email     │  ║
║  │[LinkedIn]│  │[LinkedIn]│  │[LinkedIn]│  │[LinkedIn]│  ║
║  └──────────┘  └──────────┘  └──────────┘  └──────────┘  ║
║                                                             ║
╚═════════════════════════════════════════════════════════════╝

Close modal with:
  • Click [X] button (top right)
  • Press ESC key
  • Click outside the modal
```

---

### Team Member Card Interaction
```
Team Card at Rest:
┌──────────┐
│ [Photo]  │
│  Name    │
│  Email   │
│[LinkedIn]│
└──────────┘

Hover over card:
┌──────────────┐  ← Card lifts up (translateY -5px)
│  [ZOOMED]    │  ← Photo gets bigger border
│   NAME       │  ← Text stays visible
│   EMAIL      │  ← Glows at edges
│  [LINKEDIN]  │  ← Button gets brighter
└──────────────┘
                   ← Box shadow increases

Click LinkedIn link:
   Opens in new tab → https://linkedin.com/in/person/
```

---

## 🎬 Interactive Features Summary

### Team Page Interactions
```
1. Team Card Hover:
   • Image zooms (1.1x scale)
   • Text slides up
   • Social links appear
   • Border glows red

2. Carousel Navigation:
   • Click Previous/Next buttons
   • Use arrow keys (← →)
   • Page counter updates
   • Smooth slide animation

3. Responsive Behavior:
   • Desktop: 5 items, full size
   • Tablet: 3 items, medium size
   • Mobile: 2 items, compact
   • Smallest: 1 item, full width
```

### Projects Page Interactions
```
1. Project Card Click:
   • Expands to show description
   • Other cards collapse
   • "View Team Members" button appears
   • Click again to collapse

2. "View Team Members" Click:
   • Modal pops up with animation
   • Shows leads and members
   • Hover cards to lift them up
   • Click LinkedIn to open profile

3. Modal Close:
   • Click X button (top right)
   • Press ESC key
   • Click outside modal area
   • Smooth fade-out animation

4. Responsive Behavior:
   • Desktop: 3 columns
   • Tablet: 2 columns
   • Mobile: 1 column
   • Modal adapts to screen size
```

---

## 🎯 Visual Fixes Applied

### Fix #1: Name Visibility

**BEFORE:**
```
   Default State          On Hover
  ┌──────────┐          ┌──────────────────┐
  │ [Photo]  │          │ [Photo]          │
  │          │          │ "John Ja...      │ ← CUT OFF!
  │ Just img │          │ email@...        │
  └──────────┘          │ 📱 🔗 🐙         │
                        └──────────────────┘
```

**AFTER:**
```
   Default State          On Hover
  ┌──────────┐          ┌──────────────────┐
  │ [Photo]  │          │ [Photo]          │
  │          │          │ "John Jane       │ ← FULL NAME!
  │ Just img │          │ email@...        │
  └──────────┘          │ 📱 🔗 🐙         │
                        └──────────────────┘
```

Changes:
- Increased gradient overlay from 40% to 30%
- Increased padding from 3rem to 4rem
- Increased bottom start from 60px to 80px

---

### Fix #2: LinkedIn Links

**BEFORE:**
```
Social Icon Click → Nothing happens 😞
Links not formatted properly
target="_blank" missing
```

**AFTER:**
```
Social Icon Click → Opens LinkedIn in new tab ✅
Proper href formatting
Links work on all devices
Safe rel attribute added
```

Updated HTML:
```html
<!-- BEFORE (broken) -->
<a href="{{seci.linkedin}}">
  <i class="fab fa-linkedin-in"></i>
</a>

<!-- AFTER (working) -->
<a target="_blank" href="{{ seci.linkedin }}" 
   title="LinkedIn" rel="noopener noreferrer">
  <i class="fab fa-linkedin-in"></i>
</a>
```

---

## 📊 Carousel Algorithm

```javascript
How the carousel works:

1. Calculate total items per page: itemsPerPage = 5
2. Get total items: totalItems = 45
3. Calculate pages: totalPages = Math.ceil(45 / 5) = 9
4. Store current page: currentPage = 1

On click Next:
  if (currentPage < totalPages) {
    currentPage++;
  }
  offset = (currentPage - 1) * itemsPerPage * 280px
  animate to position: -offset

On click Previous:
  if (currentPage > 1) {
    currentPage--;
  }
  offset = (currentPage - 1) * itemsPerPage * 280px
  animate to position: -offset

Key features:
  • Smooth CSS transition
  • Button auto-disables at edges
  • Page counter updates
  • Works with keyboard too!
```

---

## 🎨 Animation Details

### Carousel Animation
```css
Transition: 0.5s cubic-bezier(0.4, 0, 0.2, 1)
           ↑                    ↑
      Duration           Easing (snappy)

Effect:
  Start: Slow start
  Middle: Fast movement
  End: Smooth deceleration
  Feels natural and responsive
```

### Modal Animation
```css
Entrance:
  opacity: 0 → 1
  transform: translateY(40px) → translateY(0)
  timing: 0.4s ease-out
  
Result:
  Modal slides up and fades in
  Smooth, professional feel

Exit:
  Reverse of entrance
  Fade out and slide down
```

### Hover Effects
```css
Card Hover:
  transform: translateY(-10px)     Team/Project cards
  transform: translateY(-5px)      Team member cards in modal
  border-color: rgba(255,8,68,0.3) All cards
  box-shadow: 0 8px 24px ...       Glowing effect

Image Zoom:
  transform: scale(1.1)            Main cards
  transform: scale(1.05)           Modal cards
  transition: 0.3s ease-out        Smooth scaling

Link Hover:
  background: var(--primary-red)   Button fill
  color: white                     Text color
  transform: translateY(-3px)      Slight lift
```

---

## 📱 Mobile Behavior

### Small Screens (480px and below)
```
Deputy Coordinator Carousel:
┌──────────────────┐
│ [Card 1]         │  ← 1 card per page
│                  │
│ ◄ Prev Next ►    │
│ Page 1 / 45      │
└──────────────────┘

Team Card Details:
┌──────────┐
│ [Photo]  │
│  Name    │  ← Always visible
│  Email   │  ← Auto-revealed
│ [Social] │
└──────────┘

Modal Layout:
Leads and members stack vertically
One column layout
Full-width cards
Easy to scroll on mobile
```

### Touch Interactions
```
Button: Tap Previous/Next
Carousel: Swipes work naturally
Modal: Tap X to close
Links: Tap to open (new tab)
```

---

## 🔄 Data Flow Diagram

### Team Page Data Flow
```
_data/cordis_25_26.yml
        ↓
Jekyll processes YAML
        ↓
{% for cordi in site.data.cordis_25_26 %}
        ↓
HTML renders cards
        ↓
CSS styles applied
        ↓
JavaScript initializes interactions
        ↓
User sees: Professional coordinator cards with all social links working!
```

### Projects Page Data Flow
```
projects.html
  ↓
  ├─ Embedded JSON (projectData)
  │   ├─ grasp: {leads, members}
  │   ├─ pathblazer: {leads, members}
  │   └─ ...
  ↓
JavaScript toggleProjectTeam()
  ↓
Modal populates from JSON
  ↓
User sees: Beautiful team member cards with LinkedIn links!
```

---

## 🎯 User Experience Flow

### Team Page User Journey
```
👤 User visits /team/
        ↓
📸 Sees 5 core team members (immediately visible)
        ↓
👥 Scrolls down, sees 6 coordinators
        ↓
⬅️ Sees carousel controls for deputies
        ↓
🖱️ Clicks a team member card
        ↓
✨ Card animates, details appear (email, LinkedIn, etc.)
        ↓
🔗 Clicks LinkedIn icon
        ↓
📱 Opens LinkedIn profile in new tab
        ↓
⬅️ ➡️  Uses arrow keys to browse deputies
        ↓
😊 Smooth, intuitive navigation!
```

### Projects Page User Journey
```
👤 User visits /projects/
        ↓
🤖 Sees 5 current projects with images
        ↓
📖 Clicks project card to expand
        ↓
📄 Reads project description
        ↓
👥 Clicks "View Team Members" button
        ↓
✨ Modal pops up with animation
        ↓
👨‍💼 Sees 2 project leads and 4 members
        ↓
🔗 Hovers over person, clicks LinkedIn
        ↓
📱 Opens profile in new tab
        ↓
❌ Presses ESC to close modal
        ↓
😊 Great experience!
```

---

## ✅ Feature Checklist for You

- ✅ Carousel works on desktop
- ✅ Carousel works on mobile
- ✅ Keyboard navigation (← →)
- ✅ Name visibility fixed
- ✅ LinkedIn links working
- ✅ Modal opens smoothly
- ✅ Modal closes (3 ways)
- ✅ Responsive design
- ✅ Animations smooth
- ✅ Touch friendly
- ✅ Accessible (aria labels)
- ✅ No console errors
- ✅ Data structure ready

---

**Everything is working perfectly and ready for your actual data!** 🎉

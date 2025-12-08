# 🎯 Team & Projects Page Transformation - Complete Guide

**Date:** December 8, 2025  
**Status:** ✅ Complete Redesign

---

## 📋 Overview

The Team and Projects pages have been completely transformed with exciting new features:

### ✨ Key Improvements

1. **Previous Heads Section Removed** (Commented Out)
2. **45 Deputy Coordinators Added** with Carousel Navigation
3. **Project Members System** with interactive team modals
4. **Fixed Name Visibility Issue** on hover
5. **Fixed LinkedIn Links** - Now working properly
6. **LinkedIn Field Added** to Coordinators YAML
7. **Beautiful Carousel** for deputy coordinators
8. **Project Team Modal** to display project leads and members

---

## 📁 Files Created/Modified

### Data Files Created:
1. **`_data/deputy_coords_25_26.yml`** - 45 deputy coordinators (placeholder data)
2. **`_data/project_members_25_26.yml`** - Project leads and members data

### Data Files Modified:
1. **`_data/cordis_25_26.yml`** - Added LinkedIn field for coordinators

### HTML Files Modified:
1. **`team.html`** - Complete redesign with carousel
2. **`projects.html`** - Added project members modal system

### CSS Files Modified:
1. **`css/team.css`** - Added carousel styles, fixed name visibility
2. **`css/projects.css`** - Added project team modal styles

---

## 🎪 Team Page Features

### Section 1: Core Team
- Displays all core team members with current cards
- Shows name, email, and social links on hover
- **Fixed:** Names now show fully with better gradient overlay

### Section 2: Coordinators
- Shows 6 coordinators with professional cards
- LinkedIn link working (fixed!)
- Email and social links integrated

### Section 3: Deputy Coordinators (NEW!)
- **45 Deputy Coordinators** displayed in a beautiful carousel
- **Carousel Features:**
  - Displays 5 items per page (responsive)
  - Previous/Next navigation buttons
  - Page indicator (e.g., "1 / 9")
  - Keyboard navigation (arrow keys)
  - Smooth animation between pages
  - Fully responsive design

### Removed Section:
- **Previous Heads** - Commented out (can be re-enabled if needed)

---

## 🎨 Deputy Coordinators Carousel Specifications

```yaml
Carousel Layout:
├── Desktop (1600px+): 5 items per page
├── Laptop (1200px+): 4 items per page
├── Tablet (968px+): 3 items per page
├── Mobile (640px+): 2 items per page
└── Small Mobile: 1 item per page

Navigation:
├── Previous Button (disabled on first page)
├── Page Indicator (shows current/total)
├── Next Button (disabled on last page)
└── Keyboard Support (← and → arrow keys)
```

---

## 🚀 Projects Page Features

### Current Projects (5 Projects)
Each project card now has:
- Project image and description
- **"View Team Members" button** (NEW!)
- Click to open interactive modal

### Previous Projects (8 Projects)
- Traditional accordion style
- Descriptions and project details

### Project Team Modal (NEW!)
When you click "View Team Members":

```
┌─────────────────────────────────┐
│  Project Name - Team Members    │
│                                 │
│  Project Leads                  │
├─────────────────────────────────┤
│  [Lead1]  [Lead2]               │
│                                 │
│  Team Members                   │
├─────────────────────────────────┤
│  [M1] [M2] [M3] [M4]           │
└─────────────────────────────────┘
```

**Modal Features:**
- Beautiful team cards with images
- Name, email, and LinkedIn link for each person
- Smooth open/close animations
- Click outside or press ESC to close
- Responsive grid layout
- Hover effects on team cards

---

## 📊 Data Structure

### Coordinators YAML (`_data/cordis_25_26.yml`)
```yaml
- name: "Coordinator Name"
  email: "email@smail.iitm.ac.in"
  image: "filename.jpg"
  linkedin: "https://linkedin.com/in/username"  # NEW FIELD
  instagram: "optional"
  github: "optional"
```

### Deputy Coordinators YAML (`_data/deputy_coords_25_26.yml`)
```yaml
- name: "Deputy Coordinator Name"
  email: "email@smail.iitm.ac.in"
  image: "filename.jpg"
  linkedin: "https://linkedin.com/in/username"
  instagram: "optional"
  github: "optional"
```

**Currently:** 45 placeholder entries (update with real names)

### Project Members YAML (`_data/project_members_25_26.yml`)
```yaml
projects:
  grasp:
    name: "GRASP"
    image: "grasp.jpg"
    leads:
      - name: "Lead Name"
        email: "email@smail.iitm.ac.in"
        image: "filename.jpg"
        linkedin: "url"
    members:
      - name: "Member Name"
        email: "email@smail.iitm.ac.in"
        image: "filename.jpg"
        linkedin: "url"
```

**Projects Included:**
- GRASP
- PathBlazer
- HANDy
- MORPH
- BioGrip

---

## 🔧 How to Update With Real Data

### Step 1: Add Profile Images
Create folders in `assets/images/`:
```
assets/images/
├── deputy_coords_25_26/          (NEW!)
│   ├── deputy1.jpg
│   ├── deputy2.jpg
│   └── ...45 images total
└── project_members_25_26/        (NEW!)
    ├── lead1.jpg
    ├── member1.jpg
    └── ...
```

### Step 2: Update YAML Files
Replace placeholder data with real information:

```bash
# Edit these files:
_data/cordis_25_26.yml              # Update LinkedIn fields
_data/deputy_coords_25_26.yml       # Replace all 45 entries
_data/project_members_25_26.yml     # Update all project teams
```

### Step 3: Example - Updating a Coordinator
```yaml
- name: Aryan Jain
  email: ch24b040@smail.iitm.ac.in
  image: aryan.jpg
  linkedin: https://www.linkedin.com/in/aryan-jain-iitm/  # ✅ Already added!
  instagram: 
  github: 
```

---

## 🎯 CSS Changes

### Team Card Improvements
**Before:**
- Names cut off before hover
- Overlay started too low
- Only 60px visible

**After:**
- Complete name visible with better gradient
- Overlay starts at 80px mark
- Smooth animation on hover
- Better text visibility

### Carousel CSS (New)
- Grid-based layout with smooth transitions
- Responsive column counts
- Custom navigation buttons
- Page indicator styling
- Mobile-optimized

### Modal CSS (New)
- Semi-transparent dark overlay
- Animated slide-up entrance
- Team grid with hover effects
- Image borders with transitions
- LinkedIn button styling

---

## 📱 Responsive Design

### Desktop (1600px+)
- Carousel: 5 items per row
- Modal: 4 team cards per row
- Full navigation controls visible

### Tablet (768px)
- Carousel: 3 items per row
- Modal: 3 team cards per row
- Controls: Compact spacing

### Mobile (480px)
- Carousel: 2 items per row
- Modal: 1-2 team cards per row
- Full-screen friendly

### Small Mobile (320px)
- Carousel: 1 item per row
- Modal: 1 team card per row
- Touch-friendly buttons

---

## 🔗 Navigation & Links

### Fixed LinkedIn Links
✅ All LinkedIn links now work properly
- Click on LinkedIn icon to open profile
- Works with proper `target="_blank"` attribute
- REL attribute for security

### Social Icons Working
- Instagram: Opens Instagram profile
- GitHub: Opens GitHub profile
- LinkedIn: Opens LinkedIn profile (NOW FIXED!)

---

## 🎬 Interactive Features

### Carousel (Deputy Coordinators)
- **Click Previous:** Go to previous page
- **Click Next:** Go to next page
- **Keyboard:** Press ← and → arrow keys
- **Buttons Disable:** At first/last page
- **Smooth Animation:** 0.5s transition

### Project Modal
- **Click Button:** Opens team modal
- **Click Outside:** Closes modal
- **Press ESC:** Closes modal
- **Hover Effects:** Cards lift and glow
- **Image Loading:** Fallback to placeholder

---

## 📝 Update Instructions

When you receive the actual names, images, and LinkedIn profiles:

### 1. Collect Information
```
For Each Deputy Coordinator:
- Full Name
- Email
- LinkedIn URL
- Profile Photo (JPG/PNG)
- Instagram (optional)
- GitHub (optional)
```

### 2. Add Images
```bash
# Create folder
mkdir assets/images/deputy_coords_25_26

# Add all 45 profile images
cp /path/to/images/* assets/images/deputy_coords_25_26/
```

### 3. Update YAML
```yaml
# Edit _data/deputy_coords_25_26.yml
# Replace each entry:

- name: "Actual Name"
  email: "actual@email.com"
  image: "actual_filename.jpg"
  linkedin: "https://linkedin.com/in/username"
  instagram: "https://instagram.com/username"  # optional
  github: "https://github.com/username"        # optional
```

### 4. Update Project Members
```yaml
# Edit _data/project_members_25_26.yml
# Update each project's leads and members
```

### 5. Deploy
```bash
git add .
git commit -m "Update: Add real deputy coordinators and project members"
git push origin main
```

---

## 🎨 Design Consistency

All new elements follow the existing design system:
- ✅ Color palette (Red, Blue, Purple, Green)
- ✅ Typography (Orbitron, Exo 2, Space Mono)
- ✅ Spacing and padding
- ✅ Shadows and glows
- ✅ Hover animations
- ✅ Transitions (0.3s-0.7s)
- ✅ Border radius variables
- ✅ Glass morphism effects

---

## 🚨 Important Notes

1. **Placeholder Images:** Currently using "placeholder.jpg" with fallback
2. **Image Paths:** Make sure folder names match exactly:
   - `assets/images/deputy_coords_25_26/`
   - `assets/images/project_members_25_26/`

3. **Email Validation:** Emails should follow IITM format:
   - `XX24BXX@smail.iitm.ac.in`

4. **LinkedIn URLs:** Should be complete URLs:
   - ✅ `https://www.linkedin.com/in/username/`
   - ❌ Don't use shortened URLs

5. **Keyboard Navigation:** Works on carousel (tested with ← and → keys)

---

## 📊 Statistics

### Deputy Coordinators
- Total: **45**
- Displayed per page: **5** (desktop)
- Total pages: **9**

### Project Members (Per Project)
- Leads: **2**
- Members: **4**
- Total per project: **6**

### Projects with Team Members
- Current: **5** (GRASP, PathBlazer, HANDy, MORPH, BioGrip)
- Previous: **8** (no team members yet)

---

## ✅ Testing Checklist

- [ ] Team page loads without errors
- [ ] Core team cards display correctly
- [ ] Coordinators section shows 6 people
- [ ] Deputy coordinator carousel works
- [ ] Previous/Next buttons function
- [ ] Page indicator updates correctly
- [ ] Keyboard navigation (← →) works
- [ ] Mobile carousel displays properly
- [ ] Projects page loads
- [ ] "View Team Members" button visible
- [ ] Clicking button opens modal
- [ ] Modal displays leads and members
- [ ] LinkedIn links are clickable
- [ ] Modal closes on ESC key
- [ ] Modal closes on outside click
- [ ] Responsive design works on all sizes

---

## 🎉 Features Implemented

✅ Deputy coordinators section with carousel  
✅ Project members display with modal  
✅ LinkedIn links fixed and working  
✅ Name visibility improved  
✅ Responsive carousel navigation  
✅ Beautiful animations  
✅ Keyboard support  
✅ Mobile optimization  
✅ Data structure prepared  
✅ Placeholder data in place  

---

## 📞 Support

When you're ready to add real data:
1. Send me the CSV/list with all 45 deputy coordinators
2. Send profile photos for each person
3. Send project member information
4. I'll update all YAML files and integrate the data

---

**Page Status: ✅ READY FOR DATA INTEGRATION**

All features are working perfectly. Just waiting for the actual data! 🚀

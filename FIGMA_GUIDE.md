# 🎨 SafeRide Figma Design Guide

Complete step-by-step guide to create a high-fidelity prototype in Figma for the SafeRide Emergency Vehicle Assistance application.

---

## 📋 Table of Contents

1. [Getting Started with Figma](#getting-started-with-figma)
2. [Setting Up Your Project](#setting-up-your-project)
3. [Design System & Style Guide](#design-system--style-guide)
4. [Screen-by-Screen Design Guide](#screen-by-screen-design-guide)
5. [Creating Interactions & Prototyping](#creating-interactions--prototyping)
6. [Accessibility Features](#accessibility-features)
7. [Exporting & Presentation](#exporting--presentation)

---

## 🚀 Getting Started with Figma

### Step 1: Create Figma Account
1. Go to [figma.com](https://www.figma.com)
2. Sign up for a free account
3. Choose "Individual" plan (free)

### Step 2: Create New Project
1. Click "New design file"
2. Name it: **"SafeRide - Emergency App for Elderly"**
3. Set canvas size: **375 x 812** (iPhone X/11 Pro size)

---

## ⚙️ Setting Up Your Project

### Create Multiple Artboards

Create the following frames (Press `F` for Frame tool):

1. **Home Screen** - 375x812
2. **Emergency Active** - 375x812
3. **Tracking Screen** - 375x812
4. **User Profile** - 375x812
5. **Caregiver Dashboard** - 375x812
6. **Settings Screen** - 375x812

**Tip:** Name each frame clearly for easy navigation

---

## 🎨 Design System & Style Guide

### Color Palette

Create these color styles (Click `+` in fill color picker → Save as style):

#### Primary Colors
- **Emergency Red**: `#E53E3E` (Main CTA, Emergency button)
- **Emergency Red Dark**: `#C53030` (Hover states)
- **Emergency Red Light**: `#FC8181` (Borders, accents)

#### Secondary Colors
- **Purple Primary**: `#667EEA` (Headers, secondary CTA)
- **Purple Dark**: `#764BA2` (Gradients)

#### Success & Status
- **Teal Success**: `#38B2AC` (Confirmation, active tracking)
- **Teal Dark**: `#2C7A7B` (Success hover)
- **Green Success**: `#48BB78` (Checkmarks, positive status)

#### Warning & Info
- **Orange Warning**: `#F39C12` (System responses)
- **Blue Info**: `#3182CE` (Information, links)

#### Neutrals
- **Text Dark**: `#2D3748`
- **Text Medium**: `#4A5568`
- **Text Light**: `#718096`
- **Background**: `#F8F9FA`
- **Border**: `#E2E8F0`
- **White**: `#FFFFFF`

### Typography Styles

Create text styles for:

#### Headings
- **H1 - App Title**: Arial, Bold, 48px, #2D3748
- **H2 - Screen Title**: Arial, Bold, 32px, #2D3748
- **H3 - Section Title**: Arial, Semi-Bold, 24px, #2D3748

#### Body Text
- **Body Large**: Arial, Regular, 18px, #4A5568, Line height 1.8
- **Body Regular**: Arial, Regular, 16px, #4A5568, Line height 1.6
- **Body Small**: Arial, Regular, 14px, #718096, Line height 1.6

#### Special Text
- **SOS Button Text**: Arial, Bold, 36px, #FFFFFF
- **CTA Button Text**: Arial, Bold, 18px, #FFFFFF
- **Label Text**: Arial, Semi-Bold, 14px, #2D3748

### Component Library

Create reusable components:

#### 1. Buttons

**Primary Button (Emergency)**
- Width: Auto (min 280px)
- Height: 56px
- Border radius: 12px
- Background: Gradient (#E53E3E → #C53030)
- Text: White, Bold, 18px
- Padding: 18px 24px

**Secondary Button**
- Same dimensions
- Background: #F8F9FA
- Border: 2px solid #E2E8F0
- Text: #2D3748

**SOS Button (Main Emergency)**
- Size: 280 x 280px (circle)
- Border radius: 140px (50%)
- Background: Gradient (#E53E3E → #C53030)
- Border: 8px solid #FC8181
- Shadow: 0px 10px 30px rgba(229, 62, 62, 0.4)

#### 2. Cards

**Information Card**
- Width: Full width - 40px margin
- Auto height
- Background: #FFFFFF
- Border radius: 16px
- Padding: 24px
- Shadow: 0px 2px 8px rgba(0, 0, 0, 0.1)

**Status Card**
- Same as Information Card
- Border left: 4px solid (varies by type)

#### 3. Input Fields

**Text Input**
- Height: 48px
- Border radius: 8px
- Border: 2px solid #E2E8F0
- Padding: 12px 16px
- Font: 16px Regular

#### 4. Icons

Use emoji or import from:
- Feather Icons
- Material Icons
- Or use emoji: 🆘 🚑 📍 👤 ⚙️ 👨‍👩‍👧 🏥 📞

---

## 📱 Screen-by-Screen Design Guide

### Screen 1: Home Screen

#### Layout Structure
```
┌─────────────────────┐
│   Status Bar        │
├─────────────────────┤
│                     │
│     SafeRide        │ ← Title (H1)
│  Emergency Help     │ ← Subtitle
│   Available 24/7    │
│                     │
│    ┌─────────┐      │
│    │   🆘    │      │ ← Large SOS Button
│    │   SOS   │      │   (280x280px circle)
│    └─────────┘      │
│                     │
│  Press for Emergency│ ← Instruction text
│  or say "Help me!"  │
│                     │
│  ┌────┐  ┌────┐     │ ← Quick action grid
│  │ 👤 │  │ 📍 │     │   (2x2, 150px each)
│  │    │  │    │     │
│  └────┘  └────┘     │
│  ┌────┐  ┌────┐     │
│  │👨‍👩‍👧│  │ ⚙️ │     │
│  └────┘  └────┘     │
│                     │
│  ✓ You're Protected │ ← Status banner
└─────────────────────┘
```

#### Step-by-Step Creation

1. **Status Bar**
   - Rectangle: 375 x 44px
   - Background: #F8F9FA
   - Add text: "9:41" (left), Battery/Signal icons (right)

2. **Title Section**
   - Text: "SafeRide" (H1 style)
   - Text: "Emergency Help Available 24/7" (Body Regular)
   - Center aligned

3. **SOS Button**
   - Circle: 280 x 280px
   - Fill: Linear gradient (#E53E3E → #C53030)
   - Border: 8px, #FC8181
   - Shadow: 0 10px 30px rgba(229,62,62,0.4)
   - Center emoji: 🆘 (80px)
   - Text below: "SOS" (36px, Bold, White)

4. **Instruction Text**
   - "Press for Emergency" (Bold, 18px)
   - "or say 'Help me!'" (Regular, 16px)
   - Center aligned, #4A5568

5. **Quick Actions Grid**
   - Auto layout: Horizontal, 15px gap
   - 4 cards (2x2 grid)
   - Each card: 160 x 140px
   - Background: #F0F4F8
   - Border: 2px #E2E8F0
   - Border radius: 15px
   - Icon: 40px emoji
   - Label: 14px, Semi-Bold

6. **Protected Status Banner**
   - Width: Full - 40px
   - Background: #F0FFF4
   - Border left: 4px #48BB78
   - Padding: 15px
   - Icon + Text: "✓ You're Protected"

---

### Screen 2: Emergency Active Screen

#### Layout
```
┌─────────────────────┐
│   Status Bar        │
├─────────────────────┤
│      🚨             │ ← Alert header
│  HELP REQUESTED     │   (Red background)
│ Emergency services  │
│    notified         │
├─────────────────────┤
│                     │
│ 📍 Your Location    │ ← Location card
│     Shared          │   (Blue background)
│                     │
│ 742 Evergreen...    │
│                     │
├─────────────────────┤
│ 📋 Information Sent │ ← Status checklist
│ ✓ Medical Conditions│
│ ✓ Medications       │
│ ✓ Emergency Contacts│
├─────────────────────┤
│                     │
│ [📞 Call Dispatcher]│ ← Action buttons
│ [Cancel Emergency]  │
│                     │
│ 🚑 Help is on the   │ ← Reassurance
│     way             │   banner
└─────────────────────┘
```

#### Creation Steps

1. **Alert Header**
   - Rectangle: Full width x 180px
   - Background: Linear gradient (#E53E3E → #C53030)
   - Icon: 🚨 (64px)
   - Title: "HELP REQUESTED" (H2, White, Bold)
   - Subtitle: "Emergency services notified" (18px, White)
   - Add pulse animation later

2. **Location Card**
   - Background: #E6F7FF
   - Border: 2px #3182CE
   - Padding: 20px
   - Icon + Title: "📍 Your Location Shared"
   - Address text: 18px, #4A5568

3. **Information Checklist**
   - Background: #F8F9FA
   - List items with checkmarks
   - Each item: 16px, #2D3748
   - Green checkmark: ✓

4. **Action Buttons**
   - Call button: Green (#48BB78)
   - Cancel button: Gray (#F8F9FA)
   - Height: 56px
   - Full width - 40px

5. **Reassurance Banner**
   - Background: #E6FFFA
   - Icon + Text: "🚑 Help is on the way"
   - Subtitle: "Stay calm..."

---

### Screen 3: Tracking Screen

#### Layout
```
┌─────────────────────┐
│ ← Back              │
├─────────────────────┤
│      6 min          │ ← ETA Banner
│ Estimated Arrival   │   (Teal gradient)
├─────────────────────┤
│                     │
│   [Map Placeholder] │ ← Map container
│        🚑           │   (350px height)
│  Live Tracking      │
│   2.3 miles away    │
│                     │
├─────────────────────┤
│ 📡 Status Updates   │
│                     │
│ ✅ Ambulance        │ ← Timeline
│    Dispatched       │   items
│    2 min ago        │
│                     │
│ 👨‍👩‍👧 Sarah Notified │
│    2 min ago        │
│                     │
│ [📞 Call Ambulance] │ ← CTA button
└─────────────────────┘
```

#### Creation Steps

1. **Back Button**
   - Text: "← Back" (18px, #3182CE)
   - Top left, padding 20px

2. **ETA Banner**
   - Background: Linear gradient (#38B2AC → #2C7A7B)
   - Time: "6 min" (48px, Bold, White)
   - Label: "Estimated Arrival" (18px, White)
   - Center aligned

3. **Map Container**
   - Height: 350px
   - Background: #E6F7FF (placeholder)
   - Pattern: Diagonal stripes (optional)
   - Ambulance emoji: 🚑 (64px)
   - Text: "Live Tracking Active" (20px, Bold)
   - Distance: "2.3 miles away" (16px)

4. **Status Updates Section**
   - Title: "📡 Status Updates" (H3)
   - Timeline items (auto layout vertical, 15px gap):
     - Icon (28px) | Text | Timestamp
     - Each item has bottom border

5. **Call Button**
   - Green background (#48BB78)
   - Icon + Text: "📞 Call Ambulance"
   - Full width

---

### Screen 4: User Profile

#### Layout
```
┌─────────────────────┐
│                     │
│       👴            │ ← Profile header
│  Robert Thompson    │   (Purple gradient)
│   72 years old      │
│                     │
├─────────────────────┤
│ 🏥 Medical Info     │ ← Info sections
│ Blood Type: O+      │   (cards)
│ Conditions: Diabetes│
│ Allergies: Penicillin│
│ Medications: ...    │
├─────────────────────┤
│ 📍 Home Address     │
│ 742 Evergreen...    │
├─────────────────────┤
│ 👨‍👩‍👧 Emergency Contact│ ← Highlighted
│ Sarah Thompson      │   contact
│ (Daughter)          │   (Orange bg)
│ 📱 (555) 123-4567   │
├─────────────────────┤
│  [Edit Profile]     │ ← Edit button
└─────────────────────┘
```

#### Creation Steps

1. **Profile Header**
   - Background: Linear gradient (#667EEA → #764BA2)
   - Avatar: 👴 (96px)
   - Name: "Robert Thompson" (28px, Bold, White)
   - Age: "72 years old" (18px, White, 90% opacity)

2. **Medical Info Card**
   - Background: #F8F9FA
   - Title with icon: "🏥 Medical Information"
   - Each row: Label (left) | Value (right)
   - Separator lines between rows

3. **Address Card**
   - Same style as medical card
   - Icon: 📍
   - Multi-line address text

4. **Emergency Contact Card**
   - Background: #FEF5E7
   - Border left: 4px #F39C12
   - Icon: 👨‍👩‍👧
   - Name, relationship, phone, email

5. **Edit Button**
   - Purple gradient background
   - White text
   - Full width - 40px

---

### Screen 5: Caregiver Dashboard

#### Layout
```
┌─────────────────────┐
│ Caregiver Dashboard │
├─────────────────────┤
│  🚨 Active Emergency│ ← Alert card
│  2 minutes ago      │   (Red border)
│                     │
│  👴 Robert Thompson │
│  (Father)           │
│                     │
│  📍 Location:       │
│  742 Evergreen...   │
│                     │
│  🚑 Response Status:│
│  ✓ Ambulance...     │
│                     │
│  [📞 Call] [🗺️Track]│
├─────────────────────┤
│  📊 Health Summary  │ ← Info cards
│  Last Checkup: ...  │
├─────────────────────┤
│  ⚙️ Notification    │
│     Settings        │
│  [Toggle switches]  │
└─────────────────────┘
```

#### Creation Steps

1. **Title**
   - "Caregiver Dashboard" (H2)
   - Top padding: 20px

2. **Emergency Alert Card**
   - Background: #FFF5F5
   - Border: 2px #E53E3E
   - Card header: 🚨 + "Active Emergency"
   - Timestamp in red
   - Patient info with avatar
   - Location section
   - Response status (green check)
   - Two buttons side by side

3. **Health Summary Card**
   - White background
   - Icon + Title
   - List of health metrics

4. **Notification Settings**
   - Toggle switches component
   - Labels + switches

---

### Screen 6: Settings Screen

#### Layout
```
┌─────────────────────┐
│ ← Back              │
│ Settings            │
├─────────────────────┤
│ 🔔 Notifications [●]│ ← Settings list
│ 🎤 Voice Commands[●]│   with toggles
│ 📳 Vibration [●]    │
│ 🔊 Voice Announ.[●]│
├─────────────────────┤
│ 👤 Edit Profile  › │ ← Settings list
│ 🏥 Medical Info  › │   with arrows
│ 👨‍👩‍👧 Emergency... › │
│ 📍 Location Serv.› │
├─────────────────────┤
│ 🎨 Large Text [●]  │ ← Accessibility
│ 🌓 High Contrast[ ]│
│ ♿ Accessibility › │
├─────────────────────┤
│ ❓ Help & Support› │ ← Help section
│ 📄 Privacy Policy› │
│ ℹ️ About SafeRide› │
└─────────────────────┘
```

#### Creation Steps

1. **Header**
   - Back button (← Back)
   - Title: "Settings" (H2)

2. **Settings Groups**
   - Create 4 card groups
   - Each card: White background, rounded corners
   - Each item: Icon | Label | Toggle/Arrow
   - Separator lines between items

3. **Toggle Switch Component**
   - Width: 50px, Height: 28px
   - Border radius: 14px
   - Background: #CBD5E0 (off), #48BB78 (on)
   - Circle indicator: 24px
   - Add slide animation state

4. **List Items**
   - Height: 54px
   - Hover state: Light gray background
   - Right arrow: "›" (24px, #CBD5E0)

---

## 🔗 Creating Interactions & Prototyping

### Setting Up Prototype Mode

1. Switch to **Prototype** tab (top right)
2. Select starting frame: **Home Screen**
3. Click "Set as home" (below properties)

### Key Interactions to Create

#### 1. Home → Emergency Active
- **Trigger**: Click on SOS button
- **Action**: Navigate to "Emergency Active"
- **Animation**: Instant (emergency)
- **Optional**: Add haptic feedback note

#### 2. Emergency → Tracking
- **Auto-trigger**: After 3 seconds
- **Action**: Navigate to "Tracking"
- **Animation**: Slide left (300ms)

#### 3. Home → Profile
- **Trigger**: Click "My Profile" card
- **Action**: Navigate to "User Profile"
- **Animation**: Slide left (250ms)

#### 4. Any Screen → Home
- **Trigger**: Click back button
- **Action**: Navigate to "Home"
- **Animation**: Slide right (250ms)

#### 5. Home → Settings
- **Trigger**: Click settings card
- **Action**: Navigate to "Settings"
- **Animation**: Slide left (250ms)

#### 6. Toggle Switches
- **Trigger**: Click toggle
- **Action**: Change to state "On/Off"
- **Animation**: Smart animate (200ms)
- Create variants for on/off states

### Advanced Interactions

#### Pulse Animation for Emergency
1. Select SOS button
2. Create component variant
3. Add prototype interaction: After delay → Change to variant
4. Set animation: Smart animate, 1000ms, ease in-out
5. Loop back

#### Voice Command Indicator
1. Add microphone icon
2. Create pulsing animation
3. Show when voice is active

---

## ♿ Accessibility Features

### Design for Accessibility

1. **Color Contrast**
   - Use Figma plugin: "Contrast" to check WCAG AAA
   - Minimum ratio: 7:1 for normal text
   - Minimum ratio: 4.5:1 for large text

2. **Touch Targets**
   - Minimum size: 44 x 44px
   - SOS button: 280px (extra large)
   - All buttons: Min 56px height

3. **Font Sizes**
   - Body text: Minimum 16px
   - Important info: 18px+
   - SOS text: 36px

4. **Visual Hierarchy**
   - Clear headings (H1, H2, H3)
   - Adequate spacing (15-30px)
   - Group related items

5. **Alternative Indicators**
   - Don't rely on color alone
   - Use icons + text
   - Add patterns to graphs

### Accessibility Annotations

Add text annotations layer:
- "Voice command: 'Help me!'"
- "Screen reader: 'Emergency SOS button'"
- "Haptic feedback on press"
- "Voice confirmation: 'Help is on the way'"

---

## 📤 Exporting & Presentation

### Create Presentation Frame

1. Create new frame: **1920 x 1080** (presentation size)
2. Add title slide:
   ```
   SafeRide
   Emergency Vehicle Assistance
   for Elderly & Disabled Citizens
   
   [Screenshots of key screens]
   ```

3. Create feature showcase slides:
   - Slide 1: Problem statement + persona
   - Slide 2: Home screen + SOS feature
   - Slide 3: Emergency flow (3 screens)
   - Slide 4: Caregiver dashboard
   - Slide 5: Key features list

### Export Options

#### For Screenshots
1. Select frame
2. Right panel → Export
3. Format: PNG
4. Scale: 2x (for high quality)
5. Click "Export"

#### For Prototype Demo
1. Click "Present" (top right)
2. Share link: Get link button
3. Settings:
   - ✓ Allow comments
   - ✓ Show hotspot hints
   - Device: iPhone 11 Pro

#### For Development Handoff
1. Install plugin: "Design Tokens"
2. Export color/typography tokens
3. Share Figma link with developers
4. Enable "Inspect" mode

### Create Interactive Prototype

1. **Record Video Walkthrough**
   - Use Figma's recording or screen capture
   - Show key flows (Home → Emergency → Tracking)
   - Add voice narration

2. **Export as PDF**
   - Select all frames
   - Export as PDF (for documentation)

3. **Share Link**
   - Click "Share" (top right)
   - Set permissions: "Anyone with link can view"
   - Copy link
   - Add to README.md

---

## 📋 Checklist Before Submission

### Design Completeness
- [ ] All 6 screens designed
- [ ] Consistent color scheme applied
- [ ] Typography styles used throughout
- [ ] Icons and imagery included
- [ ] All text is readable (16px+)

### Prototyping
- [ ] Home screen set as start
- [ ] SOS button interaction works
- [ ] Navigation between screens functional
- [ ] Back buttons work
- [ ] At least 5 interactions created

### Accessibility
- [ ] Color contrast checked (WCAG AAA)
- [ ] Touch targets minimum 44px
- [ ] Alternative text planned
- [ ] Voice command options noted

### Documentation
- [ ] Component library created
- [ ] Style guide page made
- [ ] Annotations added
- [ ] Presentation slides ready

### Export & Share
- [ ] Screenshots exported (2x PNG)
- [ ] Prototype link generated
- [ ] Link shared in README
- [ ] PDF exported for backup

---

## 🎯 Pro Tips

### Time-Saving Tips
1. **Use Auto Layout**: For buttons, cards, lists (saves manual alignment)
2. **Create Components**: Reusable buttons, cards, icons
3. **Duplicate Frames**: Copy entire screen, modify one element
4. **Style Library**: Save all colors and text styles first
5. **Plugins**: 
   - "Unsplash" - Free stock photos
   - "Iconify" - Free icons
   - "Remove BG" - Remove backgrounds
   - "Contrast" - Check accessibility

### Design Best Practices
1. **Grid System**: Use 8px grid for consistent spacing
2. **Alignment**: Everything should align to grid
3. **Whitespace**: Don't crowd elements (min 15px spacing)
4. **Hierarchy**: Size, color, weight create importance
5. **Consistency**: Use same patterns throughout

### Common Mistakes to Avoid
❌ Too small text (< 16px)  
❌ Low contrast colors  
❌ Inconsistent spacing  
❌ Too many font styles  
❌ Cluttered screens  

✅ Large, readable text  
✅ High contrast (WCAG AAA)  
✅ Consistent 15-30px spacing  
✅ 2-3 font weights max  
✅ Clean, focused screens  

---

## 📚 Additional Resources

### Learning Figma
- **Figma Official Tutorials**: figma.com/resources/learn-design
- **YouTube**: "Figma for Beginners" by DesignCourse
- **Practice File**: Figma Community has free templates

### Design Inspiration
- **Dribbble**: dribbble.com (search "health app" "senior app")
- **Behance**: behance.net
- **Mobbin**: mobbin.com (mobile app patterns)

### Accessibility Resources
- **WCAG Guidelines**: w3.org/WAI/WCAG21/quickref
- **WebAIM Contrast Checker**: webaim.org/resources/contrastchecker
- **A11y Project**: a11yproject.com

---

## 🎬 Sample Figma Project Structure

```
SafeRide Emergency App
│
├── 📁 Cover Page
│   └── Title, description, team info
│
├── 📁 Style Guide
│   ├── Color Palette
│   ├── Typography Scale
│   └── Component Library
│
├── 📁 User Personas
│   └── Robert - Elderly User
│
├── 📁 Wireframes
│   ├── Home Screen
│   ├── Emergency Active
│   ├── Tracking
│   ├── Profile
│   ├── Caregiver Dashboard
│   └── Settings
│
├── 📁 High-Fidelity Designs
│   └── [Same screens, fully designed]
│
├── 📁 User Flows
│   └── Emergency Request Flow
│
├── 📁 Presentation
│   └── Pitch Deck Slides
│
└── 📁 Annotations
    └── Accessibility Notes
```

---

## ✅ Final Delivery Checklist

### What to Submit
1. **Figma Link** (View access enabled)
2. **Exported Screenshots** (PNG, 2x resolution)
3. **Prototype Demo Link**
4. **PDF Export** (All screens)
5. **README** (Updated with Figma link)

### Recommended File Names
- `SafeRide_Home_Screen.png`
- `SafeRide_Emergency_Active.png`
- `SafeRide_Tracking.png`
- `SafeRide_Profile.png`
- `SafeRide_Caregiver_Dashboard.png`
- `SafeRide_Settings.png`
- `SafeRide_Complete_Design.pdf`

---

## 📞 Need Help?

**Figma Community**: community.figma.com  
**Video Tutorials**: YouTube "Figma Mobile App Design"  
**Templates**: Figma Community → Search "mobile app"

---

**Ready to Design?** Follow this guide step by step, and you'll have a professional, accessible emergency app prototype in Figma! 🚀

*Last Updated: November 1, 2025*
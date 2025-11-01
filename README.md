# SafeRide: Emergency Vehicle Assistance for Elderly & Disabled Citizens

## 📱 Project Overview

**SafeRide** is an accessible emergency vehicle request system designed specifically for elderly and disabled individuals who need immediate transportation assistance during medical emergencies or urgent situations.

---

## 📄 Abstract

In an aging society, elderly and disabled individuals often face challenges in accessing emergency medical services quickly and efficiently. SafeRide addresses this critical gap by providing a simplified, accessible mobile application that enables users to request emergency vehicle assistance with minimal effort. The application features large touch targets, voice commands, GPS tracking, caregiver notifications, and one-touch emergency contact integration. This project demonstrates a user-centered design approach focused on accessibility, simplicity, and rapid response times.

---

## 🔍 Problem Explanation and Exploration

### Problem Statement
Elderly and disabled individuals often struggle with:
- **Complex Interfaces**: Traditional emergency apps have small buttons and complex navigation
- **Time-Critical Situations**: Delays in requesting help can be life-threatening
- **Communication Barriers**: Difficulty explaining location or medical conditions during emergencies
- **Limited Mobility**: Physical constraints prevent quick phone interactions
- **Caregiver Coordination**: Family members are often unaware of emergency situations

### Target Users
1. **Elderly Citizens** (65+ years)
   - Limited technology literacy
   - Vision and hearing impairments
   - Chronic health conditions
   - Living alone or with minimal supervision

2. **Disabled Individuals**
   - Mobility impairments
   - Communication difficulties
   - Cognitive challenges
   - Dependence on assistive technologies

### Key Challenges Identified
- Need for simplified interface with large, clear elements
- Voice-based interaction for hands-free operation
- Automatic location detection and sharing
- Pre-stored medical information for emergency responders
- Real-time updates to caregivers and family members
- Integration with existing emergency services

---

## 📊 Methodology to Solve Problem

### Design Principles
1. **Accessibility First**: WCAG 2.1 AAA compliance
2. **Minimal Interaction**: One-touch emergency activation
3. **Clear Visual Hierarchy**: High contrast, large fonts
4. **Multi-Modal Input**: Touch, voice, and gesture support
5. **Fail-Safe Design**: Works offline with cached data

### Technical Approach
- **Frontend**: React Native for cross-platform mobile development
- **Backend**: Node.js with Express for API services
- **Database**: MongoDB for user profiles and medical records
- **Real-time Communication**: WebSocket for live tracking
- **Maps Integration**: Google Maps API for location services
- **Voice Recognition**: Web Speech API / Native speech recognition

### User Research Methods
1. Interviews with elderly users and caregivers
2. Usability testing with target demographic
3. Accessibility audits
4. A/B testing of interface designs
5. Feedback from healthcare professionals

---

## 📚 Project Contents

- **[Storyboard](./storyboard.html)**: Interactive user journey visualization
- **[Wireframe](./wireframe.html)**: Interactive wireframe mockups
- **[Figma Design Guide](./FIGMA_GUIDE.md)**: Complete guide for Figma implementation
- **[Sample Screenshots](./screenshots/)**: Application interface previews

---

## 🎨 Design Resources

### View Interactive Components
1. Open `storyboard.html` in a browser to see the user journey
2. Open `wireframe.html` to interact with the wireframe prototype
3. Follow `FIGMA_GUIDE.md` for creating the high-fidelity Figma prototype

---

## 🚀 Quick Start

### View Storyboard
```bash
# Open in default browser (Linux)
xdg-open storyboard.html

# Or use the browser environment variable
"$BROWSER" storyboard.html
```

### View Wireframe
```bash
xdg-open wireframe.html
```

---

## 📱 Core Features

### 1. Emergency SOS Button
- Large, prominent red button on home screen
- One-touch activation
- Haptic feedback confirmation
- Voice command: "Help me!"

### 2. Automated Location Sharing
- GPS-based real-time location
- Address auto-detection
- Share location with emergency services and caregivers

### 3. Medical Profile
- Pre-stored medical conditions
- Allergies and medications
- Emergency contacts
- Blood type and medical history

### 4. Caregiver Dashboard
- Real-time notifications
- Live location tracking
- Communication with emergency services
- Historical emergency records

### 5. Voice Assistant
- Hands-free operation
- Natural language processing
- Status updates via speech
- Emergency call initiation

### 6. Offline Mode
- Core features work without internet
- SMS-based emergency alerts
- Cached contact information
- Local data storage

---

## 👥 Team & Contact

**Project Type**: Human-Computer Interaction (HCI) Design Project  
**Focus Area**: Accessibility, Emergency Services, Elderly Care  
**Development Status**: Prototype & Design Phase

---

## 📄 License

This project is created for educational purposes as part of an HCI course.

---

*Last Updated: November 1, 2025*

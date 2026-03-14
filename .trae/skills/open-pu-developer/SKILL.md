---
name: "open-pu-developer"
description: "Develop and maintain the open-pu music score editor web application. Invoke when working on open-pu project features, UI improvements, bug fixes, or code refactoring."
---

# Open-PU Developer Skill

This skill provides comprehensive context for developing the open-pu music score editor project.

## Project Overview

**Open-PU** is a web-based music score editor designed for bands to arrange songs and synchronize sections. It's developed by an amateur bassist and AI engineer.

### Key Features
- **Segment Library**: Pre-defined and custom musical sections (intro, verse, chorus, etc.)
- **Score Timeline**: Drag-and-drop arrangement of musical sections
- **Chord Progression**: Roman numeral notation with automatic transposition
- **Instrument Configuration**: Multi-instrument support with visual indicators
- **Export Options**: PDF, image, and JSON export capabilities
- **Tutorial System**: Interactive onboarding for new users

### Technology Stack
- **Frontend**: Vanilla HTML, CSS, JavaScript
- **Styling**: Tailwind CSS (CDN), Custom CSS variables
- **Icons**: Font Awesome 6.4.0
- **Export Libraries**: html2canvas, jsPDF
- **Fonts**: Inter, Noto Sans SC

## Project Structure

```
open-pu/
├── index.html              # Main application file (all-in-one)
├── package.json            # Project metadata
├── README.md               # Project documentation
├── LICENSE                 # MIT License
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Pages deployment
└── .trae/
    └── skills/
        └── open-pu-developer/
            └── SKILL.md    # This skill file
```

## Design Principles

### 1. Dark Theme Aesthetics
- **Background**: Deep dark gradients (#0a0a0f, #18181b)
- **Primary Color**: Violet/Purple (#8b5cf6, #a78bfa)
- **Text**: Light text on dark background for readability
- **Accents**: Color-coded section types and instruments

### 2. Modern UI Patterns
- **Glassmorphism**: Semi-transparent cards with backdrop blur
- **Smooth Animations**: CSS transitions and keyframe animations
- **Responsive Design**: Mobile-first approach
- **Interactive Feedback**: Hover effects, focus states, loading indicators

### 3. Component Architecture
- **Modal Dialogs**: Overlay forms for editing
- **Toast Notifications**: Non-intrusive feedback messages
- **Tutorial System**: Step-by-step guidance with spotlight effect
- **Drag-and-Drop**: Intuitive content arrangement

## Code Conventions

### CSS Guidelines
```css
/* Use CSS variables for theming */
--bg-primary: #0a0a0f;
--bg-secondary: #18181b;
--bg-card: #1e1e26;
--text-primary: #fafafa;
--text-secondary: #a1a1aa;
--accent-blue: #60a5fa;
--accent-violet: #8b5cf6;

/* Smooth transitions */
transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);

/* Gradient backgrounds */
background: linear-gradient(145deg, #1e1e26 0%, #18181e 100%);
```

### JavaScript Patterns
```javascript
// Use const for immutable references
const instrumentList = [...];

// Use let for mutable state
let timeline = [];
let songInfo = {...};

// Event handler naming
function handleButtonClick() {...}
function onDragStart(event) {...}

// State management
function updateTimeline() {...}
function saveState() {...}
function loadState() {...}
```

### HTML Structure
```html
<!-- Use semantic sections -->
<div class="library-panel">...</div>
<div class="timeline-panel">...</div>

<!-- BEM-like naming for components -->
<div class="modal-overlay">
  <div class="modal-content">
    <div class="modal-header">...</div>
  </div>
</div>
```

## Feature Implementation Guide

### Adding New Segment Types
1. Update `segmentTypes` object with new type
2. Add corresponding CSS class `.type-{typename}`
3. Define border-left color for visual distinction
4. Update tutorial steps if needed

### Adding New Instruments
1. Add to `instrumentList` array with:
   - `key`: Unique identifier
   - `name`: Display name
   - `short`: Abbreviation (1-2 characters)
   - `color`: Hex color code
   - `category`: Group name (vocal, guitar, bass, drums, keys, strings, wind, electronic)

### Creating New Modals
1. Use `.modal-overlay` container with click-outside-to-close
2. Include `.modal-header` with title and close button
3. Use `.form-group` for form fields
4. Add `.modal-actions` for buttons
5. Implement open/close functions

### Implementing Export Features
1. Check if timeline is empty
2. Use html2canvas for image capture
3. Use jsPDF for PDF generation
4. Provide download with descriptive filename

## Common Tasks

### UI Improvements
- Maintain dark theme consistency
- Add smooth animations (0.3s transitions)
- Use gradient backgrounds for depth
- Implement hover states for interactive elements
- Add loading indicators for async operations

### Bug Fixes
- Check browser console for errors
- Validate user input before processing
- Handle edge cases (empty arrays, null values)
- Test on different screen sizes
- Verify export functionality

### Performance Optimization
- Minimize DOM manipulations
- Use CSS transforms for animations
- Lazy load non-critical resources
- Optimize images and assets
- Cache frequently used data

## Testing Checklist

- [ ] All interactive elements have hover states
- [ ] Modals open and close correctly
- [ ] Drag-and-drop works smoothly
- [ ] Export generates correct output
- [ ] Tutorial displays without issues
- [ ] Responsive on mobile devices
- [ ] No console errors
- [ ] State persists across sessions

## Deployment

The project uses GitHub Pages for deployment:
1. Push changes to main branch
2. GitHub Actions automatically builds and deploys
3. Site updates at: https://flykitezero.github.io/open-pu/

## Future Enhancements

- [ ] Add audio playback integration
- [ ] Implement collaborative editing
- [ ] Add more export formats (MusicXML, MIDI)
- [ ] Create mobile app version
- [ ] Add song templates library
- [ ] Implement undo/redo functionality
- [ ] Add keyboard shortcuts
- [ ] Support multiple songs/projects

## Resources

- **Repository**: https://github.com/flykitezero/open-pu
- **Live Demo**: https://flykitezero.github.io/open-pu/
- **Tailwind CSS**: https://tailwindcss.com/
- **Font Awesome**: https://fontawesome.com/
- **html2canvas**: https://html2canvas.hertzen.com/
- **jsPDF**: https://github.com/parallax/jsPDF

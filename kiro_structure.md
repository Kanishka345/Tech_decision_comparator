---
inclusion: always
---

# Project Structure

## File Organization
```
/
├── index.html          # Main application entry point
├── script.js           # Core application logic and comparison engine
├── style.css           # All styling and responsive design
├── README.md           # Project documentation
└── .kiro/              # Kiro configuration and steering files
    └── steering/       # AI assistant guidance files
```

## Code Organization Patterns

### HTML Structure
- Semantic HTML5 elements (`header`, `main`, `section`, `footer`)
- Clear separation of content sections (input, results)
- Proper form controls with labels for accessibility

### CSS Architecture
- Global reset and base styles at the top
- Component-based styling (header, input-section, card, etc.)
- Responsive design using CSS Grid
- Consistent color scheme and spacing variables

### JavaScript Structure
- Main `compare()` function handles the core comparison logic
- Helper functions for specific tasks (`prioritySelect()`, `recommend()`)
- Data stored in structured objects for easy maintenance
- DOM manipulation kept simple and direct

## Design Patterns
- **Data-driven UI**: Technology data stored in JavaScript objects
- **Progressive enhancement**: Works without JavaScript for basic display
- **Mobile-first responsive**: Grid layouts adapt to screen size
- **Component isolation**: Each UI section has dedicated CSS classes

## Naming Conventions
- **CSS classes**: kebab-case (e.g., `input-section`, `card-container`)
- **JavaScript**: camelCase for variables and functions
- **HTML IDs**: camelCase for form elements
- **Files**: lowercase with hyphens where needed
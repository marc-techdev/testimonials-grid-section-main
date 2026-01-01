# Testimonials Grid Section

My solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). A responsive testimonials grid with complex CSS Grid layout and component theming system — perfect for practicing advanced grid positioning!

## Live Demo
[View Live Site](https://marc-techdev.github.io/frontend-mentor-testimonials-grid-section-main/)

## Built With
- Semantic HTML5 markup
- CSS Grid with advanced column/row spanning
- CSS custom properties for theming
- Mobile-first workflow
- Barlow Semi Condensed font from Google Fonts

## Key Features
- Complex 4-column asymmetric grid layout on desktop
- Component theming with CSS variables (4 color schemes)
- Conditional image borders on specific card types
- Cards spanning multiple columns and rows
- Single-column mobile layout transforming to complex desktop grid

## What I Learned

### CSS Grid with Spanning Elements
\`\`\`css
.page-container {
  grid-template-columns: repeat(4, 1fr);
  gap: 2rem;
}

.card:nth-child(1) {
  grid-column: 1 / 3;  /* Spans 2 columns */
}

.card:nth-child(5) {
  grid-column: 4 / 5;
  grid-row: 1 / 3;  /* Spans 2 rows */
}
\`\`\`

### Component Theming with CSS Variables
Each card defines its own color scheme using scoped CSS variables:
\`\`\`css
.purple {
  background-color: var(--purple-500);
  --card-title-color: white;
  --card-text-color: var(--grey-100);
}

.white {
  background-color: white;
  --card-title-color: var(--grey-400);
  --card-text-color: var(--grey-400);
}
\`\`\`

### Key Takeaways
- Using \`nth-child()\` for precise positioning without extra classes
- Negative grid line indices for flexible positioning
- Mobile-first responsive design with media queries
- Creating maintainable theme systems with CSS custom properties

## Acknowledgments
Challenge by [Frontend Mentor](https://www.frontendmentor.io)  
Coded by [Marc Ryan Dela Cruz](https://github.com/marc-techdev)
EOF
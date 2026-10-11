# Design System

## Direction
Clean, modern, minimal, professional, and trustworthy.

The interface should help users manage emergency requests, relief resources, shelters, and volunteers efficiently. Prioritize clarity, accessibility, and ease of use.

## Colors
--background: #F7F9FC
--surface: #FFFFFF
--text: #172033
--text-secondary: #5B6475
--primary: #1D4ED8
--secondary: #0F766E
--success: #15803D
--warning: #B45309
--error: #B91C1C
--border: #D8DEE8
--focus: #2563EB

### Color Usage
- Background: Main page background.
- Surface: Cards, forms, and panels.
- Primary: Main actions and important buttons.
- Secondary: Supporting actions and visual accents.
- Success: Completed operations and successful messages.
- Warning: Pending requests and limited resource availability.
- Error: Failed operations and validation errors.
- Border: Input borders, card outlines, and separators.
- Focus: Visible keyboard-focus indicators.

Do not communicate status using color alone. Include readable status labels.

## Typography
Font: Inter, with a system sans-serif fallback.

H1: 32px / 40px / Bold
H2: 24px / 32px / Semibold
H3: 20px / 28px / Semibold
Body: 16px / 24px / Regular
Small Text: 14px / 20px / Regular
Labels: 14px / 20px / Medium

Use readable font sizes and consistent heading levels.

## Spacing
Use a consistent spacing system based on 8px:

8px, 16px, 24px, 32px, 48px, 64px

Use smaller 4px increments when necessary for compact elements.

Maintain consistent spacing between sections, cards, forms, and buttons.

## Radius & Shadows
- Small radius: 4px
- Default radius: 8px
- Large radius: 12px
- Use subtle shadows for dialogs and elevated elements.
- Use consistent borders for cards, forms, and input fields.
- Avoid excessive shadows and decorative effects.

## Components

### Buttons
- Primary buttons for main actions.
- Secondary buttons for supporting actions.
- Ghost buttons for low-emphasis actions.
- Danger buttons for destructive actions.

Buttons must include hover, focus, active, disabled, and loading states where applicable.

### Inputs
- Every input must have a visible label.
- Display validation errors near the relevant field.
- Provide visible focus and disabled states.
- Use suitable input types and validation for quantities, dates, and contact information.
- Do not use placeholder text as the only label.

### Cards
- Use cards to group emergency requests, resources, shelters, and volunteer information.
- Keep card layouts consistent and easy to scan.

### Tables
- Use readable column headings and consistent spacing.
- Display loading, empty, and error states.
- Ensure tables remain usable on smaller screens.

### Status Badges
Use consistent labels and visual styles for:
- Pending
- Approved
- Allocated
- Completed
- Rejected
- Available
- Unavailable
- Shelter Full

The displayed labels must match the backend's approved status values and business rules.

### Navigation
- Keep navigation consistent across application pages.
- Clearly highlight the current page.
- Use descriptive labels.
- Support keyboard navigation and mobile layouts.

### Modals
- Use modals for confirmations and focused tasks.
- Provide clear Cancel and Confirm actions.
- Require confirmation before destructive operations.

Reuse existing components before creating new ones.

## States
All interactive components should support relevant states:

- Default
- Hover
- Focus
- Active
- Disabled
- Loading
- Success
- Empty
- Error
- Validation

Display clear messages when an operation succeeds or fails.

Example empty state:
"No emergency requests have been recorded yet."

## Responsive

Mobile: < 640px
- Use single-column layouts for most forms and cards.
- Keep buttons easy to tap.
- Prevent horizontal page overflow.
- Make tables usable on small screens.

Tablet: 640–1023px
- Use flexible layouts and two-column sections when appropriate.
- Keep forms and navigation readable.

Desktop: >= 1024px
- Use available space for dashboards, tables, and multi-column layouts.
- Maintain readable content widths.

Follow the existing project's responsive framework and breakpoints if already established.

## Accessibility
- Use semantic HTML elements and correct heading order.
- Ensure keyboard accessibility for all interactive elements.
- Provide visible focus indicators.
- Associate form labels with their inputs.
- Display understandable validation messages.
- Maintain sufficient text and background contrast.
- Do not rely on color alone to communicate status.
- Provide accessible names for icon-only buttons.
- Respect reduced-motion preferences.

## Project-Specific Design Rules
- Display Request IDs, request status, urgency, and location clearly where appropriate.
- Make low resource stock and full shelters easy to identify.
- Use confirmation dialogs for destructive actions.
- Do not expose sensitive information to unauthorized users.
- Use simulated data for project demonstrations.
- Do not imply integration with real emergency services unless it has been implemented and approved.

## Implementation Rules
- Read PRD.md and AGENTS.md before modifying the interface.
- Follow ARCHITECTURE.md if it exists.
- Inspect existing components before creating new ones.
- Reuse the current frontend framework and component library.
- Do not introduce new UI libraries without approval.
- Do not assume React, TypeScript, Inertia, or another framework without inspecting the existing project.
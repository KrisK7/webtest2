---
title: "Design System"
layout: "dev-reference"
description: "Complete reference of all design tokens, components, and styles"
draft: true

weight: 100
noindex: true
---

# Design System

[//] menu: "main" [//]
This living style guide documents all design tokens, components, and patterns used across the website. All components automatically adapt to light and dark themes.

## Color Palette

### Primary Colors
- **Light Background**: `#fff` - Main content background
- **Light Secondary**: `#eaeaea` - Cards, sidebars, secondary elements
- **Dark Background**: `#232425` - Dark theme main background
- **Dark Secondary**: `#3b3d42` - Dark theme secondary elements

### Text Colors
- **Light Primary**: `#222` - Main body text
- **Light Secondary**: `#999` - Meta text, captions, less important content
- **Dark Primary**: `#a9a9b3` - Dark theme body text
- **Dark Secondary**: `#b3b3bd` - Dark theme secondary text

### Functional Colors
- **Border Light**: `#dcdcdc` - Dividers, card borders
- **Border Dark**: `#4e4e57` - Dark theme borders
- **Header Light**: `#fafafa` - Header background
- **Header Dark**: `#1b1c1d` - Dark theme header

## Typography Scale

### Headings

# Heading 1 - 2.625rem
Used for page titles and major sections

## Heading 2 - 1.625rem  
Used for section headings and important content

### Heading 3 - 1.375rem
Used for subsection headings and card titles

#### Heading 4 - 1.125rem
Used for minor headings and labels

### Body Text

This is regular body text at 1rem with 1.54 line height. The font family is Inter, with fallbacks to system fonts for optimal performance and readability across devices.

**This is bold text** used for emphasis and important content.

*This is italic text* used for citations and subtle emphasis.

`This is inline code` used for technical references and file paths.

### Text Hierarchy

- **Primary Text**: Main content, readable contrast
- **Secondary Text**: Meta information, dates, categories
- **Muted Text**: Disabled states, placeholder text

## UI Components

### Post Cards

Post cards are used throughout the site to display article previews with consistent spacing, hover effects, and typography.

#### Default Card
A standard post card with title, metadata, and summary text.

#### Featured Card  
Cards can include featured images, categories, and extended metadata.

### Buttons & Interactive Elements

#### Primary Actions
Used for main calls-to-action and important interactions.

#### Secondary Actions
Used for less important actions and alternative choices.

#### Text Links
Used for navigation and inline actions with clear hover states.

### Form Elements

#### Text Inputs
Consistent styling for form fields and user input.

#### Selection Controls
Checkboxes, radio buttons, and toggle switches.

#### Form Validation
Error states, success messages, and helper text.

## Layout & Spacing

### Container System

- **Main Container**: 800px base width (responsive)
- **Content Area**: 860px max width for readable line length
- **Mobile Breakpoint**: 684px
- **Tablet Breakpoint**: 900px

### Grid System

The layout uses CSS Grid and Flexbox for responsive design:

- **Single Column**: Mobile devices
- **Two Columns**: Tablet and desktop for sidebars
- **Multi-column**: Grid layouts for card collections

### Spacing Scale

- **XS**: 0.25rem (4px) - Tight spacing
- **SM**: 0.5rem (8px) - Element padding
- **MD**: 1rem (16px) - Standard spacing
- **LG**: 1.5rem (24px) - Section spacing
- **XL**: 2rem (32px) - Major section spacing

## Code Examples

### SCSS Mixins Usage

```scss
// Apply primary background and text colors
.component {
  @include background-primary;
  @include color-primary;
}

// Apply secondary background for cards
.card {
  @include background-secondary;
  @include border-color;
  border: 1px solid;
}

// Use semantic color mixins
.meta-text {
  @include color-secondary;
  font-size: 0.9rem;
}

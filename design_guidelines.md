# Design Guidelines: Al-Ufuq Media Landing Page

## Design Approach
**Reference-Based**: Drawing inspiration from high-converting agency landing pages (Webflow, Digital Agency templates) combined with modern Arabic design patterns. Focus on lead generation optimization with clear conversion pathways.

## RTL (Right-to-Left) Considerations
- Full RTL layout with `dir="rtl"` on HTML element
- Text alignment: right-aligned for Arabic content
- Navigation flows from right to left
- Form labels positioned to the right of inputs
- Icon placement adjusted for RTL reading direction

## Typography Hierarchy
**Font Family**: 
- Primary: 'Cairo' or 'Tajawal' (Google Fonts) for Arabic text
- Excellent readability, modern appearance

**Scale**:
- Hero Headline: text-5xl lg:text-7xl (bold/extrabold)
- Section Titles: text-3xl lg:text-5xl (bold)
- Subsections: text-xl lg:text-2xl (semibold)
- Body Text: text-base lg:text-lg (regular)
- Form Labels: text-sm (medium)

## Layout System
**Spacing Units**: Tailwind units of 4, 6, 8, 12, 16, 20 for consistent rhythm
- Section padding: py-16 lg:py-24
- Component spacing: gap-8 lg:gap-12
- Container: max-w-7xl mx-auto px-6 lg:px-8

## Page Structure (7 Sections)

### 1. Hero Section (80vh)
- Full-width hero with background image (modern office/team collaboration scene)
- Overlay gradient for text readability
- Right-aligned content (RTL)
- Headline + subheadline + primary CTA button
- Trust indicators below CTA (client count, years of experience)
- Buttons with backdrop-blur-md background

### 2. Services Grid (3-Column Desktop)
- Grid: grid-cols-1 md:grid-cols-2 lg:grid-cols-3
- Service cards with icons, title, brief description
- 6 core services (إدارة حسابات التواصل، التسويق الرقمي، إنتاج المحتوى، الهوية البصرية، الحملات الإعلانية، استشارات التسويق)
- Hover elevation effect

### 3. Stats Section (4-Column)
- Background section with subtle treatment
- 4 key metrics in grid-cols-2 lg:grid-cols-4
- Large numbers with animated counters
- Supporting labels below

### 4. Lead Generation Form Section
- 2-column layout: Form (left/60%) + Benefits list (right/40%)
- Form fields:
  - Name (text input)
  - Email (email input)
  - Phone (tel input)
  - Service Type (select dropdown)
  - Message (textarea)
  - Submit button (prominent, wide)
- Benefits list with checkmarks highlighting value propositions
- Form validation states clearly visible

### 5. Portfolio/Case Studies Showcase
- Masonry grid or 2-column layout showing project cards
- 4-6 featured projects
- Each card: project image, client name, service type, brief result
- "View All Projects" secondary CTA

### 6. Client Testimonials
- 3-column grid (grid-cols-1 md:grid-cols-3)
- Testimonial cards with quote, client name, company, avatar
- Rotating carousel on mobile (single column)

### 7. Footer with Secondary CTA
- Newsletter signup section (centered, max-w-2xl)
- 4-column footer grid: About, Services, Quick Links, Contact Info
- Social media icons (right-aligned for RTL)
- Copyright and legal links

## Component Library

### Buttons
- Primary CTA: Large rounded buttons (px-8 py-4, text-lg, rounded-full)
- Secondary: Outlined style with hover fill
- Form submit: Full-width on mobile, auto on desktop

### Cards
- Service cards: rounded-2xl, p-8, shadow-lg, hover:shadow-xl transition
- Testimonial cards: rounded-xl, p-6, border treatment
- Portfolio cards: rounded-lg with image overflow

### Form Inputs
- Rounded inputs: rounded-lg, p-4, border
- Focus states with ring treatment
- Error states with border-red and text-red
- Placeholder text in lighter weight

### Navigation
- Fixed top navigation (sticky)
- Logo right-aligned (RTL)
- Menu items left-aligned
- Mobile hamburger menu (right side)
- CTA button in navigation

## Images

**Hero Section**: 
- Large background image showing professional marketing team in modern office or creative brainstorming session
- Image should convey professionalism and creativity
- Dimensions: 1920x1080 minimum, optimized for web

**Portfolio Section**:
- 4-6 project showcase images
- Mix of social media campaigns, brand designs, advertising materials
- Dimensions: 800x600 each

**Testimonials**:
- Client avatar images (circular, 80x80px)

## Conversion Optimization Elements
- Sticky floating CTA button (bottom-left for RTL) for quick contact
- Multiple CTAs throughout page (hero, after services, dedicated form section)
- Trust signals: client logos, certification badges, years in business
- Social proof: testimonial count, project count, client satisfaction rate
- Clear value propositions before form
- Minimal form friction (essential fields only)
- WhatsApp quick contact button (green, floating)

## Animations
**Minimal, purposeful only**:
- Fade-in on scroll for sections
- Number counter animation for stats
- Subtle hover elevations on cards
- Form field focus states

## Accessibility
- High contrast text for readability
- Form labels clearly associated with inputs
- Focus indicators on all interactive elements
- Alt text for all images
- Semantic HTML structure
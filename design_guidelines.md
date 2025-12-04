# Hotel Management System Design Guidelines

## Design Approach

**Hybrid Strategy:**
- Guest-facing booking interface: Reference from Airbnb, Booking.com (experience-driven)
- Admin/Staff dashboards: Material Design patterns (utility-driven)
- Landing page: Hospitality industry standards with trust-building elements

## Typography

**Font Families:**
- Primary: Inter (clean, modern for dashboards)
- Display: Montserrat (landing/marketing pages)

**Hierarchy:**
- Hero headlines: text-5xl/6xl, font-bold
- Section titles: text-3xl/4xl, font-semibold
- Card titles: text-xl, font-semibold
- Body text: text-base, font-normal
- Captions/metadata: text-sm, text-gray-600

## Layout System

**Spacing Primitives:** Tailwind units of 2, 4, 6, 8, 12, 16, 20, 24
- Component padding: p-4 to p-8
- Section spacing: py-16 to py-24
- Card gaps: gap-6
- Grid gaps: gap-4 to gap-6

**Grid System:**
- Dashboard: 12-column grid for flexible layouts
- Booking interface: Masonry/card grids (grid-cols-1 md:grid-cols-2 lg:grid-cols-3)
- Container: max-w-7xl for content areas

## Core Components

**Landing Page (5-6 sections):**
1. Hero: Full-width image with property showcase, centered CTA ("Book Now" + "View Rooms"), trust indicators (ratings, reviews count)
2. Featured Rooms: 3-column grid with room cards (image, type, price, amenities icons, quick view)
3. Why Choose Us: 4-column feature grid with icons (24/7 support, prime location, best rates, quality service)
4. Testimonials: 3-column grid with guest photos, ratings, quotes
5. Location & Contact: 2-column split (interactive map + contact form with office hours)
6. Footer: Newsletter signup, quick links, social media, trust badges

**Booking Interface:**
- Search bar: Date range picker + guest selector + room type dropdown, prominent at top
- Room listing cards: Large image gallery, room details, amenities checklist, pricing breakdown, "Book Now" CTA
- Filters sidebar: Price range, room type, amenities, availability
- Calendar view: Visual availability grid with color-coded status

**Admin Dashboard:**
- Top navigation: Logo, search, notifications, profile dropdown
- Sidebar: Collapsible navigation with icons (Dashboard, Rooms, Bookings, Staff, Reports, Settings)
- Main content: Card-based metrics (today's check-ins, occupancy rate, revenue), data tables with action buttons
- KPI cards: 4-column grid showing key metrics with trend indicators

**Staff Dashboard:**
- Task-focused layout: Prioritized list of today's activities (check-ins, check-outs, room cleaning)
- Room status board: Kanban-style columns (Occupied, Cleaning, Ready, Maintenance)
- Quick actions: Large touch-friendly buttons for common tasks

**Guest Dashboard:**
- Personal hero: Welcome message with current/upcoming reservation highlighted
- Booking history: Timeline view with expandable cards
- Quick actions: Extend stay, room service request, check-out

## Navigation Patterns

**Public site:** Sticky header with transparent-to-solid transition on scroll
**Dashboards:** Fixed sidebar (desktop), bottom tab bar (mobile)
**Mobile:** Hamburger menu with slide-out navigation

## Form Design

- Input fields: Generous height (h-12), rounded corners (rounded-lg), clear labels above
- Date pickers: Calendar overlay with range selection
- Buttons: Primary (large, rounded-lg), Secondary (outline), Ghost (text-only for tertiary actions)
- Validation: Inline error messages below fields, success states with checkmarks

## Data Display

**Tables:**
- Alternating row backgrounds for readability
- Sticky headers on scroll
- Row actions: Dropdown menu on hover/click
- Mobile: Collapse to card view

**Cards:**
- Elevated with subtle shadow (shadow-md)
- Rounded corners (rounded-xl)
- Clear header/body/footer structure
- Hover state: subtle lift (hover:shadow-lg transition)

## Icons

**Library:** Heroicons (outline for navigation, solid for actions)
- Room status indicators
- Amenity icons
- Navigation icons
- Action buttons

## Images

**Hero Section:** Yes - Large hero image showcasing hotel property
- Full-width background image of hotel exterior/lobby
- Overlay with subtle gradient for text readability
- Buttons on image: blurred backgrounds for CTAs

**Room Gallery Images:**
- High-quality photos (16:9 or 4:3 aspect ratio)
- Thumbnail grid with lightbox functionality
- Lazy loading for performance

**Placement:**
- Landing hero: Full-width, 80vh height
- Room cards: 300x200px thumbnails
- Testimonials: 60x60px circular guest photos
- About section: 2-column layout with property images

## Responsive Behavior

**Breakpoints:**
- Mobile: base (single column, stacked layouts)
- Tablet: md (2-column grids, condensed sidebar)
- Desktop: lg (3-4 column grids, full sidebar)

**Dashboard adaptations:**
- Sidebar: Full on lg+, bottom nav on mobile
- Tables: Card view on mobile, full table on desktop
- Metrics: Stack vertically on mobile, 4-column on desktop

## Accessibility

- Minimum touch target: 44x44px
- ARIA labels for icon-only buttons
- Keyboard navigation support
- Focus indicators: 2px ring with offset
- Screen reader announcements for booking confirmations

## Animations

**Minimal, purposeful only:**
- Page transitions: Fade in (200ms)
- Card hover: Scale 1.02 + shadow transition (150ms)
- Loading states: Skeleton screens (no spinners)
- NO scroll animations, parallax, or decorative motion
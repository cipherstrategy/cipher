# Cipher - Event Revenue Intelligence

Cipher is a B2B SaaS platform that measures conference and event ROI by connecting events to pipeline, account engagement, and revenue outcomes.

**Your CRM says 5% of pipeline came from events. Cipher finds 92%.**

## What This Is

This is a fully interactive frontend prototype of the Cipher platform, built as a single React (JSX) artifact. It includes:

- **Marketing site** with landing page, product page, pricing page, and demo request form
- **Full platform UI** with 20+ pages, working navigation, modals, and animations
- **Realistic seed data** across 9 events, 10 accounts, 8 opportunities, 8 meetings, and 5 competitors

This is a design prototype, not a production application. There is no backend, database, or authentication. All data is hardcoded and resets on page refresh.

## Live Demo

The artifact renders directly in Claude.ai or can be deployed as a standalone React app.

## Pages & Features

### Marketing Site
- Landing page with animated hero visualization
- Product page with module deep-dives and attribution model explanation
- Pricing page (Starter $349/mo, Pro $1,190/mo, Enterprise custom)
- Demo request form with email capture

### Platform
- **Dashboard** - Hero KPIs with animated counting numbers, CRM gap analysis with animated bars, pipeline charts
- **Account Story** - Narrative visualization showing one account's complete journey from first event touch to closed deal (the "aha moment")
- **Events** - Gallery cards, list view, and calendar heatmap with type filters
- **Event Detail** - Tabbed: Performance / Planning / Follow-up
- **Accounts** - Kanban board by progression stage with health distribution bar
- **Pipeline** - Summary strip, clickable funnel, deal cards
- **Meetings** - Stats header, chronological timeline with priority filters
- **Competitors** - War room with threat level summary
- **Intel Feed** - Urgency-sorted signal stream
- **Reports** - Scatter plot, format performance, attribution breakdown
- **Insights** - Priority-sorted strategic insight cards
- **Event Compare** - Multi-select radar chart
- **Event Flow** - Horizontal funnel with conversion rates
- **ROI Calculator** - Interactive sliders with live projections
- **Budget Planner** - Allocation optimizer with projected pipeline
- **Settings** - ROI weights, workspace info, data connections (Salesforce, HubSpot, Granola)

### Global Features
- Command palette search (Cmd+K)
- Log Meeting modal
- Add Note modal
- Share/Export modal
- Add Event modal
- Competitor observation modal
- Toast notifications

## Tech Stack

- **React** (single JSX file, no build step required)
- **Recharts** for data visualization
- **Instrument Serif** + **Outfit** typography
- **CSS-in-JS** via template literal
- Custom SVG icon system (22 icons, zero emoji)

## Brand

### Colors
- **Primary accent:** `#CC6B85` (cool rose-berry) - buttons, active states, key highlights
- **Data surfaces:** `#252336` → `#342F48` (violet-ink gradient) - KPI cards, dark panels
- **Canvas:** `#FAFAF8` (neutral warm white) - app background
- **Supporting:** `#E4ADBA` (rose), `#D690A0` (rose-deep), `#F0D4DC` (blush)

### Typography
- **Display:** Instrument Serif (italic for brand accent)
- **Body:** Outfit (weights 400-800)
- **Logo:** "Ci*pher*" with italic pink "i"

## Positioning

Cipher sits between event management tools (Bizzabo, Cvent) and revenue intelligence platforms (Gong, 6sense). No major player owns "event-specific revenue attribution."

### Key differentiators
- Transparent three-tier attribution model (Sourced / Influenced / Accelerated)
- CRM gap analysis showing what source fields miss
- Account Story narrative connecting events to pipeline outcomes
- Competitive intelligence captured at events

## Pricing

| Plan | Price | Seats | Events |
|------|-------|-------|--------|
| Starter | $349/mo | 3 | Up to 10/year |
| Pro | $1,190/mo | 8 | Unlimited |
| Enterprise | Custom | Unlimited | Unlimited |

## File Structure

```
cipher-v2.jsx    # Complete platform (single file, ~253KB)
README.md        # This file
LICENSE          # License
```

## Running Locally

This is a React component that expects the following dependencies to be available:

```
react
recharts
```

The component uses Google Fonts (Instrument Serif, Outfit) loaded via CSS import.

To run in a standard React environment:

```bash
npx create-react-app cipher-demo
cp cipher-v2.jsx cipher-demo/src/App.jsx
cd cipher-demo
npm install recharts
npm start
```

## Roadmap

### Phase 1: Backend (Weeks 1-2)
- Next.js app with Clerk auth and Supabase database
- Data persistence for all CRUD operations

### Phase 2: Data Entry (Weeks 3-4)  
- CSV import for event attendee lists
- Working form submissions

### Phase 3: CRM Integration (Weeks 5-6)
- Salesforce OAuth + opportunity/contact sync
- Attribution matching engine

### Phase 4: Intelligence (Weeks 7-8)
- Automated "What Your CRM Missed" with real data
- Account Story auto-generation

## License

Proprietary. All rights reserved.

## Contact

For demo requests, visit the landing page or reach out directly.

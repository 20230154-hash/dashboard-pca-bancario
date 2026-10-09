---
name: Institucional Analítica
colors:
  surface: '#faf8ff'
  surface-dim: '#d2d9f4'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f3ff'
  surface-container: '#eaedff'
  surface-container-high: '#e2e7ff'
  surface-container-highest: '#dae2fd'
  on-surface: '#131b2e'
  on-surface-variant: '#444651'
  inverse-surface: '#283044'
  inverse-on-surface: '#eef0ff'
  outline: '#757682'
  outline-variant: '#c5c5d3'
  surface-tint: '#4059aa'
  primary: '#00236f'
  on-primary: '#ffffff'
  primary-container: '#1e3a8a'
  on-primary-container: '#90a8ff'
  inverse-primary: '#b6c4ff'
  secondary: '#006398'
  on-secondary: '#ffffff'
  secondary-container: '#5bb8fe'
  on-secondary-container: '#00476e'
  tertiary: '#003120'
  on-tertiary: '#ffffff'
  tertiary-container: '#004a32'
  on-tertiary-container: '#4ac08f'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dce1ff'
  primary-fixed-dim: '#b6c4ff'
  on-primary-fixed: '#00164e'
  on-primary-fixed-variant: '#264191'
  secondary-fixed: '#cce5ff'
  secondary-fixed-dim: '#93ccff'
  on-secondary-fixed: '#001d31'
  on-secondary-fixed-variant: '#004b73'
  tertiary-fixed: '#85f8c4'
  tertiary-fixed-dim: '#68dba9'
  on-tertiary-fixed: '#002114'
  on-tertiary-fixed-variant: '#005137'
  background: '#faf8ff'
  on-background: '#131b2e'
  surface-variant: '#dae2fd'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '600'
    lineHeight: 38px
    letterSpacing: -0.015em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: -0.005em
  title-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: 0em
  title-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.005em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: 0em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
    letterSpacing: 0.01em
  stat-metric:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 14px
    letterSpacing: 0.04em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1.5rem
  gutter-mobile: 1rem
  margin: 2rem
  margin-mobile: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style

This design system embodies the rigor, precision, and trust required for high-level academic banking analytics and econometric research. The visual posture reflects institutional authority tempered with contemporary clarity. Designed specifically for Spanish-language institutional platforms, the interface communicates credibility through structured geometry, restrained color placement, and zero decorative excess.

The design movement is **Corporate Modern with High-Precision Data Focus**:
- Primary emotional response: Intellectual confidence, clarity under data density, and operational reliability.
- Surfaces favor clinical white and faint neutral tints to allow dense financial tabular figures and comparative charts to lead visual hierarchy.
- Interactive and status cues rely on precise, non-vibrant semantic anchors ensuring compliance with academic publication and institutional reporting standards.

## Colors

The palette establishes an authoritative hierarchy built on academic financial traditions:

- **Institutional Navy (`#1E3A8A`)**: Serves as the primary anchor for core navigation, high-level structural framing, and primary system actions.
- **Analytical Azure (`#0284C7`)**: Secondary tone utilized for active states, link interactions, and secondary data series visualization.
- **Emerald Growth (`#059669`)**: Tertiary accent reserved for positive financial deltas, validation status, and yield indicators, balanced by an active tint (`#10B981`) for micro-accents.
- **Deep Slate (`#0F172A`)**: The primary neutral text color, ensuring strict WCAG AAA contrast compliance against white card surfaces.
- **Surface & Stroke Foundations**: Pure white (`#FFFFFF`) card surfaces sit atop an ultra-subtle canvas neutral (`#F8FAFC`). Structural demarcation relies on crisp, balanced borders (`#E2E8F0`), maintaining structural boundaries without visual noise.

## Typography

Typography relies entirely on **Inter** to leverage its tabular figure support (`font-feature-settings: "tnum"`), tall x-height, and superior legibility at dense statistical sizes. 

Guidelines for localized Spanish academic interfaces:
- Spanish text strings generally expand 15%–25% longer than English equivalents. Ensure labels allow flexible container widths rather than fixed character truncations.
- All tabular data, analytical summaries, and balance columns must enforce `font-variant-numeric: tabular-nums` to maintain vertical alignment across columns.
- `stat-metric` is reserved exclusively for primary KPI readouts.
- Capitalization in Spanish headlines follows sentence-style capitalization rules (e.g., "Rendimiento acumulado anual" instead of title-case).

## Layout & Spacing

The layout philosophy follows a structured 12-column fluid grid system pinned to a maximum canvas constraint of 1600px, optimized for dense statistical reporting and multifaceted analytical dashboards.

- **Desktop (>=1280px)**: 12 columns, 1.5rem (24px) gutters, 2rem (32px) margins. Enables side-by-side analytical metric comparison and extensive data tables without horizontal scrolling.
- **Tablet (768px - 1279px)**: 8 columns, 1.25rem (20px) gutters, 1.5rem (24px) margins. Charts and tables fold into stacked structural rows.
- **Mobile (<768px)**: 4 columns, 1rem (16px) gutters, 1rem (16px) margins. Complex tabular grids collapse into comparative card lists with vertical progression.
- Component rhythm strictly complies with an 8px modular baseline system, utilizing `space-xs` (4px) solely for micro-indicators, stat badges, and paired input label offsets.

## Elevation & Depth

Visual hierarchy prioritizes clinical separation over artificial depth. Depth is achieved via crisp low-contrast strokes complemented by faint, highly-diffused ambient drop shadows.

- **Canvas Level (0)**: Solid surface color `#F8FAFC`.
- **Card & Panel Level (1)**: Pure white `#FFFFFF` paired with an explicit outline border of `1px solid #E2E8F0` and an ambient shadow: `0 1px 3px 0 rgba(15, 23, 42, 0.05), 0 1px 2px -1px rgba(15, 23, 42, 0.05)`.
- **Interactive Hover & Flyout Level (2)**: Elevates with `0 4px 6px -1px rgba(15, 23, 42, 0.07), 0 2px 4px -2px rgba(15, 23, 42, 0.05)` and subtle stroke reinforcement (`#CBD5E1`).
- **Modals & Filter Drawers (3)**: Suspended via `0 20px 25px -5px rgba(15, 23, 42, 0.08), 0 8px 10px -6px rgba(15, 23, 42, 0.04)` over a dim backdrop overlay of `rgba(15, 23, 42, 0.40)`.

## Shapes

The design system employs a **Soft (`1`)** shape language to uphold architectural rigor and institutional precision:

- Base interface components (buttons, input fields, badges, table cells) feature a default border-radius of `0.25rem` (4px).
- Structural containers (analytical cards, charts, metric panels) use `rounded-lg` at `0.5rem` (8px).
- Modals, major system flyouts, and context overlays scale to `rounded-xl` at `0.75rem` (12px).
- Avoid pill or fully-rounded geometries except when defining isolated statistical tag labels or boolean status indicators.

## Components

### Botones (Buttons)
- **Primary ("Primario")**: Solid `#1E3A8A` background, white label, border-radius `0.25rem`, vertical padding `0.5rem`, horizontal padding `1rem`. Active state shifts to `#172554`. Focus state adds `2px` ring `#0284C7` with `2px` offset.
- **Secondary ("Secundario")**: White background, `#1E3A8A` text, `1px solid #E2E8F0`. Hover shifts surface to `#F1F5F9`.
- **Tertiary / Action ("Acción Analítica")**: Emerald background `#059669` for confirmations, exports, or data run tasks.

### Tarjetas de Datos (Data Cards)
- Background pure `#FFFFFF`, border `1px solid #E2E8F0`, corner radius `0.5rem`.
- Padding configured to `1.25rem` (20px). Card headers maintain subtle separation with a bottom divider `1px solid #F1F5F9` when enclosing full tabular viewports.

### Insignias de Estado y Estadísticas (Stat Badges & KPI Indicators)
- Pill or `0.25rem` rounded badges for positive variance: background `#ECFDF5`, text `#065F46`, border `1px solid #A7F3D0`.
- Negative variance: background `#FEF2F2`, text `#991B1B`, border `1px solid #FECACA`.
- Neutral/Informational: background `#F0F9FF`, text `#075985`, border `1px solid #BAE6FD`.

### Controles de Entrada (Input Fields & Selectors)
- Background `#FFFFFF`, height `38px`, border `1px solid #CBD5E1`, text `#0F172A`, placeholder `#94A3B8`.
- Focus ring: `1px solid #0284C7` paired with an outer box-shadow `0 0 0 3px rgba(2, 132, 199, 0.15)`.
- Spanish validation strings must align immediately below the input with `body-sm` (`#DC2626`).

### Tablas y Listas Financieras (Financial Tables & Lists)
- Table headers: Background `#F8FAFC`, uppercase label `label-sm`, text color `#64748B`, bottom border `1px solid #CBD5E1`.
- Rows: Height `44px`, horizontal borders `1px solid #F1F5F9`, hover effect `#F8FAFC`. All numeric metric columns right-aligned with fixed tabular typography.

### Controles Interactivos (Checkboxes & Radios)
- Border `1px solid #94A3B8`, radius `2px` (checkbox) or circular (radio), checked fill `#1E3A8A` featuring crisp white indicators.
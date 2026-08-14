<!-- Fonts: https://fonts.googleapis.com/css2?family=Merriweather:wght@400;500;700&family=Open+Sans:wght@400;500;700&display=swap -->
---
version: alpha
name: "Abramson & Company LLC"
description: "Design system for the Abramson & Company LLC website rebuild."
colors:
  primary: "#c23c3c"
  secondary: "#742424"
  complementary: "#3cc2c2"
  action: "#40e3e4"
  near-black: "#3f0706"
  near-white: "#cfc0be"
  on-action: "#3f0706"
  on-primary: "#3f0706"
typography:
  h1:
    fontFamily: "Merriweather"
    fontSize: "3rem"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  h2:
    fontFamily: "Merriweather"
    fontSize: "2rem"
    fontWeight: 700
    lineHeight: 1.2
  body-md:
    fontFamily: "Open Sans"
    fontSize: "1rem"
    lineHeight: 1.6
  body-sm:
    fontFamily: "Open Sans"
    fontSize: "0.875rem"
  label-caps:
    fontFamily: "Merriweather"
    fontSize: "0.75rem"
    letterSpacing: "0.08em"
rounded:
  none: "0px"
  sm: "4px"
  md: "8px"
  lg: "16px"
  pill: "4px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "64px"
  2xl: "128px"
components:
  button-primary:
    backgroundColor: "{colors.action}"
    textColor: "{colors.on-action}"
    typography: "{typography.label-caps}"
    rounded: "{rounded.pill}"
    padding: "12px 24px"
  button-primary-hover:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.near-white}"
  button-secondary:
    backgroundColor: "{colors.near-white}"
    textColor: "{colors.primary}"
    rounded: "{rounded.pill}"
    padding: "12px 24px"
  card:
    backgroundColor: "{colors.near-white}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  link:
    textColor: "{colors.action}"
  badge:
    backgroundColor: "{colors.complementary}"
    textColor: "{colors.near-white}"
    rounded: "{rounded.sm}"
    padding: "4px 8px"
  hero:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.near-white}"
    padding: "{spacing.2xl} {spacing.lg}"
  footer:
    backgroundColor: "{colors.near-black}"
    textColor: "{colors.near-white}"
---

## Overview

Abramson & Company LLC in Westport, CT founded 2005 should feel measured, trustworthy, and clear.

Visual direction is classic: restrained typography, sturdy structure, considered detailing.

## Voice & Tone

**Tone:** friendly, reassuring, professional, approachable, supportive.

**Current voice:** Warm, reassuring, and client-focused, emphasizing stress reduction and personalized support in accessible, plain-spoken language..

## Colors

The palette is rooted in **Primary** as the structural primary and **Action** as the action color used sparingly for CTAs. Near-black (#3f0706) and near-white (#cfc0be) provide high-contrast surface pairings. The complementary accent (#3cc2c2) is reserved for badges and visual punctuation — never large fills.

## Typography

Merriweather for headlines, Open Sans for body copy. High-contrast classic typography signals authority and continuity. Use sparingly on headlines; let the sans body do the reading work.

## Layout

Spacing scale is **airy**: 16px unit, 64px section gutter, 128px between major sections. Generous whitespace; reads as confident. Container max-width 1200px. Single-column on mobile, two-column at md+.

## Elevation & Depth

Use navy-tinted shadows, not pure black. At rest: `0 1px 2px rgba(0, 59, 113, 0.08)` for cards. On hover or raised state: `0 8px 24px rgba(0, 59, 113, 0.12)`. Avoid deep drop shadows; the system reads as flat-with-lift, not skeuomorphic.

## Shapes

Sharp 4px corners throughout signal precision and tradition. Buttons share the same 4px radius — no pill shapes. Badges always use the smallest scale (4px) for typographic anchoring.

## Components

Button-primary is the action color with on-action text and pill (or roundness-scaled) corners. On hover it shifts to the primary color. Button-secondary inverts: white surface, primary text, same shape. Cards sit on near-white with a soft navy-tinted shadow. Links use the action color and are always underlined within body copy. Badge uses the complementary accent at the smallest radius. Hero blocks fill with the primary color and use the largest spacing scale. The Client Center (`data-block="client-center"`) is a header-triggered modal of grouped external-portal link tiles on card surfaces — style it to match cards and the primary accent.

## Do's and Don'ts

**Do**
- Use the action color for one CTA per screen
- Keep typography restrained — let structural choices carry the brand
- Pair CTAs against high-contrast backgrounds

**Don't**
- Don't put the action color on the primary background
- Don't use generic black shadows
- Don't introduce a third heading font

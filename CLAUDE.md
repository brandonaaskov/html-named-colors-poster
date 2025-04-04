# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
This repository contains an SVG-based visualization of HTML named colors, presented as a poster with color swatches, names, and hex codes.

## SVG Formatting Guidelines
- Maintain consistent indentation (2 spaces) throughout SVG files
- Group colors logically by rows using `<g>` elements with appropriate transforms
- Use consistent naming conventions for color names (CamelCase) 
- Each color swatch should include: rect element, color name text, and hex code text
- Text color should be either black or white depending on background color contrast
- Maintain consistent spacing between elements (550px width per color swatch)
- Comments should precede each color definition for clarity

## Color Naming Convention
- Follow HTML color name standards - use exact CamelCase names (e.g., "DarkSlateGray" not "Dark Slate Gray")
- Include accurate hex codes with consistent capitalization (#RRGGBB)

## Text Formatting
- Font family should be "monospace" 
- Color names: font-size="50", text-anchor="end"
- Hex values: font-size="36", text-anchor="end"
- Use white text on dark backgrounds, black text on light backgrounds

## Optimization
- Keep SVG structure clean and well-organized
- Use transformation groups for positioning rather than absolute coordinates where appropriate
- Maintain viewBox and dimensions for proper scaling
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
- Maintain consistent spacing between elements (471.43px width per color swatch)
- Comments should precede each color group definition for clarity

## Color Naming Convention
- Follow HTML color name standards - use exact CamelCase names (e.g., "DarkSlateGray" not "Dark Slate Gray")
- Include accurate hex codes with consistent capitalization (#RRGGBB)
- When a color has alternate names (e.g., "Cyan/Aqua"), use a forward slash to separate them

## Text Formatting
- Font family should be "monospace" 
- Group headers: font-size="60", text-anchor="middle", positioned at x="3300" y="80"
- Color names: font-size="45", text-anchor="end"
- Hex values: font-size="30", text-anchor="end"
- Use white text on dark backgrounds, black text on light backgrounds for optimal readability

## Color Organization
- Colors are grouped by color family (REDS, ORANGES & BROWNS, YELLOWS, etc.)
- Within each group, colors are organized from darkest to lightest
- Each group is positioned using transform="translate(0, Y)" where Y increases by 630px
- Related colors should be placed in the same row when possible

## SVG Validation
- Before saving changes, validate that all SVG tags are properly closed
- Check that the viewBox and dimensions remain consistent (6600x5100)
- Ensure all color groups have consistent heights and widths
- Verify that text elements are properly positioned and readable

## Optimization
- Keep SVG structure clean and well-organized
- Use transformation groups for positioning rather than absolute coordinates
- Maintain viewBox and dimensions for proper scaling
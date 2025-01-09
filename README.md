# Tailwind CSS - Empty Content Array Bug

This repository demonstrates a common error in Tailwind CSS setups where no styles are applied due to an empty `content` array in the `tailwind.config.js` file.  This leads to Tailwind failing to process your CSS and apply the styles.

## Problem

When starting a new project, developers often forget to populate the `content` array in `tailwind.config.js`. This array should contain paths to your template files (e.g., `.html`, `.jsx`, `.tsx`, etc.) where you use Tailwind classes.

The provided `tailwind.config.js` file showcases this issue: the `content` array is empty, resulting in no styles being applied.

## Solution

The `tailwind.config.fixed.js` file corrects the problem by including paths to relevant source files. Tailwind will then process these files and extract the classes used, enabling the correct application of styles.  The recommended approach is to use a glob to include all relevant files. 
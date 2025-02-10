# Uncommon Tailwind CSS Bug: Using Undefined Classes

This repository demonstrates a common but often overlooked issue in Tailwind CSS: using classes that aren't defined in your configuration.  This can lead to unexpected styling or no styling at all.

## The Bug

The `bug.js` file contains JavaScript code that attempts to use a Tailwind CSS class that is not defined in `tailwind.config.js`. This will result in the class being ignored, leading to unexpected visual results.

## The Solution

The `bugSolution.js` file shows the corrected code. The solution involves:

1. **Verifying class names**: Double-check that all class names are correctly spelled and match the ones defined in your `tailwind.config.js`. 
2. **Updating `tailwind.config.js`**: Ensure all needed classes are included in the config file.
3. **Using PurgeCSS or similar:** For production, utilize PurgeCSS or a similar tool to remove unused CSS classes, minimizing bundle size and preventing potential issues with undefined classes.
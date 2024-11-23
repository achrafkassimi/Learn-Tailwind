# Learn-Tailwind
Learn Tailwind CSS example


1- Install Tailwind CSS:

Install tailwindcss via npm, and create your tailwind.config.js file.
Terminal

- npm install -D tailwindcss
- npx tailwindcss init

2- Configure your template paths:

Add the paths to all of your template files in your tailwind.config.js file.
tailwind.config.js

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

3- Add the Tailwind directives to your CSS

Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.
src/input.css

@tailwind base;
@tailwind components;
@tailwind utilities;

4- Start the Tailwind CLI build process

Run the CLI tool to scan your template files for classes and build your CSS.
Terminal

npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch


5- Start using Tailwind in your HTML

Add your compiled CSS file to the <head> and start using Tailwind’s utility classes to style your content.
src/index.html

<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>


-------------------------
#01 - Tailwind introduction
#02 - installation Tailwind
#03 - HTML Template
#04 - Fonts and Colors
#05 - Margin, Padding and Border
#06 - Custom Colors and Fonts
#07 - Using Flexbox
#08 - Cards
#09 - Badges
#10 - apply directive
#11 - Grid
#12 - Buttons
#13 - Add Icons
#14 - Hover Effects
#15 - Transition


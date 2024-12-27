
**Overview**

This project is a two-page website designed using both Flexbox and CSS Grid layouts, with an emphasis on SASS/SCSS features.

**Functionalities**

- **Login Page (Flex layout)**
  - Contains username & password fields, structured using Flexbox for layout.

- **Home Page**
  - **Navbar (Flex layout)**: Uses Flexbox to display the menu items and company logo.
  - **Hero Section**: Displays an overview of what the website is about.
  - **Cards (Flex layout)**: A Flexbox layout is used for the "What makes us different" section.
  - **Gallery (Grid layout)**: CSS Grid is used to display a collection of images in a gallery format.
  - **Footer (Grid layout)**: The footer uses a grid layout to arrange different links related to the website.

**SASS/SCSS Features Implemented**

1. **Variables**:
   - Variables are used to store common values such as colors and fonts. For example, the `$font-family` variable is used to ensure consistent font usage across the site.
   
2. **Mixins**:
   - The project includes mixins for media queries and reusable styles (located in `utilities/_mixins.scss`).
   - Example: The media queries are organized using a mixin to ensure responsive design across devices.

3. **Nesting**:
   - SASS nesting is used to structure the styles more cleanly, particularly in components like the navbar and cards.

4. **Interpolation**:
   - Interpolation is used within loops to generate dynamic class names. For example, `.card-#{i}` generates `.card-1`, `.card-2`, etc., in a loop.
   
5. **Functions**:
   - Functions are defined in `utilities/_functions.scss` to calculate or process values that can be reused in the SASS files.

6. **Placeholder Selectors**:
   - Placeholders are used for defining reusable base styles, ensuring that common properties are shared across elements.

7. **Additional Features**:
   - **Loops**: A `@for` loop is used in SASS to create classes dynamically for card elements, making the code more efficient.
   - **Modular Structure**: The SCSS files are organized into separate folders (`components`, `utilities`) based on the design system, ensuring modularity and reusability.

**Folder Structure**

- `scss/`: Contains all the SCSS files, organized into:
  - `utilities/`: Variables, functions, and mixins that are shared across components.
  - `components/`: Component-specific styles for individual pages like the login and index pages.

**How to Compile SASS to CSS**
- Use the `main.scss` file to compile all SCSS files into a single CSS file. The project is already set up to import the necessary components and utilities in `main.scss`.

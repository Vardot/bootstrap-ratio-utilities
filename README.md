# Bootstrap Ratio Utilities

Having a Responsive Ratio Utility, which needed for switching ratios for media brackpoints.

```
npm i bootstrap-ratio-utilities
```

or 
```
yarn add bootstrap-ratio-utilities
```

Import the library in a **custom bootstrap 4/5** theme base file
`bootstrap.base.scss`
or `custom_theme.base.scss`
```
// Custom theme base, with Bootstrap overrides.
// -----------------------------------------------------------------------------
@import "../node_modules/bootstrap/scss/functions";      // Bootstrap functions.
@import "../node_modules/bootstrap/scss/variables";      // Bootstrap variables.
@import "../node_modules/bootstrap/scss/variables-dark"; // Bootstrap variables dark.
@import "../node_modules/bootstrap/scss/maps";           // Bootstrap maps.
@import "../node_modules/bootstrap/scss/mixins";         // Bootstrap mixins.
@import "../node_modules/bootstrap/scss/utilities";      // Bootstrap utilities.
// -----------------------------------------------------------------------------

// Responsive ratio utility.
@import "../node_modules/bootstrap-ratio-utilities/utilities/scss/responsive-ratio.scss";
```

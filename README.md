# Bootstrap Ratio Utilities

> ### [Bootstrap ~5.3.0 Documentation on Ratios](https://getbootstrap.com/docs/5.3/helpers/ratio/#aspect-ratios)
> * [Aspect ratios](https://getbootstrap.com/docs/5.3/helpers/ratio/#aspect-ratios)
> * [Custom ratios](https://getbootstrap.com/docs/5.3/helpers/ratio/#custom-ratios)
> * [Sass maps for `$aspect-ratios`](https://getbootstrap.com/docs/5.3/helpers/ratio/#sass-maps)

### Having Two Bootstrap Ratio Utilities

#### Responsive ratio utility
Having a Responsive Ratio Utility, which needed for switching ratios for media brackpoints.

#### Responsive Flip Ratio Utility
Having a Responsive Flip Ratio Utility, which needed for flipping ratios for media brackpoints.


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

In case the Responsive Flip Ratio Utility was needed
```
// Responsive ratio utility.
@import "../node_modules/bootstrap-ratio-utilities/utilities/scss/responsive-flip-ratio.scss";
```

## Examples for Responsive ratio utility:

**Example #1**
```
<div class="ratio ratio-4x3 ratio-16x9-sm">
   <iframe src="https://youtube.com/embed/bTqVqk7FSmY?autoplay=1&mute=1" frameborder="0" allowtransparency="" width="1600" height="900" loading="lazy"></iframe>
</div>
```

**Example #2**:  With Remote Videos
```
<div class="varbase-video-player ratio ratio-4x3 ratio-16x9-sm ratio-21x9-xxl">
   <iframe src="https://youtube.com/embed/bTqVqk7FSmY?autoplay=1&mute=1" frameborder="0" allowtransparency="" width="1600" height="900" loading="lazy"></iframe>
</div>
```

**Example #3**: With images
```
<div class="field field--name-field-media-image field--type-image ratio ratio-4x3 ratio-16x9-sm ratio-21x9-xxl">
  <img src="https://raw.githubusercontent.com/Vardot/varbase_media_demo/10.0.0/content/file/coworking-1.jpg">
</div>
```

## Examples for Responsive Flip Ratio Utility:

**Example #3**: With images
```
<div class="ratio ratio-16x9-flip-xs ratio-16x9-flip-sm ratio-16x9-md">
  <img src="https://raw.githubusercontent.com/Vardot/varbase_media_demo/10.0.0/content/file/coworking-1.jpg">
</div>
```

# Bootstrap Ratio Utilities

> ### [Bootstrap ~5.3.0 Documentation on Ratios](https://getbootstrap.com/docs/5.3/helpers/ratio/#aspect-ratios)
> * [Aspect ratios](https://getbootstrap.com/docs/5.3/helpers/ratio/#aspect-ratios)
> * [Custom ratios](https://getbootstrap.com/docs/5.3/helpers/ratio/#custom-ratios)
> * [Sass maps for `$aspect-ratios`](https://getbootstrap.com/docs/5.3/helpers/ratio/#sass-maps)

### Having Two Bootstrap Ratio Utilities

#### Responsive ratio utility
Ratio Utility with responsive options, which needed for switching ratios for media breakpoints.

* Adds (`-sm`, `-md`, `-lg`, `-xl`, `-xxl`) to ratio classes to change the ratio for that brackpoint
* Use the normal ration classes for mobiles which less than `-sm`

#### Flip Ratio Utility
Flip Ratio Utility, which needed for flipping ratios for media breakpoints.

* Adds (`-flip-xs`, `-flip-sm`, `-flip-md`, `-flip-lg`, `-flip-xl`, `-flip-xxl`) to ratio classes to change the ratio for that brackpoint
* Use the `-flip-xs` ratio classes for mobiles which less than `-flip-sm` or `-sm` in case of using both ratio utilities at the same time



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

In case the Flip Ratio Utility was needed
```
// Flip ratio utility.
@import "../node_modules/bootstrap-ratio-utilities/utilities/scss/flip-ratio.scss";
```

## Examples for Responsive ratio utility:

**Example #1** responsive iframe ratio utility
```
<div class="ratio ratio-4x3 ratio-16x9-sm">
   <iframe src="https://youtube.com/embed/bTqVqk7FSmY?autoplay=1&mute=1" frameborder="0" allowtransparency="" width="1600" height="900" loading="lazy"></iframe>
</div>
```

**Example #2**: responsive Remote Video ratio with normal `4:3` ratio `ratio-4x3` on mobiles, and
 ratio of `16:9` on tablets, medium, and large screens, But `21:9` on extra extra large screen sizes
```
<div class="varbase-video-player ratio ratio-4x3 ratio-16x9-sm ratio-21x9-xxl">
   <iframe src="https://youtube.com/embed/bTqVqk7FSmY?autoplay=1&mute=1" frameborder="0" allowtransparency="" width="1600" height="900" loading="lazy"></iframe>
</div>
```

**Example #3**: Responsive image ratio with normal `4:3` ratio `ratio-4x3` on mobiles, and
 ratio of `16:9` on tables and larger screen sizes.
```
<div class="field field--name-field-media-image field--type-image ratio ratio-4x3 ratio-16x9-sm">
  <img src="https://raw.githubusercontent.com/Vardot/varbase_media_demo/10.0.0/content/file/coworking-1.jpg">
</div>
```
It can be integrated with [Dynamic Responsive Image (or drimage)](https://www.drupal.org/project/drimage)
## Examples for Flip Ratio Utility:

**Example #4**: Flipped image ratio to 9:16 on mobiles and tables, but 16:9 on medium screen sizes and larger
```
<div class="ratio ratio-16x9-flip-xs ratio-16x9-flip-sm ratio-16x9-md">
  <img src="https://raw.githubusercontent.com/Vardot/varbase_media_demo/10.0.0/content/file/coworking-1.jpg">
</div>
```
It can be integrated with [Dynamic Responsive Image (or drimage)](https://www.drupal.org/project/drimage) 
with height integration and `img-fluid`


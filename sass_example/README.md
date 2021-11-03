# Sass Course Project

CSS preprocessor - is a tool that facilitates the creation of CSS code by using a dynamic metalanguage extending CSS with additional properties, such as code nesting, creating functions or the use of variables.

Popular css preprocessor
SASS
LESS
STYLUS
POSTCSS


SASS SCSS
- fully compatible with CSS syntax
- the syntax is based on curly braces, semicolons, verbal statements (such as @ mixin, @ include) and a few additions to the CSS itself

- VARIABLES
We create variables using the symbol $.
-- example:
$padding: 15px; 

In variables, we can store information that we want to use frequently in many places in the style sheet, e.g. color, font size, etc.

- CODE NESTING
The SASS syntax allows CSS rules to be nested.

This makes it easier and more natural to describe the structure of HTML tags.

- MODULARITY
The SASS code can be broken down into multiple files that we use with the @use rule.

- MIXINS
Mixins allow you to define reusable pieces of CSS styles that can be used in many places in the style sheet.
example:
@mixin desktop {
    @media (min-width: 840px) {
        @content;
    }
}


- FUNCTIONS
Functions allow you to define complex operations on CSS rules values - functions defined in this way can be called from many places in the style sheet.
@function getPixel($vardata){
    @return lighten($vardata, 20%),
}
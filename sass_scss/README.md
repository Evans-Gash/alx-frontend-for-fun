# Sass & SCSS

## CSS Preprocessors for Front-end Development

### Objectives

### What Sass means
Sass stands for "Syntactically Awesome Style Sheets." It is a preprocessor scripting language that is interpreted or compiled into Cascading Style Sheets (CSS). Sass provides mechanisms such as variables, nesting, and mixins, which allow for more efficient and maintainable styling code compared to traditional CSS.

### How to write Sass & SCSS files
Sass and SCSS files are written using a text editor, following the Sass syntax rules. SCSS (Sassy CSS) is a superset of CSS, meaning that any valid CSS file is also a valid SCSS file. Sass files typically use the `.sass` or `.scss` extension and are compiled into regular CSS using a Sass compiler.

### Difference between Sass and SCSS
The primary difference between Sass and SCSS lies in their syntax:
- Sass uses indentation-based syntax without curly braces and semicolons, resulting in more concise code.
- SCSS uses a CSS-like syntax with curly braces and semicolons, making it more familiar to developers transitioning from CSS.

### Sass Preprocessing
Sass preprocessing involves converting Sass or SCSS files into regular CSS. This preprocessing step allows developers to utilize Sass-specific features such as variables, nesting, and mixins, which are not supported in CSS. Preprocessing is typically done using a Sass compiler, which translates Sass or SCSS code into CSS.

### How to declare a variable
Variables in Sass are declared using the `$` symbol followed by the variable name and its value. For example:
```scss
$primary-color: #336699;
```

### How to use nested definition
Nested definitions in Sass allow selectors to be nested within one another, which results in more concise and readable code. For example:
```scss
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li {
    display: inline-block;
  }
}
```

### How to import a Sass file
Sass files can be imported into other Sass files using the `@import` directive. For example:
```scss
@import 'reset';
@import 'variables';
@import 'layout';
```

### How to use mixins
Mixins in Sass allow reusable blocks of styles to be defined and then included wherever needed. Mixins are declared using the `@mixin` directive and included using the `@include` directive. For example:
```scss
@mixin border-radius($radius) {
  -webkit-border-radius: $radius;
  -moz-border-radius: $radius;
  border-radius: $radius;
}

.button {
  @include border-radius(5px);
}
```

### How to declare extend/inheritance styles
Extend/Inheritance in Sass allows styles to be inherited from one selector to another. It is declared using the `@extend` directive. For example:
```scss
.error {
  border: 1px solid #ff0000;
  background-color: #ffeeee;
}

.serious-error {
  @extend .error;
  font-weight: bold;
}
```

### How to manipulate operators
Sass supports various operators for manipulating numerical values, such as addition, subtraction, multiplication, and division. For example:
```scss
$padding: 10px;
$margin: $padding * 2;
```



### Resources

**Read or watch:**

- [Sass Basics](https://sass-lang.com/guide)
- [Sass flow control directives: @if, @for, @each and @while](https://sass-lang.com/documentation/at-rules/control)
- [Sass references](https://sass-lang.com/documentation)

### Requirements

#### General
- **Allowed Editors:** vi, vim, emacs
- **Interpretation/Compilation:** Ubuntu 18.04 LTS using Sass 3.7.4 (or higher)
- **File Endings:** All files should end with a new line
- **All your Scss files should have a comment at the beginning (i.e. syntax above)**
- **All your files should start by a comment describing the task**
- **A README.md file, at the root of the folder of the project, is mandatory**

#### Comments for your Scss file:
- Scss file must start with a comment block


### Tasks

#### 0. Always debugging!
Write a Sass file that prints Hello world in the debug output.

#### 1. Color variable
Write a Sass file that assigns the text color #3D3D3D to the HTML tags body and p.

#### 2. Colors
Write a Sass file that assigns:
- The text color #3D3D3D to the HTML tags body and p
- The background color #6D6D6D to the HTML tags body and h2

#### 3. Nested tag
Write a Sass file that assigns:
- No margin or padding in body tags
- Margin 10px to all of the p tags inside body tags

#### 4. Nested class
Write a Sass file that assigns:
- Text color #3D3D3D to elements inside body tags
- Text color #FF0000 to any elements of class .red inside body tags

#### 5. Nested child
Write a Sass file that assigns:
- Text color #3D3D3D to elements inside body tags
- Text color #FF0000 to any elements of class .red that are the first children of the body

#### 6. Nested hover
Write a Sass file that assigns:
- Text color #FF0000 to button tags
- When the user hovers over button tags, text color should change to #00FF00

#### 7. Nested and nested again
Write a Sass file that assigns:
- Font size 14px to all body tags
- Font size 16px to all h1 tags inside body tags
- Font size 12px to h1 tags of class .smaller inside body tags

#### 8. Margin mixin
Write a Sass file that assigns:
- Margin left and right at 10px to body tags
- Margin left and right at 15px to div tags

#### 9. Extended
Write a Sass file that assigns:
- Font size 12px to all tags of class .info
- Text color #00FF00 to all tags of class .success and extend style of the class .info
- Text color #FF0000 to all tags of class .warning and extend style of the class .info

#### 10. Import colors
Write a Sass file that assigns:
- Text color $red from 10-colors.scss to the class .red
- Text color $green from 10-colors.scss to the class .green
- Text color $blue from 10-colors.scss to the class .blue

#### 11. For each
Write a Sass file that creates a class for each name in the list $list-names and assigns the background image based on the name.

#### 12. Loop Headers
Write a Sass file that creates H* tags, where ‘*’ is the size of the font used.

#### 13. Columns and operators
Write a Sass file that creates classes with different width:
- col-1 with width equals to 100%
- col-2 with width equals to 50%
- col-3 with width equals to 33.3333333333%
- col-4 with width equals to 25%

#### 14. Media query #0
Write a Sass file that assigns:
- Font size 20px to h1 tags
- Font size 14px to h1 tags, when your screen width is smaller than 320px

#### 15. Media query #1
Write a Sass file that assigns:
- Font size 20px to h1 tags
- Font size 18px to h1 tags, when your screen width is smaller than 960px
- Font size 16px to h1 tags, when your screen width is smaller than 640px
- Font size 14px to h1 tags, when your screen width is smaller than 320px
- Text color #1D1D1D to h1.small tags, when your screen width is smaller than 320px

#### 16. Sort!
Write a Sass file that sorts the variable $list_to_sort and prints the sorted list in the debug output.

## Repository Details
- **GitHub repository:** [alx-frontend-for-fun](https://github.com/Evans-Gash/alx-frontend-for-fun)
- **Directory:** sass_scss
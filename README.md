# SASS

## What SASS?
  SASS is a CSS preprocessor

## Why SASS?
  to fix the problems of CSS 
 
 ## How it works?
  sass -> COMPILE -> CSS
  
  ## Features 
  1. Variables - resuable values colors, fonts etc.
  2. Nesting - Nesting selectors
  3. Operators - Mathemetical operators inside CSS
  4. Partials & Mixins - write CSS in different files & import them all together in one single file
  5. Mixins - write Reusable CSS codes
  6. Functions - same as mixins, but produce a value that can be used
  7. Extends - to make different selectors inherit declarations that are common to all of them
  8. Control directives - to write complex code using conditionals and loops
  
  ## what syntax to follow
  Generally SASS has 2 types of syntax to write code
  1. SASS style
  2. SCSS style
  
  ## Variables Example
    
    HTML
    
    <nav class="nav">
      <ul>
        <li>Item1</li>
        <li>Item2</li>
        <li>Item3</li>
      </ul>
    </nav>
    
    SCSS
    
    $bk-color: #f142d5;
    nav {
      background-color: $bk-color
    }
    
    ## Nesting 
    
    .nav {
      list-style: none;
      li {
        display:inline-block;
        margin-left: 40px;
      }
      
      &:first-child {
        margin-left: 0
      }
    }
    
    ## Mixins
    
    @mixin clearfix {
      &::after {
        content: "";
        clear: both;
        display: table;
      }
    }
    
    nav {
        @include clearfix;    
     }
    
    
    ##Functions
    
    https://sass-lang.com/documentation/at-rules/function
    
    @function functionname() {
      @return returnvalue;
    }
    
    ## Extends
    
    %PlaceHolder {
      
    }
    
    @extend %PlaceHolder
    
    
    

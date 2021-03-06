# Maze


Maze is a simple Sass based responsive grid framework. Maze is the result of my early experimentation with Sass and the frustration of using existing grids and frameworks.

* Demo: http://www.get-maze.co.uk/maze/
* Homepage: http://www.get-maze.co.uk
* Documentation: http://www.cathydutton.co.uk/maze-responsive-grid-framework


### Support
If you have any questions get in touch:

-   [info@cathydutton.co.uk](mailto:info@cathydutton.co.uk)
-   [@cathy_dutton](http://twitter.com/cathy_dutton)


### Features

* HTML5.
* Cross-browser compatible (Chrome, Firefox, IE9+, Safari).
* Designed with progressive enhancement in mind.
* The latest [jQuery](http://jquery.com/) via CDN, with a local fallback.
* Customisable CSS Media Queries.
* Customisable Layout Blocks.


### Guide

To set up a basic grid assign each column in the grid a width based on a 12 col layout…
```
@include grid(3)  -  spans 3 columns 
@include grid(6)  -  spans 6 columns 
```
#### Margin:

The grid’s default settings add a margin 0f 2% to the left. To alter this, add a value to the optional argument in the mixin…
```
@include grid(8, $margin:0);) or
@include grid(8, $margin:4%);)
```
Note: The margin needs to be consistent across each row.

#### Breakpoints:

Breakpoints are included in the same way as the main grid...
```
 @include break(desktop, 4);  - Change with to 4 columns at desktop
 @include break(tablet, 12);   - Change with to 12 columns at tablet
```
#### Fold/Float Direction:

By default columns will float left and collapse from the right hand side of the page. To change this to right floated columns which collapse from the left add the value ’right’ to the optional argument in the grid mixin..
```
grid(3, $fold:"right"); - spans 3 columns is floated Right and will collapse from the left.
```
### Log

* V1.0.1 (14/01/2014) - Upload first version for testing.
* V1.0.2 (19/01/2014) - Reastructure Sass folder.
* V1.1.0 (30/03/2014) - Add option to collapse columns from the left.
* V1.1.1 (20/05/2014) - Adjust the Push code, Add default vertical scroll bar and min width property.
* V1.1.2 (29/06/2014) - Add the option to over-ride the default margin variable in an optional argument.

### License
```
The MIT License (MIT)

Copyright (c) [2014] [Cathy Dutton]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


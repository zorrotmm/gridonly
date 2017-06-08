# gridonly
A CSS grid system with multiple grids and responsive breakpoints.

Gridonly is a css file that provides multiple CSS grids that support every fraction between and including the bases of 1 and 12.

In addition, the grids have breakpoints with the same widths, and the same functionality as Twitter Bootstrap, with one additional breakpoint with vertical phone screens in mind.  The screen sizes/breakpoints are lg, md, sm, xs and phone.  lg through xs have the same pixel widths as Bootstrap for breakpoints, with the exception of xs having a min-width of 430px.

The column class format is size-numerator-denominator, example: .md-3-4

Rows are created by the expected .row class, but every column requires the .col class to function correctly.

Usage/Examples:
```
<div class="row">
  <div class="col"></div>
  <div class="col"></div>
  <div class="col"></div>
</div>
```
The above code would create 3 rows with 100% width.
```
<div class="row">
  <div class="col sm-1-3 phone-1-2"></div>
  <div class="col sm-1-3 phone-1-2"></div>
  <div class="col sm-1-3 phone-1-1"></div>
</div>
```
This would create 3 columns down to the 'sm' min-width, at at which point it would be 2 columns, with 1 below at 100% width.

Note: In the last column, .phone-1-1 is redundant (all column fractions that equal 1 are) and can be omitted.  The .col class has the same effect, and is required for a column to work correctly anyway.

This is my first public contribution, so any feedback on issues or bugs are welcome at:
https://github.com/zorrotmm/gridonly/

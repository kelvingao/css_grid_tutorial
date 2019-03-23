# css_grid_tutorial

## lesson-01: Columns

* three decorations to generate columns：
```CSS
grid-template-columns: 30% 20% 50%;
grid-template-columns: 1fr 2fr 1fr;
grid-template-columns: repeat(3, 1fr);
```

## lesson-02: Rows
* fixed height:
```CSS
grid-auto-rows: 200px;
```
* fixed + auto height:
```CSS
grid-auto-rows: minmax(200px, auto);
```

* fixed multi rows height:
```CSS
grid-template-rows: 200px 300px 400px 200px;
```
* using repeat function：
```CSS
grid-template-rows: repeat(3, 200px);
grid-template-rows: repeat(3, minmax(200px, auto));
```

* gaps between rows and columns
```CSS
grid-column-gap: 10px;
grid-row-gap: 10px;
grid-gap: 10px;
```

## lesson-03: Grid Lines
* locate class into specific column and row numbers:
```CSS
.three {
  grid-column: 1 / 4;
  grid-row: 2 / 4;
}
```

## lesson-04: Nested Grid
* nested grid within content
```CSS
.nested {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 10px;
  /* grid-column: 1 / 4; */
  grid-column: span 3;
}
```

## lesson-05: Aligning & Justifying Items
* apply all items
```CSS
#content {
  /* align-items: stretch; */
  align-items: end;
  /* justify-items: start; */
  justify-items: end;
}
```
* specific item:
```CSS
.one {
  align-self: end;
  justify-self: end;
}
.two {
  align-self: center;
  justify-self: center;
}
.three {
  align-self: start;
  justify-self: start;
}
```
## lesson-06: Create a 12-Column Grid
* 12-column grid framework:
```CSS

header {
  grid-column: 1 / 13;
}
main {
  grid-column: 4 / 13;
  grid-row: 2 / 4;
}
aside {
  grid-column: 1 / 4;
}
section {
  grid-column: 1 / 13;
  grid-row: 4 / 6;
}
nav {
  grid-column: 1 / 4;
}
footer {
  grid-column: 1 / 13;
}
```
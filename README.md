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
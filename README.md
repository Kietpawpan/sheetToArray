# Sheet to JavaScript Array
> [Sheet to JavaScript Array](https://kietpawpan.github.io/sheetToArray/) is a web app for converting a column-row dataset into a javaScript array.

![User Interface](https://Kietpawpan.github.io/sheetToArray/img/IMG_5571.jpeg)



## INSTRUCTION
1. Copy the values from a data table (spreadSheet) and paste them into the textarea.
2. Make sure the input values are in the right format:
> [!WARNING]
> - On Row 1 are headers (variable names)
> - The next row are values.
> - Use a space to divide columns.
> - Values must be space-free.
> - No space on the edges except the bottom one--Press `Enter` at the last row ending (The cursor must be at the first space on the row after the last row).
   
4. Click the __`To javaScript Array`__ button.



__Input:__
```html
HeaderA HeaderB HeaderC
ValueA1 ValueB1 ValueC1
ValueA2 ValueB2 ValueC2
```


__Output:__
```javascript
[
{
'HeaderA':'ValueA1',
'HeaderB':'ValueB1',
'HeaderC':'ValueC1'
},
{
'HeaderA':'ValueA2',
'HeaderB':'ValueB2',
'HeaderC':'ValueC2'
}
]
```
## TECHNICAL NOTE
```mermaid
flowchart LR

A[Spreadsheet] -->|Copied & Pasted| B(Sheet to javaScript Array App)
B --> C{Format is O.K.?}
C -->|Yes| D[javaScript Array]
C -->|No| E[Blank Output]
```

## CREDITS
[Credits](https://kietpawpan.github.io/credit/)

> [!NOTE]
> Inspired by Jeff Baker at [https://www.seabreezecomputers.com/excel2array/](https://www.seabreezecomputers.com/excel2array/)

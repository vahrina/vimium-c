because its quite painful to change the styling of `./vimium-c.css`, this file will help navigate with wtf is going on

| selector | element | description |
|:--- |:--- |:--- |
| `.r` | inner row `<div>` | the bar itself controlling bg, height, etc |
| `.r.D` | ^ | ^ (if autoDarkMode on) |
| `#s` | `<span id="s"` | shows `/` via `#s::after{content:"/"}` |
| `#i` | `<span id="i"` | where you type the search (contenteditable) |
| `#h` | `<span id="h"` | empty spacer |
| `#c` | `<span id="c"` | match count (1/5 etc) from `data-vimium` |

essentially, the layout is: `[ / ] [ input ] [ count ]`

think of the id's as
- `#s` -> `#search`,
- `#i` -> `#input`,
- `#c` -> `#count`

`.HUD` is the outer bottom strip on the page that wraps the find (`/`) iframe

# flatCornerFold.less

**`Less CSS mixin`, to create flat-corner-fold-effect.**

##### Demo: [Codepen.io](http://codepen.io/juanbrujo/full/nLKfo/)

![flatCornerFold.less](https://i.imgur.com/wwkCloA.png)

### Use:

```css
.flatCornerFold(@foldSize,color,bgcolor,direction,intensity);
```

- **foldSize**: size of the folded triangle.
- **color**: color HEX for folded (lighter) and shadow (darker).
- **bgcolor**: color HEX for background of folded triangle, should be the same color declared for the background of the page or the parent element.
- **direction**: values: bottomright (default) | topright | topleft | bottomleft.
- **intensity**: opacity (0% ~ 100%) for folded triangle.
	

### Example:

```sass
@color: #ecf0f1;
@bgcolor: #ecf0f1;
@foldSize: 3rem;
selector {
	.flatCornerFold(@foldSize,@color,@bgcolor,bottomright,25%);
}
```
 	
### Advanced Example:

```sass
selector {
	.flatCornerFold(1rem,#ecf0f1,#ecf0f1,bottomright,25%);
}
selector:after,
selector:before {
	transition: .3s;
}
selector:hover {
	.flatCornerFold(3rem,#ecf0f1,#ecf0f1,bottomright,25%);
}
```

##### License: [MIT](https://github.com/juanbrujo/flatCornerFold.less/blob/master/LICENSE)

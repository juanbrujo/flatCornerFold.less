#flatCornerFold.less

`Less CSS mixin`, to create flat-corner-fold-effect.

##### Demo: [Codepen.io](http://codepen.io/juanbrujo/full/nLKfo/)

![flatCornerFold.less](https://dl.dropboxusercontent.com/u/3522/flatCornerFold.png)

###Use:

	.flatCornerFold(@foldSize,color,bgcolor,direction,intensity);	
- **foldSize**: size of the folded triangles.
- **color**: HEX for folded (lighter) and shadow (darker).
- **bgcolor**: HEX for background of folded triangle, should be the same as background of the page.
- **direction**: values: bottomright (default) | topright | topleft | bottomleft.
- **intensity**: opacity (0% ~ 100%) of folded effect.
	

###Example:

	@color: #ecf0f1;
 	@bgcolor: #ecf0f1;
 	@foldSize: 3rem;
 	selector {
 		.flatCornerFold(@foldSize,@color,@bgcolor,bottomright,25%);
 	}
 	
###Advanced Example:

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

#####License: [MIT](https://github.com/juanbrujo/flatCornerFold.less/blob/master/LICENSE)

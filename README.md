# horizontally_centered_div_using_twitter_bootstrap

center a div horizontally with respect to its outer div using twitter bootstrap column class

Very often we need to center a div with respect to another div horizontally. When we are using twiiter bootstrap it is relatively easier process with the combination of column and offset class. The approach is like, suppose the outer div takes 12 columns that means the class of outer div is col-lg-12 [we are considering for the large screen. Process is similar for other screen sizes like md , sm or xs]. So the outer div is taking 12 columns, and suppose the inner div [which needs to be horizontally centered with respect to the outer div] takes 8 columns that means the class of inner div will be col-lg-8. Now in order to make this inner div horizontally centered we will put offset class on it. That means we will move the inner div by "x" columns.

Here x =( number of columns outer div taken - number of columns inner div taken )/2
so x = (12-8)/2 = 2

So we will add col-lg-offset-2 for inner div

So the final HTML code will be like this
 ```
 <div id="outer" class="col-lg-12 col-md-12">
   <div id="inner" class="col-lg-8 col-md-8 col-lg-offset-2 col-md-offset-2">

  </div>
 </div>
 ```
 

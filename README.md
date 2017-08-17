# udemy


Udemy Bootcamp:

1. use image address for img tab no third party needed
2. <b>use command and click</b> for simultanious edit code at different code (pikeman.html)
3. command d for duplicate
4. tag name and tab 
5. Id : unique should be used only once 
6. Class: same named class  can be used several times  

7. CSS Selectors:
￼
￼<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497339031/Screen_Shot_2017-06-12_at_11.46.21_PM_ry8tqt.png">
<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497339031/Screen_Shot_2017-06-12_at_11.46.21_PM_ry8tqt.png">
<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497339030/Screen_Shot_2017-06-12_at_11.46.04_PM_kh5ias.png">
<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497339035/Screen_Shot_2017-06-12_at_11.45.25_PM_vispfg.png">
￼
￼
8. Specific and cascade

priority ascending order:
-> body
-> ul
-> li
->class
->id  (higher priority)
￼
<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497339344/Screen_Shot_2017-06-13_at_12.16.38_AM_uj8wew.png">

Order of the Specificity

<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497340219/Screen_Shot_2017-06-13_at_12.49.51_AM_tw3a5h.png">

9) Revising Specific tags styles

<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497344210/Screen_Shot_2017-06-13_at_1.56.26_AM_wwvqiv.png">

10) <b>Text And Font:</b>
<a href="http://www.cssfontstack.com/">cssfontstack</a>

10.1 )  Font's
<a href="https://fonts.google.com/">Google fonts and repected libraries</a>

  10.2) Box Model
  <img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497389606/Screen_Shot_2017-06-13_at_2.32.51_PM_wck1dl.png">

  10.3) Padding, Margin
  <img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1497389941/Screen_Shot_2017-06-13_at_2.38.41_PM_jclvkn.png">
  

11)<b> What's the best practice for putting multiple projects in a git repository?</b>

A single repository can contain multiple independent branches, called orphan branches. Orphan branches are completely separate from each other; they do not share histories.

git checkout --orphan BRANCHNAME
This creates a new branch, unrelated to your current branch. Each project should be in its own orphaned branch.

Now for whatever reason, git needs a bit of cleanup after an orphan checkout.
~~~
rm .git/index

rm -r *
~~~
Make sure everything is committed before deleting

Once the orphan branch is clean, you can use it normally.

Solution 2

Avoid all the hassle of orphan branches. Create two independent repositories, and push them to the same remote. Just use different branch names for each repo.

# repo 1
git push origin master:master-1

# repo 2
git push origin master:master-2

12) <b>Autocomplete does not work in HTML and CSS files</b>

-> html tab (autocompletion not working) 
i.e 
~~~
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>

</body>
</html>

Solution:   Preferences > Settings -- User file:

"auto_complete_selector": "source, text",

~~~

13) I)colors ,transparent ,hexcode,RGB red green blue

<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1502871323/Screen_Shot_2017-08-16_at_1_11_48_AM_k9mfmt.webp">
<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1502871319/Screen_Shot_2017-08-16_at_1_11_29_AM_ifptdj.webp">
<img src="http://res.cloudinary.com/duqwfkttw/image/upload/v1502871314/Screen_Shot_2017-08-16_at_1_11_01_AM_fjqtfc.webp">

II) border

~~~
border: 8px solid red;

~~~

13.1) 

~~~
h1:hover{
color:blue;
}

h1:visited{
color:grey
}

#special:first-letter{
color:green;
font-size:20px;
}

~~~


~~~

// font weight 

p{
font-weight:bold;
}

//line height 

p{
line-height:2em;
}

//text -decoration

h1{
text-decoration:underline;
}
~~~

~~~

p{
margin: top right bottom left; // clock wise 
marign : 20px 2px 3px 4px ;
same as -
margin : 20px auto 20px auto;  ===   margin : 20px auto;

~~~

13.2) How to change the Photos in web site to color black and white whithout doing manually?

# .css 

~~~
 img{
filter: grayscale(100%);
}
~~~

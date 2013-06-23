# BlankPlate: A HTML, Sass (scss) Boilerplate

## What is this?
It's a bare bones boilerplate/SCSS framework I'll start off most web projects with.

It includes a CSS reset and a bunch of minimal boilerplate styles that should come in useful for any project.

It is not as in depth as something like <a href="http://html5boilerplate.com/">HTML5 Boilerplate</a> and doesn't include styled components like <a href="http://twitter.github.io/bootstrap/">Bootstrap</a>.

It can be used for a static web project as is, or you can copy the CSS folder into an existing framework.

## Features
* Uses SASS partials to help structure the CSS.
* Uses Compass to take advantage of CSS3 mixins so you don't have to worry about browser prefixes (-webkit- etc.).
* Uses Normalize to reset browser styles.
* Only enough CSS to get you started; no visual styling with this boilerplate.
* Only the HTML/JS you need to get started; very little components with this boilerplate.

## How to Use
This will vary depending on the framework you are using. The following is how to for a basic static website.

### Install Ruby
BlankPlate uses SASS and Compass, which rely on Ruby.

Macs come pre-installed with Ruby but if you need to you can <a href="http://www.ruby-lang.org/en/downloads/">download ruby here</a>.

### Install the compass gem
Open up terminal (or command line) and install compass .
```
$ gem update --system 
$ gem install compass
```

### Download BlankPlate
Download and copy the motherplate files into your new project folder.

### Run compass watch
In terminal go to your project folder and run compass.
```
$ cd sites/mynewproject/
$ compass watch
```

### Only edit the SCSS files
When you make changes to any of the scss files, your main.css file will be automatically updated.
You don't edit main.css directly, compass takes care of that for you.

If you were working on a Rails project for example, you could just copy the files in the css folder to app/assets/stylesheets (and use the compass-rails gem).

## HTML
A bare bones index.html template.

## CSS
* **_variable.scss** Put all your variables in here e.g. colors, padding, border radius - this helps with consistency across your project.
* **_forms.scss** Some basic form styles.
* **_layout.scss** This is where your main styles go. I typically have header, footer, nav, logo classes here.
* **_links-buttons.scss** Styles for any text links and/or buttons.
* **_mixins.scss** Reusabled SASS mixins e.g. clearfix.
* **_helper-classes.scss** Small reusable other styles that don't fit the rest of the framework.
* **_print.scss** Basic print stylesheets to make your pages look better when printed.
* **_reset.scss** This is normalize.
* **_shame.scss** Keep this to hand for any quick and dirty CSS you need to add but plan to tidy later.
* **_tables.scss** Styles for tables.
* **_type.scss** Basic styling for your typography.
* **main.scss** This brings all the partials together. Compass only compiles files that don't have an underscore. Don't write any css in this file. It's just to combine.
* **/assets** Any images that the CSS references e.g. an image sprite, goes in here.
* **/assets/fonts** For any fonts you reference in CSS including icon fonts or @font-face.

As your project grows and you need to add more styles just create new .scss files and reference them anywhere in your main.scss file.

Typical files I'll end up adding include _nav.scss, _notifications.scss, _home.scss.

## JavaScript ##
* I've included some basic Javascript including the latest jQuery and the document ready function.

## Images ##
* There is a /img folder for images.
* For images referenced in the CSS I tend to keep them in the css/assets/ folder e.g. sp.png is a sprite I can reference.
* Images referenced in the HTML are stored in the /img folder.

## Documentation ##
* <a href="https://github.com/leemunroe/motherplate">Motherplate</a>
* <a href="http://compass-style.org/">Compass Framework</a>
* <a href="http://sass-lang.com/">SASS</a>
* <a href="http://necolas.github.com/normalize.css/">normalize.css</a>
* <a href="http://csswizardry.com/2013/04/shame-css/">Shame css</a>





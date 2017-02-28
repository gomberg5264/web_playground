# Web Playground

Harrys web playground, demonstrating variety of website development techniques using best practices and standards.

Built for the University of Bristol unit [Web Technologies](https://www.cs.bris.ac.uk/Teaching/Resources/COMSM0104/cw/assign5/).

![Screenshot](screenshot.png "Screenshot")

# TODO
- Test performance by using the chrome extension of lighthouse:
		https://developers.google.com/web/tools/lighthouse/
- Automatically test performance using grunt performance testing tools, available here: https://github.com/blackrabbit99/browser-performance-testing-tools
- Comment all
- Use PhantomJs to automate things you do in the website
- Research this: https://github.com/sahat/hackathon-starter#recommended-design-resources
- Go through security here http://expressjs.com/en/advanced/best-practice-security.html
- Add async to js files?
- Check what happens if js is disabled on site
- Check what happens when the internet is disabled on site (font awesome icons dont load in header for a start)
- Host on Heroku instance

## Dependancies

- Clone project `git clone git@github.com:harrymt/web_playground.git`
- Ensure Ruby, Sass the Ruby gem and Grunt is installed
	- `gem update --system && gem install scss_lint`
- Ensure [sqlite3](https://www.sqlite.org/download.html) is setup and added to your PATH
- `npm install`

## Run Project

- `node server`
- View at `localhost:3001`


## Build Project

- Run `grunt` to build the files


## Test Project

- `grunt tests`


# General / Report

- Online LATEX parsers to make report!!
- Follow these security points: http://expressjs.com/en/advanced/best-practice-security.html

Why boilerplates?

NodeBootstrap - unobtrusive skeleton project for Node/Express.js with pre-configured best-practices. Kick-start your Node project development with tons of boilerplate taken care of, such as: clustering, Docker-support, error-handling, modularity, logging, views, environments etc. http://www.nodebootstrap.io
make a note, that all boilerplates are poo?
(Why use a boilerplate? http://whatis.techtarget.com/definition/boilerplate)

Boilerplates to consider:
https://www.npmjs.com/package/node-boilerplate (Doesn't use docker, or express, pro docker bit)
https://github.com/inadarei/nodebootstrap (TOO BLOATED)
http://www.clementinejs.com/tutorials/tutorial-beginner.html (More lighter weight! Dont use though)
Use basic Express application generator: https://expressjs.com/en/starter/generator.html



# HTML

- Practices, JS at the end of document
- CSS at top via a CDN probs
- Use &#960 rather than hex characters
- Use 1.0XML
- Handles content negotiation using (Polyglot HTML)[https://www.w3.org/TR/2011/WD-html-polyglot-20110405/#dfn-polyglot-markup]
https://www.w3.org/TR/xhtml-media-types/#media-types
- Uses [PUG](https://pugjs.org)

## Validators

- Uses a PUG validator

https://github.com/mozilla/html5-lint ?
https://www.npmjs.com/package/html-validator ?


# CSS


- Dont use lots of whitespace, add more columns
- Uses a CSS framework I designed
- Uses [SCSS](http://sass-lang.com/)
	- Styleguide of: https://github.com/airbnb/css
	- Uses scss-lint here https://www.npmjs.com/package/grunt-scss-lint


# JS
- Uses [Mocha](https://github.com/mochajs/mocha) for unit tests
- Experiment with showing off popular algorithms! As part of software job practice! Visulise them!
- QUnit for tests, JSlint for linting
- StyleGuide https://google.github.io/styleguide/jsguide.html

### Best Practices

- Douglas Crockford JS best practices
	- Use Strict mode
	- Make field and methods private
	- Avoid using this keywrod
	- Use Power consutrctors to avoid the new keyword
	- Inheritence is different
	- New ES6 features (not neccessarily well supported cross brower )


# PNG

# SVG

- Look at inkscape, different technologies!!!
- Generate circles in SVG http://www.lugolabs.com/circles

Animate a person icon using svg.

```scss

.svg-icon {
  height: 100px;
  overflow: visible;
  width: 100px;
}

.svg-icon path {
  animation: animatePath 5s 1s forwards infinite;
  fill: none;
  stroke: rgba(255, 255, 255, .9);
  stroke-width: 0.45;
}

```

# Server

https://github.com/sahat/hackathon-starter#recommended-nodejs-libraries


# Database

Why not Mongo DB
http://www.sarahmei.com/blog/2013/11/11/why-you-should-never-use-mongodb/

http://cryto.net/~joepie91/blog/2015/07/19/why-you-should-never-ever-ever-use-mongodb/

- SQLite


# Dynamic Pages

- Pug


# General Testing
- Performance, use Lighthouse extension
	https://developers.google.com/web/tools/lighthouse/
- Use PhantomJs to automate things you do in the website



# Topic
- Web playground!
- Build an interesting site structure, and adding a server to deliver pages and handle a database.
- e.g. shopping for sports gear, reviewing cameras, discussing politics, supporting a particular charity or organisation, teaching astronomy, uploading and showing off photos, social media, playing games.
- Need to demonstrate my grasp of wide varieyu of different technologies.
- It doesn't necessarily matter if your site doesn't make complete coherent sense in the end.


# Requirements
- Use standard HTML, CSS, JavaScript, PNG, SVG and other integrated client-side technologies, following the advice from the lectures.
- Node-based server
- DB embedded, preferably SQLite
- Design can be desktop-first or mobile-first, and you can use client-side or server-side techniques for creating dynamic pages.
- You can write everything yourself, or use any existing JavaScript-based frameworks or libraries or modules or scripts that you like.
- You should use open source tools as much as possible.

# Resources
- When reusing stuff.
- Check any restrictions (b) acknowledge them in your report (c) adapt them to follow the standards and advice in the lectures where necessary and (d) explain your added value (e.g. "I just copied it and learnt how to use it" or "I changed it a little" or "I understood it fully and re-wrote it").


# Marks

- X for HTML (out of 10)
- X for CSS (out of 10)
- X for JS (out of 10)
- X for PNG (out of 10)
- X for SVG (out of 10)
- X for Server (out of 10)
- X for Database (out of 10)
- X for Dynamic pages (out of 10)
- X for Depth (out of 40)
Total: out of 120

Key:
X means you have done nothing in this area
D means you started but got stuck or ran out of time
C means you have done basic work
B means you have done some solid work
A means you have done sophisticated or extensive work
? means you don't want to estimate


## Mark breakdown

- HTML:
	- Used XHTML delivery, or a validator, to make sure your pages are correct
	- Investigated a variety of different issues and gained a general high level of confidence with the structure of HTML pages (or with generating HTML via a framework)
- CSS:
	- No inline styles
	- Investigated a variety of different issues and gained a general high level of confidence with CSS style (or with generating CSS via a framework)
- JS:
	- Client-side JS for effects or animation or interaction, including use of client-side frameworks, but excluding aspects which are to do with dynamic page construction
	- Written a substantial script yourself, or written a number of script functions with different issues involved, or gained a medium amount of experience with client-side frameworks
	- Gained a high level of understanding of how client-side JavaScript works, or a high level of expertise in using client-side frameworks
- PNG:
	- Working with bitmap graphics in Gimp or Krita
	- Show how to convert images to PNG, cropping away unwanted edges, changing resoluation
	- Use basic tools such as using filters or changing colours or combining existing images or creating simple shapes or filling
	- Gained experience with some more sophisticated tools such as handling layers and transparency, or airbrushing or creating original artwork
- SVG:
	- this is working with vector graphics in Inkscape
	- Created a basic drawing in Inkscape, probably by copying something else
	- Gained experience with some of Inkscape's features such as shape tools, freehand drawing, simplification
	- Gained a higher level of experience, e.g. with path editing, grouping, transformations, gradients, patterns, etc., or put a lot of effort into vector artwork
- Server:
	- this is creating or adapting a server, either programming it yourself or using express and its add-ons
	- means you've created a server by minimally adapting the one provided, or closely following a tutorial to set up express
	- B means you've dealt with things like port numbers, URL validation, content negotiation for old browsers, sending redirections to browsers, handling UTF-8
	- A means you've dealt with things like https and certificates, or web sockets, or cloud hosting, or security issues beyond URL validation, or auto-testing, or cookies, or running under reduced privilege
- Database:
	- C means you've manually created a database, and then extracted data from it in your server
	- B means you've managed to update or insert data as well as extract it, and you've got the hang of callbacks for getting things to happen in the right order
	- A means you've gained a lot of experience with SQL, or you've put a lot of effort into organising database access (e.g. into a separate server-side module) or you've put a lot of effort into database design or details of handling your data
- Dynamic pages:
	- this is either inserting data into templates on the server side and delivering dynamic pages or requesting data from the server and inserting into existing pages on the client side
	- C means you've created a simple dynamic delivery system or you have used a framework in a simple way
	- B means you've organised dynamic delivery in a more sophisticated way, either doing more of your own programming or using more features of a framework
	- A means you've put in a lot of programming effort or become very fluent in using your chosen framework

## Additional work

Can subsitute one part for another (or just do more on one)

- animation done using CSS can count a little towards the JS heading
- using canvas, including its vector features, can take the place of conventional SVG work
- something clever with web sockets for a chat or game application might take the place of conventional dynamic page delivery

Understanding something properly!
If you have used a framework, making it do what you want counts for more than just producing a site that looks like most of the other sites that use that framework.


## How marking will work

- install node modules needed (otherwise server should be ready
- ZIP file should contain everything, e.g. downloaded images, dont include node_modules or git repo

- Submit report as a webpage or PDF? Use online Latex report???? Add option to download PDF online, e.g. d.o.server.com/playground/report!

- No marks for report.
- In PNG heading, describe how you created it!! (maybe make it online in a section?)

- Report should give estimated grades under each heading and list things ive done + JUSTIFY ESTIMATE

- Write something longer to explain overall aim and design
- Highlight things that I am proud of
- Anything that took a long time, but didn't make it into the site


## Technologies Used

- [Markdown to PDF](https://www.npmjs.com/package/markdown-pdf)
- [sqlite3](https://www.sqlite.org/download.html)
- [Mocha](https://github.com/mochajs/mocha)
- [SCSS](http://sass-lang.com/)
- [PUG](https://pugjs.org)

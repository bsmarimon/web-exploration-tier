## Week 2

#### Logistics
RGB, a design event hosting by the club, is coming up. Here's a sneak peak of the website by Julia Sun, <http://juliasun.io>.

<http://rgb.innovativedesign.club>

#### Review of Git
Git is a version control system designed to help organize small and large projects. Now, to review what we went over last week. First, Github is a web-based Git repository hosting service. You can use it to collaborate on projects with partners, or to hold code for personal projects (there are a lot of uses). The code you have in a repository your machine is your local copy. The same repository on Github is the remote copy. When you create a Git repo using `git init` (see below), the repository is not initialized with any remotes, and you must add them manually. If you clone a repository, the link you clone from is added as a remote with the name origin automatically, since by cloning, you tell Git where the repository remote is located! Below is a list of popular Git commands.

`git init` - creates a new Github repository in the directory where the command is run <br>
`git remote add _remoteName _remoteLink` - adds a new remote with the name provided as an argument, which points to the link provided (a link to a Github repository) <br>
`git remote rm _remoteName` - removes the remote with the name provided as an argument <br>
`git clone _githubLink` - creates a copy of the repository located at the Github link provided as an argument in the directory where the command is run <br>
`git status` - print the status of your current project <br>
`git add --all` or `git add .` - stages all files that have been changed (since the last commit) for commit <br>
`git commit -m "your message"` - commits files that have been staged for commit with a message <br>
`git push origin master` - pushes your changes to the <br>

#### Let's host a website
Last week, everyone made a Github account. In addition to managing Git repositories, Github also offers free hosting for static web pages, which is why you see so many websites with the partial domain \*.github.io. There's a nice and simple tutorial on how to do this here <https://pages.github.com/>. Let's walk through it!

Not every website you see has a \*.github.io domain, so how are they hosted? Another popular choice is Heroku, which provides free hosting for more complicated web applications than Github. These web applications are typically built on an existing Framework, such as Ruby on Rails, and have the domain \*.herokuapp.com. So how do we end up with creative URLs, such as innovativedesign.club? Developers can purchase a custom domain name, and then set this domain to point to the, for lack of a better term, uglier one. Now, whenever a user loads innovativedesign.club, it displays the web application hosted on Heroku for instance, but uses this special domain name instead!

The last concept we'll touch on here isn't related to front end web design, but to web security design. Why does Github configure domain names to be https://username.github.io instead of, for instance, https://github.io/username? Part of the answer is a web security concept called Same Origin Policy, implemented in modern browsers. Every website has an origin, which is collectively defined by it's protocol (http, https), it's domain name (username.github.io), and it's port number (2222), but we won't worry about the last one for now. For example, the origin for https://www.innovativedesign.club/decal/lesson/1 is https://www.innovativedesign.club. The Same Origin Policy states that a web browser should not permit scripts on one site to interact with another site if both web pages do not have the same origin - web pages can only "know" about other web pages with the same origin. Coming back to Github, their design choice means that every user website is protected from other user sites, since each has a separate origin due to the username domain name.

#### HTML (the first triforce piece heh)
We touched a little on HTML when hosting a website through Github, but now we're going to learn even more about it! HTML stands for HyperText Markdown Language. The idea is that a developer writes plain text, then marks it down with a specific language, changing how it appears. To start, let's talk about tags, or this language we'll use to change how plain text appears. Common tags are the paragraph tag, `<p>`, the link tag, `<a>`, and the bold tag `<b>`. Every tag in HTML starts with the letter, or word, specifying the tag, surrounded by <tag>. Every tag the ends with the same letter surrounded by </tag>. An example of a properly formatted tag is

`<p>Innovative Design Retreat is coming up soon, get excited!</p>`

Links work in a similar way, but now have some additional fields we need to specific, in particular, what the link will link us too!

`<a href="www.google.com">Click here to go to google!</a>`

If we want the link to open up a new tab, instead of changing the current page to the one specified in the link, we can also add target="\_blank". This can helpful in case that the user will still want to use the web page they're currently at, in addition to the one in the link.

`<a target="_blank" href="www.google.com">Click here to go to google!</a>`

During the meeting, we'll go over other HTML tags, including how to add images. For now, if you want a more in depth overview of HTML tags, check out <https://github.com/cle1994/InnoD_Web_Handbook/blob/master/3-html.md>.

#### CSS (the second piece!)
CSS stands for Cascading Style Sheets and, to put it simply, is used to make our web pages look pretty (aesthetically appealing?). The first step is figuring out how to get our HTML files and CSS files to talk to each other, since just because we place them in the same directory, doesn't mean that the browser will automatically link them together for us. This "linking" is done in the `<head></head>` section of an HTML file, with the `<link>` tag. For instance

`<link rel="stylesheet" type="text/css" href="main.css">`

Once we've linked our CSS, it can start talking to our HTML files. We'll go over ids, classes, and CSS syntax during the meeting. For a more in depth overview of CSS properties, again, I suggest you check out <https://github.com/cle1994/InnoD_Web_Handbook/blob/master/4-css.md>. There are also some links here to some really great sites, such as W3Schools.

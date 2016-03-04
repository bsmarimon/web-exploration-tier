## Week 3

#### Logistics
Retreat is this weekend ~ get excited! RGB, a design event hosting by the club, is coming up. Here's the finished website by Julia Sun, <http://juliasun.io>.

<http://rgb.innovativedesign.club>

Time for good news! Also, if you ever played Pokemon as a kid, check this out <http://www.pokegraphs.com/>. If you like windows, check out this too <http://www.windowsofnewyork.com/>.

#### Review of CSS
The properties we covered last week were
* background-color
* color
* font-family
* font-size

#### More HTML Tags!
We're going to add a couple more HTML elements to our toolbox today. To start, we're going to talk about forms. Forms are specified using the <form> tag. They can be used for a lot of different things, for instance, signing up a user for a site, saving your credit card information during a purchase, having you fill out a survey for a class online. Forms take user input through <input> tags, which can be labelled for a specific purpose, such as username, with the <label> tag. Input tags have different types. If you wanted to have the input be used for a user's name, you would set `<input type="text">`. Every form needs a submit button, which in this case, we'll also use an input tag, with the type submit, `<input type="submit">`.

#### The Box Model
We can place elements on a page, but how can we add spacing between them? Every element has it's own box model, which consists of content, padding, border, and margins. You can find a helpful visualization of this here <http://www.w3schools.com/css/css_boxmodel.asp>. We'll go through a couple exercises, but for now, the most important two concepts here are padding and margins.

#### Vertical Alignment
Vertical and horizontal alignment are important to know in general for web design. Let's start with vertical alignment, and the concept of parent and child elements.

```
.element {
  position: relative;
  top: 50%;
  transform: translateY(-50%);
}
```

#### Breaking Pages into Components
When thinking about the design of page, it can be helpful to examine the individual components on the page and consider what each accomplishes. To start, let's look at a very common component of most websites, the navigation bar. Let's walk through the tutorial on how to do a horizontal navigation bar.

#### A Monotonous Web
If we get here ~

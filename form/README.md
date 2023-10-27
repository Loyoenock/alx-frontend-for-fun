# Forms

__HTML | CSS | Front-end__

## Resources

__Read or watch:__

* [An Extensive Guide To Web Form Usability — Smashing Magazine](https://www.smashingmagazine.com/2011/11/extensive-guide-web-form-usability/)
* [Forms - UX Movement](https://uxmovement.com/category/forms/)
* [Placeholders in Form Fields are Harmful (Video)](https://www.nngroup.com/videos/placeholders-form-fields/)
* [The Anatomy of Accessible Forms: Best Practices | Deque](https://www.deque.com/blog/anatomy-of-accessible-forms-best-practices/)
* [Pure CSS Custom Error Messaging for Default Form Elements – Sarah Holley Design](https://sarahholleydesign.com/pure-css-custom-error-messaging-for-default-form-elements/)

__MDN resources:__

* [HTML forms - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/Forms)
* [form - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)
* [fieldset: The Field Set element - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/fieldset)
* [legend - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/legend)
* [label - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label)
* [input: The Input (Form Input) element - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input)
* [tabindex - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex)
* [accesskey - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/accesskey)
* [button: The Button element - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button)
* [select - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/select)
* [optgroup - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/optgroup)
* [datalist - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/datalist)
* [textarea - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/textarea)
* [Form Validation UX in HTML and CSS | CSS-Tricks](https://css-tricks.com/form-validation-ux-html-css/)
* [Constraint validation - Developer guides | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Constraint_validation)
* [:invalid - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/:invalid)
* [:valid - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/:valid)
* [:optional - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/:optional)


## Learning objectives

At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), without the help of Google:

* How to create an HTML5 form
* How to choose the right input type
* How to constrain a form field with regular expressions
* How to style inputs for invalid, valid, and required fields
* How to build a a comment form
* How to build a simple search form
* How to create usable and accessible forms

## Requirements

* Allowed editors: vi, vim, emacs
* A README.md at the root of the project directory is mandatory
* HTML and CSS have been rendered on Chrome 78 or more.

### Tasks

0. basic comment structure
* [html](./01-article.html)
* [css](./01-styles.css)

To ensure we start on the same foot, use these files:

00-article.html

In your 01-article.html file

* Sibling to the <div class="post">, create a new <section> with the class post-comments
* Inside the section create an header
*   In the <header> create a heading level 2 with class section-title and text: Leave a comment
*   under the level 2 heading create a paragraph with text: All fields are required.

* Create a form siblings to the header
*   Action: #
*   Method: post

In your 01-styles.css file

After the Tag list styles, create a new comment

```
/*** FORM ***/
/* Comment section
    ============================= */
```

* Target post-comments class
*   Property: width, Value: 80%
*   Property: margin, Value: 10rem 0 0 auto
*   Property: padding-left, Value: 7rem
* Target the section-title class inside the post-comments class 
*   Property: font-variant, Value: small-caps
* Add a new comment section


```
/* Basic form
    ============================= */
```

* Target all form
*   Property: display, Value: flex
*   Property: flex-direction, Value: column
*   Property: padding, Value: 1rem 0
*   Property: margin, Value: 0

__inal rendering__


__Repo:__

* GitHub repository: alx-frontend-for-fun
* Directory: form
* File: 01-article.html, 01-styles.css

1. more comment basic structure
* [html](./02-article.html)
* [css](./02-styles.css)

From 01-article.html, create 02-article.html

* In the form in the comment section
*   Create a first fieldset with a legend that has the text Your personal information and the class visually-hidden
*       In the fieldset create a first div with the classes form-group and col-1-2
*       Sibling to the first div, create a second div with the classes form-group and col-1-2
*       Sibling to the 2 divs create a third div with the classes form-group and col-2-3
*   Sibling to the first fieldset, create a second fieldset with a legend that has the text Your comment and the class visually-hidden
*       In the second fieldset create a first div with the classes form-group and col-2-3
*       Sibling to the first div create a second div with the classes form-group and col-2-3
*       Sibling to the 2 divs create a third div with the class form-group

From 01-styles.css, create 02-styles.css

* Target all fieldset and set the following rules
*   flex display
*   direction of flex is column
*   justify the content at flex-start
*   no border
*   0 0 2rem padding

__Final rendering (same as previously because <legend> tags are hidden by default)__

__Repo:__

* GitHub repository: alx-frontend-for-fun
* Directory: form
* File: 02-article.html, 02-styles.css


2. create labels and input container

* [css](./03-styles.css)
* [html](./ 03-article.html)

From 02-article.html, create 03-article.html and in the form which is in the comment section:

*   In the first fieldset
*   In the first div (which has classes form-group and col-1-2)
*       Create a label
*           For: your-first-name
*           Text: First Name
*       Sibling to the label, create a <div> with the class form-field
*           Create a span inside the div with the class form-field-container
*   In the second div (which has classes form-group and col-1-2)
*       Create a label
*           For: your-last-name
*           Text: Last Name
*       Sibling to the label, create a <div> with the class form-field
*           Create a span inside the div with the class form-field-container
*   In the third div (which has classes form-group and col-2-3)
*       Create a label
*           For: your-email
*           Text: Email
*       Sibling to the label, create a <div> with the class form-field
*           Create a span inside the div with the class form-field-container
* In the second fieldset
*   In the first div (which has classes form-group and col-2-3)
*       Create a label
*           For: your-title
*           Text: Title
*       Sibling to the label, create a <div> with the class form-field
*           Create a span inside the div with the class form-field-container
*   In the second div (which has classes form-group and col-2-3)
*       Create a label
*           For: your-comment
*           Text: Comment
*       Sibling to the label, create a <div> with the class form-field
*           Create a span inside the div with the class form-field-container
*   In the third div (which has class form-group)
*       Create a <button> with the classes button and button-primary
*           Text: Post my comment

__From 02-styles.css, create 03-styles.css:__

* Target all label
*   cursor should be pointer
*   display as block element
*   don’t wrap white space
*   size of font should be 1.4rem
*   set padding to 0 0 .5rem

Final rendering



__Final rendering with button in hover__



__Repo:__

* GitHub repository: alx-frontend-for-fun
* Directory: form
* File: 03-styles.css, 03-article.html

3. create the inputs

* [html](./04-article.html)
* [css](./04-styles.css)

From 03-article.html, create 04-article.html:

* In the first fieldset
*   In the first span of form-field-container class, create an input
*       Type: text
*       Name: your-first-name
*       Id: your-first-name
*       Placeholder: e.g. Mike
*       Pattern: [A-Za-zÀ-ž\s]{3,} (we want to allow all characters with and without accents and spaces. We want to have at least 3 characters to make the input valid)
*       Max length: 35
*       Autocomplete is on
*       Access Key: f
*       Required: true
*   In the second span of form-field-container class, create an input
*       Type: text
*       Name: your-last-name
*       Id: your-last-name
*       Placeholder: e.g. Smith
*       Pattern: [A-Za-zÀ-ž\s]{3,} (we want to allow all characters with and without accents and spaces. We want to have at least 3 characters to make the input valid)
*       Max length: 40
*       Autocomplete is on
*       Access Key: l
*       Required: true
*   In the third span of form-field-container class, create an input
*       Type: email
*       Name: your-email
*       Id: your-email
*       Placeholder: e.g. youremail@gmail.com
*       Pattern: [a-z0-9.\_%+-]+@[a-z0-9.-]+\\.[a-z]{2,}$ (we want to ensure the correct format of the email)
*       Max length: 55
*       Autocomplete is on
*       Access Key: e
*       Required: true
*   In the second fieldset
*       In the first span of form-field-container class, create an input
*       Type: text
*       Name: your-title
*       Id: your-title
*       Placeholder: e.g. I loved that article
*       Pattern: [A-Za-zÀ-ž\s]{4,} (we want to allow all characters with and without accents and spaces. We want to have at least 4 characters to make the input valid)
*       Max length: 75
*       Autocomplete is on
*       Access Key: t
*       Required: true
*   In the second span of form-field-container class, create a textarea
*   Name: your-comment
*   Id: your-comment
*   Placeholder: Write your comment here
*   Minimum length: 10
*   Access Key: c
*   Required: true
*   Columns: 30
*   Rows: 6

From 03-styles.css, create 04-styles.css, after the label selector:

* Target in one selector all input type text, all input type email, all textarea
*   Property: position, Value: relative
*   Property: width, Value: 100%
*   Property: padding, Value: 1.2rem
*   Property: line-height, Value: 1
*   Property: border, Value: .1rem solid point to the variable color-black
*   Property: background-color, Value: point to the variable color-white
*   Property: box-shadow, Value: none
*   Property: outline, Value: 0
*   Target in one selector all input type text, all input type email
*   Property: padding-right, Value: 3rem
* Target in one selector the focus state of all input type text, the focus state of all input type email, the focus state of all textarea
*   Property: border, Value: .1rem solid point to the variable color-grey
*   Property: background-color, Value: point to the color-light-grey
* Now target the placeholder, it can be tricky so I’m gone give you the code to add to your stylesheet:

```
::placeholder {
  font-style: italic;
  font-size: var(--font-size-small);
}
```
Final rendering

Final rendering when “Last name” field is focus

__Repo:__

* GitHub repository: alx-frontend-for-fun
* Directory: form
* File: 04-article.html, 04-styles.css


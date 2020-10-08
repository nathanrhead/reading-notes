# Code 201 | Forms & JS Events

## Class 09 Reading Notes

---

## Chapter 7: Forms (pp. 330 - 357), from _HTML & CSS_ by Jon Duckett

I. Introduction:
    
    A. "HTML borrows the concept of a form  to refer to different elements that allow you to collect information from visitors to your site."
    B. "The best known form on the web is probably the search box that sits right in the middle of Google's homepage."

II. Form Controls

    A. Types
        1. Adding text
            a. text input (single-line)
            b. Passwords: "Like a single line text box but it masks the characters entered."
            c. Text area (multi-line)
        2. Making choices
            a. Radio buttons: "For use when a user must select one of a number of options."
            b. Checkboxes
            c. Drop-down menus
        3. Submitting forms
            a. Submit buttons
            b. Image buttons: similar to submit buttons, but with an image of your choice.
            c. File upload

    B. How forms work
        1. "A user fills in a form and then presses a button to submit the information to the server."
        2. "The name of each form control is sent to the server along with the value the user enters or selects."
        3. "The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database."
        4. "The server creates a new page to send back to the browser based on the information received."

    C. Differentiated types of data
        1. "To differentiate between various pieces of inputted data, information is sent from the browser to the server using name/value pairs," e.g., username = Nathan.
        2. "If the form control allows the user to enter text, then the value of the form control is whatever the user has typed in. If the form control allows you to choose from a fixed set of answers (e.g. radio buttons, checkboxes or a drop down list), the web page author will add code that gives each option an automatic value."
        
III. Form structure

    A. <form>: "This element should always carry the action attribute and will usually have a method and id attribute too."
        1. action attribute: "Its value is the URL for the page on the server that will receive the information in the form when it is submitted."
        2. method attribute: "Forms can be sent using one of two methods: get or post."
            a. get method (default): "the values from the form are added to the end of the URL specified in the action attribute. The get method is ideal for:"
                i. "short forms (such as search boxes)"
                ii. "when you are just retrieving data from the web server (not sending information that should be added to or deleted from a database)"
            b. post: "the values are sent in what are known as HTTP headers. As a rule of thumb you should use the post method if your form:"
                i. "allows users to upload a file";
                ii. "is very long";
                iii. "contains sensitive data (e.g. passwords)";
                iv. "adds information to, or deletes information from, a database."
        3. The id attribute: "the value is used to identify the form distinctly from other elements on the page (and is often used by scripts — such as those that check you have entered information into fields that require values)."
    
    B. <input>: "used to create several different form controls. The value of the type attribute determines what kind of input they will be creating."
        1. type="text": single-line text input form.
            a. name attribute: "[E]ach form control requires a name attribute. The value of this attribute identifies the form control and is sent along with the information they enter to the server."
            b. size attribute: "The size attribute should not be used on new forms. . . . In any new forms you write, CSS should be used to control the width of form elements."
            c. maxlength attribute: limits the number of characters that may be entered.
        2. type="password": like a single-line text input, except that the characters are masked. 
            a. name attribute: "indicates the name of the password input," e.g., password
            b. size, maxlength attributes may be used.
            c. Not to be used to send sensitive data to a server. "For full security, the server needs to be set up to communicate with users' browsers using Secure Sockets Layer (SSL)."
        3. <textarea>: form for multi-line text input.
            a. Needs an opening AND a closing tag.
            b. "Any text that appears between the opening <textarea> and closing </textarea> tags will appear in the text box when the page loads. . . . Some sites use JavaScript to clear this information when the user clicks in the text area.)" Otherwise, that text gets sent to the server, too.
            c. Use CSS to control the forms width and height. 
        4. type="radio"
            a. name attribute: "the value of the name attribute should be the same for all of the radio buttons used to answer that question."
            b. value attribute: "indicates the value that is sent to the server for the selected option."
            c. checked attribute: "used to indicate which value (if any) should be selected when the page loads."
            d. "If you are only allowing the user one option and want them to be able to deselect it (for example if they are indicating they agree to terms and conditions), you should use a checkbox instead."
        5. type="checkbox"
            a. name attribute: "sent to the server with the value of the option(s) the user selects." Should be the same for all of the boxes that address the same question.
            b. value attribute: the answer checked by the user.
            c. checked attribute: can be used to check a box when the page loads.
        6. type="file"
            a. "This type of input creates a box that looks like a text input followed by a browse button. When the user clicks on the browse button, a window opens up that allows them to select a file from their computer to be uploaded to the website."
            b. "When you are allowing users to upload files, the method attribute on the <form> element must have a value of post. (You cannot send files using the HTTP get method.)"
            c. You can't control the appearance of the browse window. 
        7. type="submit": used to send a form to a server.
            a. name: not required.
            b. value: "The value attribute is used to control the text that appears on a button. It is a good idea to specify the words you want to appear on a button because the default value of buttons on some browsers is ‘Submit query’ and this might not be appropriate for all kinds of form."
            c. "If you want to control the appearance of a submit button, you can either use CSS (as you will learn on page 343), or you can use an image for the button."
        8. type="image": "If you want to use an image for the submit button, you can give the type attribute a value of image. The src, width, height, and alt attributes work just like they do when used with the <img> element."
        9. type="hidden": "These form controls are not shown on the page (although you can see them if you use the View Source option in the browser). They allow web page authors to add values to forms that users cannot see. For example, a web page author might use a hidden field to indicate which page the user was on when they submitted a form."
        10. type="date": "This will create a date input in browsers that support the new HMTL5 input types." The appearance of the date depends on the browser. 
        11. type="email": "Browsers that support HTML5 validation will check that the user has provided information in the correct format of an email address. Some smart phones also optimize their keyboard to display the keys you are most likely to need when entering an email address (such as the @ symbol)."
        12. type="url"
        13. type="search"
        14. placeholder attribute: "On any text input, you can also use an attribute called placeholder whose value is text that will be shown in the text box until the user clicks in that area. Older browsers simply ignore this attribute."

    C. <select>: drop-down menu
        1. "[C]ontains two or more <option> elements." 
        2. name attribute: " indicates the name of the form control being sent to the server, along with the value the user selected."
        3. <option>: "used to specify the options that the user can select from," assigned the title indicated between the opening and closing tags.
            a. value attribute: "indicate the value that is sent to the server along with the name of the control if this option is selected."
            b. selected attribute: "used to indicate the option that should be selected when the page loads. . . . If this attribute is not used, the first option will be shown when the page loads. If the user does not select an option, then the first item will be sent to the server as the value for this control."
        4. size attribute: "You can turn a drop down select box into a box that shows more than one option by adding the size attribute. Its value should be the number of options you want to show at once." According to this book, it's buggy on Firefox and Safari. 
        5. multiple attribute: 
            a. "You can allow users to select multiple options from this list by adding the multiple attribute with a value of multiple."
            b. "It is a good idea to tell users if they can select more than one option at a time. It is also helpful to indicate that on a PC they should hold down the control key while selecting multiple options and on a Mac they should use the command key while selecting options."

    D. <button>: "introduced to allow users more control over how their buttons appear, and to allow other elements to appear inside the button. This means that you can combine text and images between the opening <button> tag and closing </button> tag."

    E. <lable>: "[E]ach form control should have its own <label> element as this makes the form accessible to vision-impaired users."
        1. "The <label> element can be used in two ways. It can:"
            a. "Wrap around both the text description and the form input";
            b. "Be kept separate from the form control and use the for attribute to indicate which form control it is a label for."
        2. for attribute: "tates which form control the label belongs to."
        3. "The value of the for attribute matches that of the id attribute on the form control it is labelling. This technique using the for and id attributes can be used on any form control. When a <label> element is used with a checkbox or radio button, users can click on either the form control or the label to select. The expanded clickable area makes the form easier to use."
        4. Best way to place labels on form controls:
            a. Above or to the left of:
                i. text inputs
                ii. text areas
                iii. select boxes
                iv. file uploads
            b. To the right of:
                i. each checkbox
                ii. each radio button
                
    F. <fieldset>: used to group related controls together, especially when forms are long. "Most browsers will show the fieldset with a line around the edge to show how they are related. The appearance of these lines can be adjusted using CSS."

    G. <legend>: "The <legend> element can come directly after the opening <fieldset> tag and contains a caption which helps identify the purpose of that group of form controls."

IV. Form Validation: the message you get when you don't complete a form field correctly.
    A. Done in HTML5 or in JS.
    B. "Validation helps ensure the user enters information in a form that the server will be able to understand when the form is submitted."

## Chapter 14: Lists, Tables & Forms (pp. 330 - 357), from _HTML & CSS_ by Jon Duckett

## Chapter 6: Events (pp. 243 - 292), from _JavaScript & jQuery_ by Jon Duckett

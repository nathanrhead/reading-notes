# Notes on CSS

## from _HTML & CSS_ by Jon Duckkett

I. Chapter 10: Introducing CSS

    A. What CSS Does: "CSS allows you to create rules that specify how the content of an element should appear."

    B. How CSS Works

        i. "The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element."
        ii. "CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented."

    C. Rules, Properties, and Values

        i. "A CSS rule contains two parts: a selector and a declaration."
        ii. Ex: p is the selector and font-family: Arial is the declaration.
        iii. "CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon."

    D. Linking CSS to HTML

        i. Internally: style tag nested in the head tag: outdated method. 
        ii. Externally: link tag nested in the head and utilizing the href, type, and rel attributes. 
            a. href: "This specifies the path to the CSS file (which is often placed in a folder called css or styles)."
            b. type: "This attribute specifies the type of document being linked to. The value should be text/css."
            c. "rel: This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file."
        iii. Example
        ---
        <link href="css/styles.css" type="text/css" rel="stylesheet" />
        ---
        iv. Benefits of external over internal linking
            a. "Allows all pages to use the same style rules (rather than repeating them in each page)."
            b. "Keeps the content separate from how the page looks."
            c. "Means you can change the styles used across all pages by altering just one file (rather than each individual page)."
        
    E. CSS Selectors
        i. Case sensitive.
        ii. General types of selectors

    ![General CSS Selectors](Images/General CSS Selectors.jpeg)

    F. "How CSS Rules Cascade"
        
        i. Last Rule: "If the two selectors are identical, the latter of the two will take precedence."
        ii. Specificity: "If one selector is more specific than the others, the more specific rule will take precedence."
        iii. Important: "You can add !important after any property value to indicate that it should be considered more important than other rules that apply to the same element."
        iv. Inheritance: Font-family and color elelments will apply to child elements, while elements like background-color or borders are not inherited. 
        iv. "You can force a lot of properties to inherit values from their parent elements by using inherit for the value of the properties."

II. Chapter 11: Color

    A. How to Specify Colors
        
        i. Foreground Colors
            a. RGB Values: "These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)."
            b. Hex Codes: "These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80."
            c. Color Names: "There are 147 predefined color names that are recognized by browsers. For example: DarkCyan."
        
        ii. Background Colors
            a. "CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box."
            b. "You can specify your choice of background color in the same three ways you can specify foreground colors."
            c. "If you do not specify a background color, then the background is transparent."

    B. Color Terminology and Contrast
        i. "Every color on a computer screen is created by mixing amounts of red, green, and blue."
        ii. Definitions
            a. Hue: "Hue is near to the colloquial idea of color. Technically speaking, however, a color can also have saturation and brightness as well as hue."
            B. Saturation: "Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray."
            C. Brightness: "Brightness (or "value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the color would be very dark."
        iii. Contrast
            a. "When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible."
            b. "Text is harder to read when there is low contrast between background and foreground colors."
            c. "Text is easier to read when there is higher contrast between background and foreground colors."
            d. "For long spans of text, reducing the contrast a little bit improves readability."
        iv. Opacity: RGB_a_
            a. "CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity)."
            b. "Because some browsers will not recognize RGBA colors, you can offer a fallback so that they display a solid color. If there are two rules that apply to the same element, the latter of the two will take priority. To create the fallback, you can specify a color as a hex code, color name or RGB value, followed by the rule that specifies an RGBA value. If the browser understands RGBA colors it will use that rule. If it doesn't, it will use the RGB value."
    C. HSL Colors: "CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values."
        i. Hue: "In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from 0 to 360."
        ii. Saturation: "Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray."
        iii. Lightness: "Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred to as luminosity."
    D. HSL and HSLA: the alpha represents transparency, with a value between 0 and 1. 

[<--Home-->](../README.md)

# information-foraging
/Tasks

Finding Content in HTML
    - <div id="visit-our-school"> ==$0

Changing Menu Names
    Inspect the menu item "Parent Resources" and take a look at it's ancestors.
        - <ts-load data-name="header"></ts-load>
    Change the menu item "Parent Resources" to "Recommended Reading". When you save the file, your local version should automatically refresh and you should be able to see your new text.
        - <a id="parent-resources" href="files/parent_resources.html">Recommended Reading</a>

Finding and Modifying CSS Properties
    Curently, there's an 80 pixel border around "Visit Our School", the "Our students..." sentence and the "Contact Us" button. Figure out how to change it to a 60 pixel border. Then, make it so that "Our students..." text has a larger inset from the border (i.e. make the text occupy a narrower space and the gray space to the left and right is larger). Note: To accomplish this, you will need to change one existing CSS property value and add at least one new one.
        #visit-our-school {
            text-align: center;
            background-color: #eee;
            padding: 60px;
            margin-bottom: 2em;
        }

        #visit-our-school p {
            text-align: left;
            margin-bottom: 2em;
            font-size: 1.25em;
            padding: 70px;
        }

        Modified padding for #visit-our-school
        Added padding to #visit-our-school p

Defining New CSS Properties
    An Example Style That Cascaded
        Task: Use the web developer tools to find the HTML element for "Classroom News" and look at it's styling.

        Question: Where is the CSS specification that defines which font is used (e.g. Arial, Times New Roman, etc)? Hint: if you've found the right thing, you should see that the font property is inherited.
            body main {
            color: #555;
            font-family: "Source Sans Pro", "Helvetica Neue", Helvetica, Arial, sans-serif;
            line-height: 1.45;
            }
    Making a New Style
        Task: Suppose you wanted to make the Classroom News header stand out more. Define a new style specification to make it's font size twice as big as the standard font size. This change should not effect the Announcements header next to it. Hint: You may need to assign a class to the relevant HTML and define a style for that class.

        Question: What does your CSS code look like?
            In common.css, added:
                #left-header{
                    font-size: 2em;
                }


JavaScript
    Task: Follow this tutorial on how to create a sticky tutorial and adapt it to work with the Nursery School site. Sticky Header Tutorial

    Question: What is the id for the html element associated with the header?
        <header role="banner" id="auto_gen_id_unq_21">

    Question: What is the css definition for sticky as defined for your header element?
        #auto_gen_id_unq_21{
            position: sticky;
            top: 0;
            padding: 20px 30px;
            background-color:#fff;
        }

        Sticky as defined by my header element is a header that stays in the top reference position once a user scrolls it to that point and keeps the header there throughout the scroll journey.
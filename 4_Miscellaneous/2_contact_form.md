```css
body {
    background-color: #EEEEEE;
    font-family: sans-serif;
}

#layout {
    width: 500px;
    margin: 0px auto;
}

header,
footer {
    text-align: center;
    padding: 50px;
}

header p {
    font-size: 14px;
}

form {
    background-color: white;
    padding: 36px;
    border: 2px solid #CCCCCC;
    border-radius: 2px;
}

form div label {
    display: block;
    margin-bottom: 8px;
    font-weight: bold;
}

input,
select,
textarea {
    padding: 12px;
    width: 100%;
    box-sizing: border-box;
    border: 1px solid #CCCCCC;
    margin-bottom: 16px;
}

textarea {
    font-family: sans-serif;
}

/*
    The special [] selector syntax allows us to target 
    different inputs based on their type attribute
*/
input[type=submit] {
    width: auto;
    background-color: #0e6de1;
    color: white;
    border: 0;
    border-radius: 3px;
    min-width: 75px;
}

/*
    This is an advanced selector that says that
    we will target a form input if it is in an
    invalid state, but only if it is not in focus
    and there is not a placeholder shown inside
    (in other words, only if the user has typed
    something and left the field)
*/
input:not(:focus):not(:placeholder-shown):invalid {
    background-color: lightcoral;
    border: 2px solid red;
}

```html
<!DOCTYPE html>
<html lang="en">
    <head> 
        <meta charset="UTF-8"> 
        <meta http-equiv="X-UA-Compatible" content="IE=edge"> 
        <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
        <title>Contact Form</title>
        <link href="css/style.css" rel="stylesheet">
    </head>
    <body>
        <div id="layout">
            <header>
                <h1>Contact Us</h1>
                <p>
                    Got a question? 
                    We'd love to hear from you. 
                    Send us a message and we'll
                    respond as soon as possible.
                </p>
            </header>
            <main>
                <!--
                    To make a form actually functional, you must do two things:
                        - set the method attribute to "POST"
                        - provide a valid URL to the action attribute,
                          which will handle the form submission
                          (a free option is to create an account on getform.io,
                          and use the endpoint URL that they provide you with)
                -->
                <form 
                    method="POST" 
                    action="https://getform.io/f/599c2b13-fd57-44e4-95a1-2c722b05c5e8"
                >
                    <div>
                        <label for="services_id">
                            What can we help you with?
                        </label>
                        <select id="services_id" name="service_selection">
                            <option 
                                id="default_option" 
                                value="none" 
                                disabled
                                selected
                            >
                                Select what we can help you with
                            </option>
                            <option value="gardening">
                                Gardening
                            </option>
                            <option value="coding">
                                Coding
                            </option>
                            <option value="web dev">
                                Web Development
                            </option>
                        </select>
                    </div>
                    <div>
                        <label for="name_id">Name</label>
                        <input 
                            type="text" 
                            id="name_id" 
                            name="name" 
                            required 
                            minlength="2"
                            placeholder="E.g. John Smith"
                        >
                    </div>
                    <div>
                        <label for="email_id">Email</label>
                        <input 
                            type="email" 
                            id="email_id" 
                            name="email"
                            required
                            placeholder="E.g. jane.doe@gmail.com"
                        >
                    </div>
                    <div>
                        <label for="message_id">Message</label>
                        <textarea 
                            id="message_id" 
                            name="message"
                            placeholder="I would like you to..."></textarea>
                    </div>
                    <div>
                        <input type="submit" value="Send">
                    </div>
                </form>
            </main>
            <footer>
                <h2>Oh, you want more?</h2>
                <p>
                    To make a form like this functional, try creating
                    an account at 
                    <a href="https://getform.io/" target="_blank">
                        getform.io 
                    </a>.
                </p>
                <p>
                    Then, copy the <b>Form Endpoint</b> URL they provide
                    you with, and set it as the <form>'s 
                    <i>action</i> attribute, as well as set the 
                    <i>method</i> attribute to "POST".
                </p>
                <p>
                    That should make your form functional, and you can
                    see the submitted forms in getform.io, or in the 
                    inbox you associated with your getform.io account!
                </p>
            </footer>
        </div>
    </body>
</html>
```

---
title: "Inputs"
description: Input components are used for forms.
date: 
draft: false
layout: list
menu:
  main:
    parent: Components
    weight: 6
sections: 
    - name: Form Inputs
      subsections: 
        # CHECKBOX
        - id: checkbox
          name: Checkbox
          description: Checkboxes are important for various reasons.
          example:
            code: >-
                &lt;form&gt;
                    &lt;input type="checkbox" id="vehicle1" name="vehicle1" value="Bike"&gt;
                    &lt;label for="vehicle1"&gt; I have a bike&lt;/label&gt;&lt;br&gt;
                    &lt;input type="checkbox" id="vehicle2" name="vehicle2" value="Car"&gt;
                    &lt;label for="vehicle2"&gt; I have a car&lt;/label&gt;&lt;br&gt;
                    &lt;input type="checkbox" id="vehicle3" name="vehicle3" value="Boat"&gt;
                    &lt;label for="vehicle3"&gt; I have a boat&lt;/label&gt;&lt;br&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
                    <label for="vehicle1"> I have a bike</label><br>
                    <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
                    <label for="vehicle2"> I have a car</label><br>
                    <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
                    <label for="vehicle3"> I have a boat</label><br>
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:
            - name: for
              value: element_id
              description: Specifies the id of the form element the label should be bound to
            - name: form
              value: form_id
              description: Specifies which form the label belongs to
        # RADIO
        - id: radio
          name: Radio Buttons
          description: Radio buttons are used to select multiple values in a form.
          example:
            code: >-
                &lt;form&gt;
                    &lt;input type="radio" id="male" name="gender" value="male"&gt;
                    &lt;label for="male"&gt;Male&lt;/label&gt;&lt;br&gt;
                    &lt;input type="radio" id="female" name="gender" value="female"&gt;
                    &lt;label for="female"&gt;Female&lt;/label&gt;&lt;br&gt;
                    &lt;input type="radio" id="other" name="gender" value="other"&gt;
                    &lt;label for="other"&gt;Other&lt;/label&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <input type="radio" id="male" name="gender" value="male">
                    <label for="male">Male</label><br>
                    <input type="radio" id="female" name="gender" value="female">
                    <label for="female">Female</label><br>
                    <input type="radio" id="other" name="gender" value="other">
                    <label for="other">Other</label>
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:
            - name: for
              value: element_id
              description: Specifies the id of the form element the label should be bound to
            - name: form
              value: form_id
              description: Specifies which form the label belongs to
        # SELECT BOX
        - id: select
          name: Select Box
          description: Select boxes are form elements that allow you to choose from a list of options.
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="cars"&gt;Choose a car:&lt;/label&gt;
                    &lt;select id="cars"&gt;
                        &lt;option value="volvo"&gt;Volvo&lt;/option&gt;
                        &lt;option value="saab"&gt;Saab&lt;/option&gt;
                        &lt;option value="opel"&gt;Opel&lt;/option&gt;
                        &lt;option value="audi"&gt;Audi&lt;/option&gt;
                    &lt;/select&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="cars">Choose a car:</label>
                    <select id="cars">
                        <option value="volvo">Volvo</option>
                        <option value="saab">Saab</option>
                        <option value="opel">Opel</option>
                        <option value="audi">Audi</option>
                    </select>
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes: 
        # RANGE
        - id: range
          name: Range Selector
          description: The range input selector allows you to input a number within a specific programable range.
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="points"&gt;Points (between 0 and 10):&lt;/label&gt;
                    &lt;input type="range" id="points" name="points" min="0" max="10"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="points">Points (between 0 and 10):</label>
                    <input type="range" id="points" name="points" min="0" max="10">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes: 
        #TEXT 
        - id: text
          name: Text Input
          description: Text inputs are the most common input elements. The allow a user to input a single line of text.
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="fname">First name:&lt;/label&gt;
                    &lt;input type="text" id="fname" name="fname"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="fname">First name:</label>
                    <input type="text" id="fname" name="fname">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes: 
        #TEXTAREA 
        - id: textarea
          name: Textarea
          description: Textarea elements are like input elements but allow the user to input multiple lines of text.
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="w3review"&gt;Review of W3Schools:&lt;/label&gt;
                    &lt;textarea id="w3review" name="w3review" rows="4" cols="50"&gt;
                    At w3schools.com you will learn how to make a website. They offer free tutorials in all web development technologies.
                    &lt;/textarea&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="w3review">Review of W3Schools:</label>
                    <textarea id="w3review" name="w3review" rows="4" cols="50">
                    At w3schools.com you will learn how to make a website. They offer free tutorials in all web development technologies.
                    </textarea>
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:  
        #COLOR
        - id: color
          name: Color Input
          description: The color input element allows the user to select a single color from a color picker.  
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="favcolor"&gt;Select your favorite color:&lt;/label&gt;
                    &lt;input type="color" id="favcolor" name="favcolor" value="#ff0000"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="favcolor">Select your favorite color:</label>
                    <input type="color" id="favcolor" name="favcolor" value="#ff0000">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:  
        # DATE
        - id: date
          name: Date Input
          description: Date inputs allows the user to select a date using the datepicker.  
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="birthday"&gt;Birthday:&lt;/label&gt;
                    &lt;input type="date" id="birthday" name="birthday"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="birthday">Birthday:</label>
                    <input type="date" id="birthday" name="birthday">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes: 
        #TIME 
        - id: time
          name: Time Input
          description: The time input allows users to input the time using the time input which accepts three separate values for hours, minutes and time of day. 
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="appt"&gt;Select a time:&lt;/label&gt;
                    &lt;input type="time" id="appt" name="appt"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="appt">Select a time:</label>
                    <input type="time" id="appt" name="appt">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:  
        #FILE
        - id: file 
          name: File Input
          description: The file input button allows the user to upload local files from their computer.
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="myfile"&gt;Select a file:&lt;/label&gt;
                    &lt;input type="file" id="myfile" name="myfile"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="myfile">Select a file:</label>
                    <input type="file" id="myfile" name="myfile">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:  
        #PASSWORD
        - id: password
          name: Password Input
          description: The input password is used to input passwords. It visibly masks the input so the user can't see what was entered in the input field. 
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="pwd"&gt;Password:&lt;/label&gt;
                    &lt;input type="password" id="pwd" name="pwd"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="pwd">Password:</label>
                    <input type="password" id="pwd" name="pwd">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes: 
        #EMAIL 
        - id: email
          name: Email Input
          description: The email input is inteneded for users to add their email address. It is very similar to the text input but gives the user some keyboard benefits in mobile browsers.
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="email"&gt;Enter your email:&lt;/label&gt;
                    &lt;input type="email" id="email" name="email"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="email">Enter your email:</label>
                    <input type="email" id="email" name="email">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes: 
        #TELEPHONE 
        - id: telephone
          name: Telephone Input
          description: The telephone input
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="phone"&gt;Enter your phone number:&lt;/label&gt;
                    &lt;input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="phone">Enter your phone number:</label>
                    <input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:
        #NUMBER  
        - id: nubmer
          name: Nubmer Input
          description: The number input
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="quantity"&gt;Quantity (between 1 and 5):&lt;/label&gt;
                    &lt;input type="number" id="quantity" name="quantity" min="1" max="5"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="quantity">Quantity (between 1 and 5):</label>
                    <input type="number" id="quantity" name="quantity" min="1" max="5">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:
        #URL  
        - id: url
          name: URL Input
          description: The url input
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="homepage"&gt;Add your homepage:&lt;/label&gt;
                    &lt;input type="url" id="homepage" name="homepage"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="homepage">Add your homepage:</label>
                    <input type="url" id="homepage" name="homepage">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:
        #SEARCH  
        - id: search
          name: Search Input
          description: The search input
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="gsearch"&gt;Search Google:&lt;/label&gt;
                    &lt;input type="search" id="gsearch" name="gsearch"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="gsearch">Search Google:</label>
                    <input type="search" id="gsearch" name="gsearch">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:
        #DATALIST  
        - id: datalist
          name: Search with Datalist
          description: The datalist input allows the user to select some predefined search options when using the search input. 
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="browser"&gt;Choose your browser from the list:&lt;/label&gt;
                    &lt;input list="browsers" name="browser" id="browser"&gt;
                    &lt;datalist id="browsers"&gt;
                        &lt;option value="Edge"&gt;
                        &lt;option value="Firefox"&gt;
                        &lt;option value="Chrome"&gt;
                        &lt;option value="Opera"&gt;
                        &lt;option value="Safari"&gt;
                    &lt;/datalist&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="browser">Choose your browser from the list:</label>
                    <input list="browsers" name="browser" id="browser">
                    <datalist id="browsers">
                        <option value="Edge">
                        <option value="Firefox">
                        <option value="Chrome">
                        <option value="Opera">
                        <option value="Safari">
                    </datalist>
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:
        #RESET  
        - id: reset
          name: Search with Reset Button
          description: The reset input button clears a search input when clicked. With the reset and datalist elements you can create a more user friendly search experience. 
          example:
            code: >-
                &lt;form&gt;
                    &lt;label for="id"&gt;User ID:&lt;/label&gt;
                    &lt;input type="text" id="id" name="id" /&gt;
                    &lt;input type="reset" value="Reset"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <label for="id">User ID:</label>
                    <input type="text" id="id" name="id" />
                    <input type="reset" value="Reset">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:
        #SUBMIT  
        - id: submit
          name: Submit Button
          description: The submit button sends all form data in a form to the specified location. 
          example:
            code: >-
                &lt;form&gt;
                    &lt;input type="submit"&gt;
                &lt;/form&gt;
            html: >-
                <form>
                    <input type="submit">
                </form>
            hugo: >-
                {{ partial "components/" }}
            javascript: >-
                <component></component>
          attributes:         
---

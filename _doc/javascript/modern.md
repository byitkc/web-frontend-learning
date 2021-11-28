# Modern Javascript

## Classes

``` class.js
class Contact {

    // constructor gets called anytime the class is used
    constructor() {
        this.fullName = form.elements["fullName"].value;
        this.email = form.elements["email"].value;
        this.subject = form.elements["subject"].value;
        this.body = form.elements["msg"].value;
    }

    fullName = "";
    email = "";
    subject = "";
    body = "";

    send() {
        console.info(this.formatMessage());
        showMessage("We're not sending emails yet... feature for version 2.");
    }

    formatMessage() {
        return `To: ${this.fullName}
                Email: ${this.email}
                Subject: ${this.subject}
                Body: ${this.body}`;
    }

};
```

## Modular JavaScript

can use other file names and import where needed.

``` import.js
import Contact from "./Contact.js"; // Imports the default class from import.js
```

## ECMAScript

Standardizing languages across browsers

## Packaging

Take the different files that we are using in Javascript.

### Webpack

- Transpiling - Ensure code is valid in as many browsers as possible

Packages Javascript up into a single document.

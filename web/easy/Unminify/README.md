# Unminify

Category: Web Exploitation  
Difficulty: Easy  

---

Opened the link to the site and it looked normal. had some texts on the page and all that. 

![Login page](screenshots/page.png)



Inside `secure.js`, the credentials were being checked on the client side.

It was basically comparing:
- username ==  admin  
- password ==  strongPassword098765  

![secure.js code](screenshots/secure.png)

So instead of any real server-side validation, the login was just handled in the browser.

I used those values and logged in successfully.

![Logged in page](screenshots/flag.png)


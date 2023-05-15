# Cloning and Pushing to Your Own Repository

1. Fork this repository by clicking the "Fork" button in the top right corner of this page. This will create a copy of this repository in your GitHub account.
2. Clone your forked repository to your local machine using the following command in your terminal:
    - `git clone https://github.com/your-username/javascript-callbacks-assignment.git`
    - Replace `your-username` with your GitHub username.
3. Make changes to the files in your local repository as directed in the exercises.
4. After making changes, add, commit and push your changes to your remote repository using the following commands in your terminal:

```
git add .
git commit -m "Add changes as directed in the exercises"
git push origin main
```

Replace `main` with the name of the branch you want

# Form validation using JS Callbacks
Form validation is the process of ensuring a user's answers to a form are correct, complete, and fit within
some specific criteria (e.g. a password having containing a number or special character), is a VERY
important part of being a fullstack developer as it helps prevent errors, improve data accuracy, and ensures
that no data is missing upon form completion

# Your assignment is to do the following:
1. Write a function called validateForm(e) where e is an 'event' variable (this is default
   behavior for forms - feel free to call it 'event' as well)
2. Inside of validateForm(e), get the information of the form fields by either using querySelectors or by traversing the event object and do the following checks:
     * If the #name input element is empty, send an alert telling the user to enter their name
         using the alert() method and then return false
     * If the #email input element doesn't have a '@' in it, send an alert to tell them to enter
         a proper email and then return false
     * If the #password input element is empty, send an alert telling the user to enter a password
         and return false
     * If the #password input element is less than 8 characters, send an alert telling the user
         their password must be at least 8 characters and then return false
3. If all of the checks pass, return true
4. Lastly, add an event listener onto the form (id="#userForm") that waits for
   a 'submit' event and runs the validateForm callback function when that event happens

Hint: When dealing with a form submission that takes an event variable as a parameter, use e.preventDefault()
      (or event.preventDefault() depending on the name of the variable) to prevent the page
      from refreshing when a form is submitted. Do all your checks after that line.

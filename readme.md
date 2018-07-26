## How to use
Load up https://thejambo.github.io/ToDoInterviewTest/ for the candidate.
Tell them "This is an application we've built interally and are planning to use to track basic tasks day to day, we'd like you to give it a quick test (timeboxed to 20 mins) to identify any issues"

As this is a browser based test, there are a few ways you can suggest they write their findings, such as:
 * [Word Processor](https://www.writeurl.com/)
 * [Spreadsheet](https://ethercalc.org/)
 * [Markdown](https://dillinger.io)
 * Old Fashioned Paper
 
It's importatnt to note that the test itself is not important, we just use the results of the test as a starting point for many different conversations.

### Topics needed to cover:

* Assumptions made (What should the "Clear" button do? Clear completed? Clear Everything?)
  * Who would you clear these assumptions with?
* Field Testing
  * Max values (Length)
  * Unicode?
  * JS Injection?
  * DB Injection? (Did they know it doesn't use a DB?)
* Value of Exploratory vs Script based testing
  * Which will result in finding more issues?
  * Given limited time, which would you focus on any why?
* What is written down in a bug report from this example?
  * Input Provided
  * Expected Output
  * Actual Output
  * Full steps to reproduce?
  * Log files? (if logical error/exception)
  * Screenshot? (if visual error)

## Bugs still to Create

* Editing an item to be empty doesn't delete the item.
* Save blank items

## Current Bugs
* Spelling error (toodo) in instruction text at the bottom of the screen
* Spelling Error in default "What need's to be done?" Text (apostrophe)
* Not counting the number of items properly (-1)
* Active should have a capital 'A' for consistency
* Clear button only clears completed items - Intentional or not? Assumptions will be made here.
* Two 404 errors in the console
* With enough refreshes, the Symbol Ã (A with Tilde) will appear instead of the
 X and â (A with carat/a-circumflex) will appear instead of the "Check All"
 button.
* Undoing "Complete All" takes two clicks
* Delete Task button has a tooltip of "TODO:REMOVE THIS EVENTUALLY"
* When window is made smaller, everything looks fine except the title overlaps itself
* Trimmed items will expand to their original state when editing
* After creating a new item, the "New Item" entry box has 3 spaces in it


## Improvement Suggestions
* Not using HTTPS
* When a large item is created, the "Complete" button is vertically centered, but the delete button is at the bottom.
* Down arrow as "Complete All" is unintuitive
* When adding a new item, page should navigate back to the "All" or "Active" tab to see the new item.

## Worthwhile observations
* It trims spaces at the start and the end and only allows a single space elsewhere.

## How to use
Load up http://todolist.james.am for the candidate.
Tell them "This is an application we've built interally and are planning to use to track basic tasks day to day, we'd like you to give it a quick test (timeboxed to 20 mins) to identify any issues"

As this is a browser based test, there are a few ways you can suggest they write their findings, such as:
 * [Word Processor](https://www.writeurl.com/)
 * [Spreadsheet](https://ethercalc.org/)
 * [Markdown](https://dillinger.io)
 * Old Fashioned Paper
 
It's important to note that the test itself is not important, we just use the results of the test as a starting point for many different conversations.

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
  
* Severity vs Impact of the bugs
  * What is Severity and Impact?
  * How would you prioritise the list you've written?
    * If you only had 5 minutes to retest the application, where would you start?  
    
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
* Not counting the number of items properly (-1)
* Spelling error (toodo) in instruction text at the bottom of the screen
* Active should have a capital 'A' for consistency
* Can't prioritise the tasks / reorder items
* Elements are too pale/small/unreadable
* Undoing "Complete All" takes two clicks
* Spelling Error in default "What need's to be done?" Text (apostrophe)
* Delete Task button has a tooltip of "TODO:REMOVE THIS EVENTUALLY"
* When window is made smaller, everything looks fine except the title overlaps itself
* When a large item is created, the "Complete" button is vertically centered, but the delete button is at the bottom.
* After creating a new item, the "New Item" entry box has 3 spaces in it
* Word Wrapping isn't great - Cuts words apart
* Inappropriate comment in source code.
* Two 404 errors in the console
* Trimmed items will expand to their original state when editing
* Rarely on a refresh, the Symbol Ã will appear instead of the X and â will appear instead of the "Check All" button (Font failing to load)
* When using two tabs, the list is not kept up to date, you need to manually refresh.

## Improvement Suggestions
* Not using HTTPS
* When a large item is created, the "Complete" button is vertically centered, but the delete button is at the bottom.
* Down arrow as "Complete All" is unintuitive
* When adding a new item, page should navigate back to the "All" or "Active" tab to see the new item.

## Worthwhile observations
* It trims spaces at the start and the end and only allows a single space elsewhere.
* Item count should probbably be on a page by page basis, not global.

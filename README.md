### Welcome
Welcome to the Rebol 3 issue tracker, supporting the
development of Rebol 3. We have now completed the migration from our previous
[CureCode instance](http://curecode.org/rebol3/) to Github.

The issues are in this repository under the issues tab:

https://github.com/rebol/rebol-issues/issues

### Using github issues for curecode users
TBC

1. @rebolbot imported everything. How do I seach for issues that I raised? 
  * Try the following search `is:issue is:open "Submitted by: ladislav" in:body`
2. Can I edit my issues which have been imported from curecode?
  * Unfortunately as @rebolbot imported and owns all of the tickets you cannot edit your old tickets. Any new tickets or comments on existing tickets will be editable as expected.
3. Why are the links to other issues not working in some cases?
  * In curecode issues there is often code in the description field. To stop the code being interpreted as markdown the import script escapes quite a lot as code using backticks. The simple rule used to determine if something was text was if the line starts with a capital letter then it is probably text. Not an infallible rule, but surprisingly effective. When text is marked up as code the #1234 links do not work.

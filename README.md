### Welcome
Welcome to the Rebol 3 issue tracker, supporting the
development of Rebol 3. We have now completed the migration from our previous
[CureCode instance](http://curecode.org/rebol3/) to Github.

The issues are in this repository under the issues tab:

https://github.com/rebol/rebol-issues/issues

### Using github issues for curecode users

1. @rebolbot imported everything. How do I seach for issues that I raised? 
  * Try the following search `is:issue is:open "Submitted by: ladislav" in:body`
2. Can I edit my issues which have been imported from curecode?
  * Unfortunately as @rebolbot imported and owns all of the tickets you cannot edit your old tickets. Any new tickets or comments on existing tickets will be editable as expected.
3. Why are the links to other issues not working in some cases?
  * In curecode issues there is often code in the description field. To stop the code being interpreted as markdown the import script escapes quite a lot as code using backticks. The simple rule used to determine if something was text was if the line starts with a capital letter then it is probably text. Not an infallible rule, but surprisingly effective. When text is marked up as code the #1234 links do not work.

#### Issue labels

In CureCode, there are fields like ticket/type, ticket/version, ticket/platform, ticket/status, ticket/category, ticket/severity and ticket/priority. The fields ported to this issue tracker are:

ticket/type

*bug - the ticket describes a bug, transformed to "type.bug" label

*wish - the ticket describes a wish, transformed to "type.wish" label

*note - the ticket is a note, transformed to "type.note" label

*nuts - ??, transformed to "type.alien" label

ticket/severity

*major - the resolution would require major changes to existing code, transformed to "status.important" label

*crash - the issue discusses interpreter crash, transformed to "status.important" label

*block - blocks new code to be written or prevents it to function, transformed to "status.important" label

*not-a-bug - this is not a bug, transformed to "status.dismissed" label

ticket/priority

*high - high priority, transformed to "status.important" label

*urgent - urgent priority, transformed to "status.important" label

*immediate - immediate priority, transformed to "status.important" label

#### CureCode fields not ported

ticket/version - Specifies the version affected by the issue.

ticket/platform - Specifies the platform on which the issue occurs.

*all - all platforms are affected

ticket/status

*submitted - ticket was not reviewed yet

*reviewed - ticket is being reviewed

*problem - there is something problematic about this issue, which needs to be resolved, before it can become actionable

*waiting - waiting for other tickets being resolved, waiting for a good name, etc.

*deferred - revisit later

*dismissed - the ticket has been dismissed

*pending - the pull request resolving the ticket has been submitted and it is waiting for merge

*built - the resolution has been built

*tested - the resolution is being tested

*complete - the ticket has been resolved completely

ticket/category

*documentation

*evaluation

*mezzanine

*native

*datatype

*math

*parse

*ports

*graphics

*syntax

*security

*error handling

*console

*platform

*extensions

*host-kit

*chat

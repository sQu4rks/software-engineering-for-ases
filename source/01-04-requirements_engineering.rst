Requirements Engineering
========================

Requirements engineering aims to capture, document and  maintain the needs and functionalities wished by a user
in a standardized form. 

Regardless of which development model you choose there will be the need to capture requirements at some point. 

User Story
----------

A common tool to capture requirements are **User Stories**. Especially in the agile world user stories commonly serve
as the first requirement document. User stories can be written by everyone in an agile team but it is usually 
the product owners role to maintain the backlog of users stories. In agile new user stories can be added throughout the 
project. 

A user story has the format 

As a *<role>* I can *<capability>* so that *<outcome/reason>*

An example of a user story could be 

As a *Webex Teams user* I can *edit my messages* so that *I can correct my mistakes*

Quite often user stories end up being too large. The example above is a major enhancement that requires a 
multitude of changes across different parts of the software. A reasonable approach would 
be to split this story into multiple sub-stories. Big overarching user stories that contain multiple sub-
stories leading to a common outcome are referred to as a **epic**. 

As a rule of thumb: If a user story can't be implemented by an agile team within one month then it should be split. 

Use Case 
--------

A use case is very similar to a user story but focus on a different aspect. While user stories are about the 
capability of a user, a use case is about the functionality you build into a software to meet the user story. 

Use cases thus specify more aspects than a user story. While user stories should be easily readable by users 
use cases can require in-depth knowledge of your current architecture. 

A good use case captures the following properties 

* **Name** A descriptive name of this use case
* **Summary** A summary of the capabilities/actions carried out in this use case
* **Rational** A description of why this feature/change is useful
* **Users** A list of impacted users 
* **Preconditions** A set of pre-conditions that need to be set in order for this new feature to work 
* **Basic course of events** A basic flow of events that lead to the desired outcome
* **Alternative paths** Alternatives that can be taken in the flow presented above. Typically these are abort of rollback operations.
* **Postconditions** What are the conditions present after the use case has been carried out

With such a use case description a developer has a very clear idea on how to implement the required feature. 

A common pitfall though is to become overly specific. A use case is not about how the software looks like 
but how it behaves and what kinds of interactions the user has. As an example: The search-and-replace use 
case for a terminal-based editor like vim or emacs looks exactly the same as the search-and-replace use case
for a visual application like word. 

Do user stories replace all other types of requirements?
--------------------------------------------------------

User stories are great to serve as an entry point to additional requirement documentation as well as providing a 
simple acceptance test for this requirement. If a user can carry out the operation as described in the user 
story this feature is implemented.

A user story might be linked to a set of interaction diagrams (we will cover these in the section on software architecture),
a flow diagram or a mock-up of a solution. 

What makes a requirement bad?
-----------------------------

It is very hard to specify a good requirement. However the following aspects, sometimes referred to as *requirements smell* 
are a good indicator that requirements are bad. 

* subjective language 
* ambiguous adverbs
* superlatives
* negative statements

Requirements Engineering Lab
----------------------------

In this lab you will specify user stories based on a case study. 

Download the lab guide :download:`here <_static/labs/lab-requirements_engineering.pdf>`.
# Python: Writing tests for your code

[Github Repo](https://github.com/DallasMorningNews/python-testing-101)

* Andrew Chavez

##### Description

Every programmer makes mistakes. Writing good tests can help you avoid making them in production. In this session, you will learn how to use Python's built-in tools to automate testing so you can sleep better at night. 

This session is good for: People who use Python regularly and want to improve their workflow.

## Notes

Code that exercises your code.

Code that ensures consistent behavior of code you've already written.

Gift for future developers who have to maintain your code.

Blueprint for what your code is supposed to do.

Cover things in tests that could keep you up at night. Things that interact with readers or staff.

Regression testing: If something breaks, write a test to make sure it doesn't break again.

Good tests test one narrow behavior. When the test fails, you know exactly what it wrong.

In output:

. = passed test
E = error
F = failed

Coverage.py

makefile to integrate command line into testing (e.g. check for existence of other files)

Testing things with randomness or other behavior:

E.g. site being up. Is your code wrong or is the site down?

Mocking tricks test into returning a different thing than it otherwise would.

Freezegun lets you freeze time. Other mocking libraries let you mock S3, etc.

Setup, Teardown and Class functions for test cases can be useful.

Continuous integration with Circle

Push to git, tests pass, deployed.

##### Speakers

Andrew Chavez is a senior computational journalist on the data and interactives team at The Dallas Morning News and a lecturer at the journalism school at The University of Texas at Austin.

_Description and speakers from [official schedule](https://www.ire.org/events-and-training/event/3189/3631/)_
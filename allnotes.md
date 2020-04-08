# Onsdag, 18 mars, 2015

- This is a test file, to show how a daily journal might look.
# Tuesday, 7 April, 2020

# 15 Jan 2020
* change to American spelling of "canceled'
	* first push to production, learn deployment process

# 16 Jan 2020
* format pending cancel dates in admin date format (admin dashboard)
	* use existing date formatting code

# 21 Jan 2020
* display "only sell packages" and "single photo" from database (admin dashboard)

# 30 Jan 2020
* unit tests for CStringHelper functions

# 3 Feb 2020
* remove cloud download darklaunch logic
	* traced through front end code in cleanup branch

# 7 Feb 2020
* make calendar clickable
	* inline jQuery selector in the view
	* complex selector to grab DOM element and capture click
	* final solution using CSS class pattern to attach handler to element on datepicker init
* make cursor into hand on hover
	* apply CSS class handler pattern

# 11 Feb 2020
* disable cancel after cover upload start
	* apply CSS class handler pattern
	* tracing of logic in front end js

# 12 Feb 2020
* change accented chars to ASCII for username generation
	* set up fixtures for unit testing
	* use locale-specific substitutions for accented chars

# 14 Feb 2020
* use new accented character logic in slug generation
	* reuse code

# 20 Feb 2020
* refactor actionActivation function
	* * big refactor to simplify future development and to clarify logic
	* * broke down tasks into 4 private methods
	* * wrote before and after end-to-end test matrix
	* * prevent users from activating accounts after they're banned by expiring their activation links

# 24 Feb 2020
* disable back after watermark upload start
	* * use CSS class handler pattern from disable cancel after upload start

# 26 Feb 2020
* bugfix / record digital order download size settings in db
	* wrote unit tests

# 5 Mar 2020
* change order download url to use custom domain, if set
	* learned to use fixtures
	* learned to configure routes in main.php
	* refactored to use framework functions to create URLs

# 11 Mar 2020
* create solution to delete IDP cache from CG admin dashboard
	* learned structure of Redis cache
	* learned how to connect CG and IDP together using API endpoint on CG
	* learned how to make call to API endpoint using Guzzle
	* learned about whitelisting endpoints in main.php

# 23 Mar 2020
* generalize DNS lookup refactor
	* broke down DNS record lookups into discrete private functions
	* a lot of manual end to end testing - majority of time spent

# 27 Mar 2020
* validate CAA records
	* simplified code by taking advantage of knowledge of CAA search algorithm

# 27 Mar 2020
* validate AAAA records
	* learned how to use logging system to diagnose problems

# 8 Apr 2020
* fix order exports out of memory
	* difficult refactor due to test being data-dependent
	* reduce risk by launching to admin pages first
	* made tradeoffs between raw SQL queries and ActiveRecord

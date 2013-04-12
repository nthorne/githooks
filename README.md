githooks
========

This repository contains assorted git hooks.


pre-commit.work-unittest
------------------------
This pre-commit hook requires that for each committed cpp file, hpp file or
unit test (a file matching .*Test.?pp) , a CppUnit-style unit test is to be
found in the committed unit's test folder, and the test is required to pass.
Any committed file matching the pattern [Ss]tub\.?pp or residing in a folder
matching the pattern [Ss]tubs will be excluded from any checks.

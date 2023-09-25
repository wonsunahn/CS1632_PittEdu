TEST FIXTURE:
1. Firefox browser version >= 105, or Chrome browser version >= 105 is installed and launched.

TEST CASES:

```
IDENTIFIER: TEST-1-TITLE
TEST CASE: Check that title of the home page is "Department of Computer Science | University of Pittsburgh".
PRECONDITIONS: None.
EXECUTION STEPS: None.
1. Open the URL https://cs.pitt.edu/ on the web browser.
POSTCONDITIONS:
* The title of the page is "Department of Computer Science | University of Pittsburgh"
  (Use "assert title" command.)
```

```
IDENTIFIER: TEST-2-GIVE-BUTTON
TEST CASE: Check that the "GIVE" menu item exists.
PRECONDITIONS: None.
EXECUTION STEPS:
1. Open the URL https://cs.pitt.edu/ on the web browser.
POSTCONDITIONS: 
* A menu item with the text "GIVE" is present on the page.
  (Use "assert element present" command on locator with "GIVE" string.)
```

```
IDENTIFIER: TEST-3-GIVE-LINK
TEST CASE: Check that the "GIVE" menu contains a link to "https://giveto.pitt.edu/giveSCI".
PRECONDITIONS: None.
EXECUTION STEPS:
1. Open the URL https://cs.pitt.edu/ on the web browser.
POSTCONDITIONS: 
* The menu item with the text "GIVE" has an href attribute with the value "https://giveto.pitt.edu/giveSCI".
  (Use "store attribute" command followed by "assert" command.)
```

```
IDENTIFIER: TEST-4-RESEARCH-AREA-COMPUTER-VISION
TEST CASE: Check that the fifth item in the research areas page is "Computer Vision".
PRECONDITIONS: None.
EXECUTION STEPS:
1. Open the URL https://cs.pitt.edu/ on the web browser.
2. Click on the "Research" menu.
3. Click on the "Research Areas" link in the next page.
POSTCONDITIONS: 
* The fifth div element in the research areas list contains the text "Computer Vision".
  (Use "assert text" command on xpath that contains div[5].)
```

```
IDENTIFIER: TEST-5-RESEARCH-AREA-COUNT
TEST CASE: Check that there are 15 areas in the research areas page.
PRECONDITIONS: None.
EXECUTION STEPS:
1. Open the URL https://cs.pitt.edu/ on the web browser.
2. Click on the "Research" menu.
3. Click on the "Research Areas" link in the next page.
POSTCONDITIONS: 
* There are exactly 15 div elements for the 15 research areas.
  (Use "assert element present" for div[15] followed by "assert element not present" for div[16].)
```

```
IDENTIFIER: TEST-6-SEARCH-CSC
TEST CASE: Check that the second item when searching "csc" iis the CSC Officers page.
PRECONDITIONS: None.
EXECUTION STEPS:
1. Open the URL https://cs.pitt.edu/ on the web browser.
2. Click on the search icon.
3. Type "csc" in the search box that pops up.
4. Type [Enter] in the search box.
POSTCONDITIONS: 
* The second div element in the search results has the title:
  "CSC Officers | Department of Computer Science | University of ...". 
  (Use "assert text" for xpath containing div[2].) 
```

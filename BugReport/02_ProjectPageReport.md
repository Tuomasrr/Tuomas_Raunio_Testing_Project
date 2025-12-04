
## Summary (Summarize the bug encountered concisely)
On the GitLab project creation page the button text Create Blank Project is incorrectly displayed as Create Black Project. So there is typo in UI.


## Steps to reproduce     
Open browser, Login to GitLab, Navigate to project creation page (https://gitlab.com/projects/new), Observe the first button that should show "Create blank project", Notice that it says "Create black project"
   

## What is the current bug behavior?
The UI shows incorrect text "Create black project" on the Create blank project box. Functionality still works, but it may confuse users.
     

## What is the expected correct behavior?
UI should display the correct text "Create blank project"

     
## Relevant logs and/or screenshots
![Here's the bug](../Image/Bug_Project_create_blank.png)
![Here's the correct behavior](../Image/Bug_Screenshot.png)
      

## Possible fixes
Correct the text string in project creation page template
Replace the incorrect word "black" with "blank"
Maybe add automated test that check for right labels.
Simple possible solution as line of code:
<button>Create black project</button> -> <button>Create blank project</button>

## Whom do you report/ Assign To/ Tags
Report to: UI Team
Assign to: Frontend Dev
Tags: GitLab, UI, Typo, Project Page, Create Project

## Priority
Minor
As it does not effect on functionality, but may create confusion because the typo.
      

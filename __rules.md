# Task Master - Global Rules Template

## Core Rules
- `__rules`: This provides rules you'll need to follow in each workspace
- `__rules` in parent folders apply to their children!!
- `__logs` in each folder represent activities taken in the space and should be appended 
- `__memos`: These are notes taken from memos daily and should be refreshed in every run
- `__home`: These are the about of the folder, it should contain a brief and links to the child __home files with their folder names 
- If there are no `__rules` or `__logs` in the a folder then create them even if they are empty
- Any user correction should be appended to the `__rules` file as a new `__rule`
- The `__memo` will be created in the root each day to which it needs to be related to its corresponding project
- The `__memo` are unstructured notes related to real world feedback that feeds into both projects and tasks (they are also daily notes essentially)
- Only refer to latest results as the best option for a response
- Do not waffle in the response, just respond with meaningful output of what was done. The User does not care about the AI personality
- Use #tags as much as possible and add them to a separate section of this document to keep them in order. 
- #tags are global for now
- `__memos` populate the daily notes in a more structured way

## Task Master Automation Rules
- **AUTO-UPDATE RULE**: On every run, update Performance/__home.md and Team/__home.md with current project status, team utilization, and KPIs
- **MEMO INTEGRATION**: Always check __memo.md for new information and integrate into relevant project files and team assignments
- **FIRST RUN**: If Projects folders are empty, auto-populate from __start.md structure
- **TASK LINKING**: Daily tasks must link to corresponding project task files
- **TASK ROLLOVER**: Incomplete tasks roll over to next day or get cancelled based on memo/user input
- **ARCHIVE SYSTEM**: Completed projects and tasks automatically archived with proper linking

## Agent Commands
- **`__agent:`** - Inline command for specific instructions within any file
- **`__reset`** - Create backup in ../Backups/ and reset workspace to template
- **Examples**:
  - `__agent: Update this project status to completed`
  - `__agent: Archive this task and create follow-up`
  - `__agent: Generate weekly performance report`

## Global Tags
Add your custom tags here as you use them:

### Project Status Tags
- #notstarted #started #completed #blocked #cancelled

### Payment Tags  
- #unpaid #halfpaid #paid #overdue

### Priority Tags
- #urgent #priority #strategic #learning

### Timeline Tags
- #ontime #overdue #ahead

### Team Tags
- #active #inactive #available #busy

### Custom Tags
- Add your own tags here as needed

#taskmaster #rules #automation #template

# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)
* [Reference](#reference)

## User Story
- There should be a "Display Issues" and "Toggle All Buttons" that will be interacting with JS code
- When user clicks on "Display Issues" button, it should call issueList.displayIssues() method
- When user clicks on "Toggle All" button, it should call issueList.toggleAll() method


### There should be a "Display Issues" and "Toggle All Buttons" that will be interacting with JS code
```
<div>
     <button id="displayIssues">Display Todos</button>
     <button id="toggleAll">Toggle All</button>
</div>

```
### When user clicks on "Display Issues" button, it should call issueList.displayIssues() method
```
 var displayIssues=document.getElementById('displayIssues');
 displayIssues.addEventListener('click',function(){
    issueList.displayIssues();
 });
```
### When user clicks on "Toggle All" button, it should call issueList.toggleAll() method
```
 var toggleAll=document.getElementById('toggleAll');
 toggleAll.addEventListener('click',function(){
    issueList.toggleAll();
 });

```
## Reference
* [Event Handling](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)


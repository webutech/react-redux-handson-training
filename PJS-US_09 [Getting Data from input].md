# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)

## User Story
- Code Refactoring
- There should be a working control for adding issue
- There should be a working control for changing issue
- There should be a working control for deleting issue
- There should be a working control for toggling issue


### Code Refactoring
```
  -------- index.html ---------
  <button onclick="handlers.displayIssues()">Display Todos</button>
  <button onclick="handlers.toggleAll()">Toggle All</button>
  
  -------- script.js ---------
  var handlers={
    displayIssues:function(){
        issueList.displayIssues();
    },
    
    toggleAll:function(){
        issueList.toggleAll();
    }
};

```
### There should be a working control for adding issue
```
--------- index.html -----------
<div>
    <input type="text" placeholder="Enter issue" id="addIssueText">
    <button onclick="handlers.addIssue()">Add</button>
</div>

-------- script.js ------------
 <div>
     <input type="text" placeholder="Enter issue" id="addIssueTextInput">
     <button onclick="handlers.addIssue()">Add</button>
 </div>
```
### There should be a working control for changing issue
```
--------- index.html -----------
<div>
    <input type="number" placeholder="Enter Position" id="changeIssuePositionInput">
    <input type="text" placeholder="Enter issue" id="changeIssueTextInput">
    <button onclick="handlers.changeIssue()">Change</button>
</div>
-------- script.js ------------
changeIssue:function(){
        var changeIssuePositionInput=document.getElementById('changeIssuePositionInput');
        var changeIssueTextInput=document.getElementById('changeIssueTextInput');
        issueList.changeIssue(changeIssuePositionInput.valueAsNumber,changeIssueTextInput.value);
        changeIssuePositionInput.value='';
        changeIssueTextInput.value='';
    } 
```

### There should be a working control for deleting issue
```
--------- index.html -----------
<div>
    <input type="number" placeholder="Enter Position" id="deleteIssuePositionInput">
    <button onclick="handlers.deleteIssue()">Delete</button>
</div>
-------- script.js ------------
deleteIssue:function(){
        var deleteIssuePositionInput=document.getElementById('deleteIssuePositionInput');
        issueList.deleteIssue(deleteIssuePositionInput.value);
        deleteIssuePositionInput.value='';
    }
```

### There should be a working control for toggling issue

```
--------- index.html -----------
<div>
    <input type="number" placeholder="Enter Position" id="toggleIssuePositionInput">
    <button onclick="handlers.toggleComplete()">Toggle</button>
</div>
-------- script.js ------------
toggleComplete:function(){
        var toggleIssuePositionInput=document.getElementById('toggleIssuePositionInput');
        issueList.toggleComplete(toggleIssuePositionInput.value);
        toggleIssuePositionInput.value='';
    }
```



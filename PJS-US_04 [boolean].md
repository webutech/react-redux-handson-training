# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)

## User Story
- issueList.addIssue() method should be able to add one issue object
- issueList.changeIssue() method should change issueText property of issue object
- issueList.toggleComplete() should change the completed status of issue object

Note :  For listed requirements as above we need to make certain changes in the **issueList** object. We want to create an empty issues
array, and addIssue method should add one object and this object will have two properties related to issue and that is issueText and completed status.
follow below code for the required changes. 
```
var issueList={
    issues:[],
  
   };
```
### issueList.addIssue() method should be able to add one issue object
```
var issueList={
    issues:[],
    displayIssues:function(){
        console.log(this.issues);
    },
    
    addIssue:function(issueText){
        this.issues.push({
            issueText:issueText,
            completed:false
        });
        this.displayIssues();
    }
  
   };
```
### issueList.changeIssue() method should change issueText property of issue object
```
var issueList={
    issues:[],  
    .............
    .............    
    changeIssue: function(position, issueText){
        this.issues[position].issueText=issueText;
        this.displayIssues();
    }
   };
```
### issueList.toggleComplete() should change the completed status of issue object
```
var issueList={
    issues:[],
    .............
    .............
    toggleComplete:function(position){
        var issue=this.issues[position];
        issue.completed=!issue.completed;
        this.displayIssues();
    },
    
    .............
    .............
    
};
```



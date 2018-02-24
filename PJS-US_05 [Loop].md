# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)
* [Reference](#reference)

## User Story
- displayIssues should display issueText
- displayIssues should check if issues array is empty
- displayIssues should show completed


### displayIssues should display issueText
```
var issueList={
    issues:[],
  
    displayIssues:function(){
        console.log('My Issues : ');
        for(var i=0;i<this.issues.length;i++){
            console.log(this.issues[i].issueText);
        }        
    }
    };
```
### displayIssues should check if issues array is empty
```
  var issueList={
    issues:[],
  
    displayIssues:function(){
        if(this.issues.length===0){
            console.log('There is no issue in issue list');
        }
        else{
            console.log('My Issues : ');
            for(var i=0;i<this.issues.length;i++){
                console.log(this.issues[i].issueText);
            }            
        }
        
    }
    };
```
### displayIssues should show completed
```
var issueList={
    issues:[],
  
    displayIssues:function(){
        if(this.issues.length===0){
            console.log('There is no issue in issue list');
        }
        else{
            var issueWithCompletedStatus='';
            console.log('My Issues : ');
            for(var i=0;i<this.issues.length;i++){
                var issue=this.issues[i];
                if(issue.completed===true){
                    issueWithCompletedStatus='(X)'+issue.issueText;
                }
                else{
                    issueWithCompletedStatus='()'+issue.issueText;
                }
                console.log(issueWithCompletedStatus);
            }            
        }        
    }
    };
```
## Reference
* [Loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)


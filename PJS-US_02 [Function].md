# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)
* [Reference](#reference)

## User Story
- It should have a way to add an issue in the issues list using function
- It should have a way to display issues list using function
- It should have a way to change an issue in the issues list using function
- It should have a way to delete an issue from issues list using function

## Code Snippet

### It should have a way to add an issue in the issues list using function
```
 function addIssue(issue){
  issues.push(issue);
  displayIssues();
 }
```

### It should have a way to display issues list using function
```
 function displayIssues(){
  console.log('My Issues : ',issues);
 }
```

### It should have a way to change an issue in the issues list using function
```
 function changeIssue(position,newIssue){
  issues[position]=newIssue;
  displayIssues();
 }
```

### It should have a way to delete an issue from issues list using function
```
 function deleteIssue(position){
  issues.splice(position,1);
  displayIssues();
 }
```
## Reference
* [Functions - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

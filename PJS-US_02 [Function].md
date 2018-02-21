# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)
* [Reference](#reference)

## User Story
- It should have a way to add issue using function
- It should have a way to display issues using function
- It should have a way to change a issue using function
- It should have a way to delete a issue using function

## Code Snippet

### It Should have a way to add issue using function
```
 function addIssue(issue){
  issues.push(issue);
  displayIssues();
 }
```

### It should have a way to display issues using function
```
 function displayIssues(){
  console.log('My Issues : ',issues);
 }
```

### It should have a way to change a issue using function
```
 function changeIssue(position,newIssue){
  issues[position]=newIssue;
  displayIssues();
 }
```

### It should have a way to delete a issue using function
```
 function deleteIssue(position){
  issues.splice(position,1);
  displayIssues();
 }
```
## Reference
* [Functions - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

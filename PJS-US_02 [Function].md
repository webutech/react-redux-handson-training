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
 }
```

### It should have a way to display issues using function
```
 console.log('My Issues : ',issues);
```

### It should have a way to change a issue using function
```
 issues[1]='changed';
```

### It should have a way to delete a issue using function
```
 issues.splice(1,1);
```
## Reference
* [Functions - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

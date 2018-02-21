# Contents

* [User Story](#user-story)
* [Code Snippet](#code-snippet)
* [Reference](#reference)

## User Story
- Your issue-tracker app should have a place to store issues
- It should have a way to add issue
- It should have a way to display issues
- It should have a way to change a issue
- It should have a way to delete a issue

## Code Snippet

### Your Issue-Tracker app should have a place to store issues
```
 var issues=['issue-1','issue-2','issue-3'];
```
### It Should have a way to add issue
```
 issues.push('issue-4');
```

### It should have a way to display issues
```
 console.log('My Issues : ',issues);
```

### It should have a way to change a issue
```
 issues[1]='changed';
```

### It should have a way to delete a issue
```
 issues.splice(1,1);
```
## Reference
* [Array - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

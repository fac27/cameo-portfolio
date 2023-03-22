# Testing
We were tasked to create a simple to do list tracker that allows users to create, complete, and remove tasks from a list. 
In our spike was templates, custom elements, nodelists, advaned CSS selectors, formatting code, and a workshop on testing. 

We had criteria whereby we need to have a working to do list, tests for at least 3 user stories, a responsive mobile first 
design, and ensure that the app is accessible by as many users as possible.

I found this projec the most difficult. While we were able to have the to do list working, we weren't able to narrow our scope in 
time and write modular testable functions. 

## 1. Check that passing a given input into our tests returns the expected output
We started off by writing 3 functions that we wrote tests for. Unfortunately, these functions grew with 'scope creep.' 
Our aim was to create an array and that when a user input a task that array would grow and we could test this with the below test. 

```javascript 
//Add tasks to a list so that I can keep track of them
test("Submitting a new task adds it to the list", () => {
  const result = addTask([], "item");
  console.log("Actual result:", result);
  equal(result.length, 1, "Submitting a new task adds it to the list");
});
```
## 2. Write tests to mimic the behaviour of a user performing different actions

## 3. Write testable, modular functions

## 4. Write functions that add, remove or modify DOM nodes

## 5. Apply event listeners to HTML form elements

## 6. Use scope to control what variables are accessible inside functions and blocks

## 7. Use CSS grid to make layouts that adapt to the viewport size
```CSS
@media screen and (min-width: 450px) {
  .two-columns {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr;
    gap: 10px;
  }
  #todo-list {
    grid-column-start: 1;
    grid-column-end: 2;
  }
  #completes {
    grid-column-start: 2;
    grid-column-end: 3;
  }
}
```

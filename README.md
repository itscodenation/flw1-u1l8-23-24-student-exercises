# Lesson 1.8: DOM Manipulation, Part 3, Review & Project Work Time

## 🔀 DOM Manipulation

So far, we’ve learned to update HTML dynamically using JavaScript. Today, we'll expand on this by adding elements to the DOM. We'll majorly focus on two methods: `createElement` and `appendChild`.

### createElement()

This JavaScript method creates an HTML element:

```javascript
let par = document.createElement("p");
```

Even though the element is created, it hasn't been added to the DOM yet. Once created, you can manipulate its properties:

```javascript
let img = document.createElement("img");
img.src = "fox.jpeg";
let para = document.createElement("p");
para.innerHTML = "Hello!";
```


### appendChild()

Once you've created an element, you'll want to add it to the DOM. This is where `appendChild()` comes in:

```javascript
let body = document.querySelector("body");
let para = document.createElement("p");
document.body.appendChild(para);
```

This method adds the created element as the last child of the target element. Keep in mind the order, especially when nesting elements.
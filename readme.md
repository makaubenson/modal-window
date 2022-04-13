## DOM Manipulation

- We use `querySelectorAll()` to select several elements with the same class name
- They ussualy form an array which is then looped through to access each single button.
- `const btnsOpenModal = document.querySelectorAll('.show-modal');`
- `console.log(btnsOpenModal);`- //Looping through three buttons with the same class
- `for (let i = 0; i < btnsOpenModal.length; i++)`
- `{ console.log(btnsOpenModal[i].textContent); }`
- `btnsOpenModal` is treated as an array

## Events Continuation

- To track an event, we must attach an event handler/listener to the element

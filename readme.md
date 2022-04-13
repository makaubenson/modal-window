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

### Removing classes from divs

- `modal.classList.remove('hidden');` - Note: we do not use dots(.) while specifying the class name. The dot is ONLY for the selector
- To parse multiple classes we write it like : `modal.classList.remove('hidden', 'about', 'love');`
- `modal.classList.remove('hidden');`
- Alternative
- `modal.style.display = 'block';`
- Both achieve the same goal
- `btnCloseModal.addEventListener('click', closeModal);` is used instead of `btnCloseModal.addEventListener('click', closeModal());` - This is because, closeModal() would get executed immediately the line is reached. While what we need is that closeModal is called once a click event has been captured.
- For global events we ussualy listen on the whole document.

#### There are 3 types of events for the keyboard

- keydown- fired as soon as we press down a key
- keyup - fired when we lift our finger off the key
- keypress - fired continuously as we keep our finger on a certain key
- `document.addEventListener('keydown', function () { console.log('A key was pressed'); });` - is executed for any key on the keyboard.

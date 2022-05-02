Tasks
The books array contains books in the following format:
{
  "title": "",
  "authors": ["", ""],
  "description": "",
  "price": 0,
  "rating": 5,
  "quantity": 1
}
Write the following functions in the index.js file.

renderBook()
This function accepts a book object in the format described above.
Create and return the HTML to render a single book. The HTML for a single book should look like this:
<div class="book">
  <div class="details">
    <div class="title">
      Elements of the Theory of Computation
      <span class="rating">(4.7 stars)</span>
    </div>
    <div class="authors">by Harry Lewis, Christos H. Papadimitriou</div>
    <div class="description">
      Algorithms, complexity analysis, and algorithmic ideas are introduced
      informally in Chapter 1, and are pursued throughout the book.
    </div>
    <button class="removeBtn">Remove from cart</button>
  </div>
  <div class="quantity">2 @ $182.65</div>
  <div class="price">$365.30</div>
</div>

calculateTotal()
Calculate and return the total price of all items in the cart. The function should return 0 when the cart is empty and should also consider the quantity for multiple items.

render()
Render the array of books and the cart total and insert them into the DOM.
The books should be rendered in the section with ID cartItems. 
If there are no items in the cart, the text "Nothing in cart" should be inserted here instead.
The total should be rendered in the div with class total-price in the section with ID cartTotal. 
If there are no items in cart, the total should show "\$0".

<!-- sortByPrice()
Sort the books array by price in ascending order.
Attach an event listener to the #sortBtn button that firsts sorts the array with the sortByPrice() function, then calls render(). -->

main()
Perform all the startup tasks in the main function:
- Attach required event listeners
- Call the render() function
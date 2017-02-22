## Cashier Lab

- Use the `create-react-app` CLI to generate your skeleton app. Type `yarn start`, and code away!

- Spend **at least** the first 15 minutes:
  - Wire-framing your app's UI.
  - Identifying the React components that the UI will be composed of - be sure to draw a rectangle around each component as shown in [Thinking in React](https://facebook.github.io/react/docs/thinking-in-react.html).
  - Which components are stateful, which are stateless?

- Once your component hierarchy is laid out, build your page with static/skeleton versions of those components. Then, add the dynamic behavior. 

- Complete as many of the User Stories, in sequence, as you can. Don't expect to finish all of them.

### Cash Register

The _Cash Register_ is a fun to use cash register.

##### User Stories

- AA Cashier, I would like to see the list of items for purchase on the left side of the display.

- AA Cashier, I would like to click a "Purchase" button displayed near to the item I want to add to the order.

- AA Cashier, I would like to see a detailed running receipt on the right of the display that is updated as items are added to the order.

- AA Cashier, I want the receipt to show the _Desc_, _Price_ for each item; and the _Order Total_ so that I can inform the customer how much they owe.

- AA Cashier, I would like to clear the current order and start a new one.

- AA Cashier, I would like to be able to remove a purchased item from the receipt in case I make a mistake or the customer changes their mind.

- AA Cashier, I don't want to see the "Purchase" button displayed for items already purchased.

- AA Cashier, I would like sales tax at a rate of 10.5% displayed and added to the _Order Total_ so that the government can get their piece of the action.

- AA Cashier, I would like to like to display the _Qty_ and _Ext. Price_ (in lieu of _Price_).

- AA Cashier, I would like to and be able to easily increase/decrease the _Qty_ and have the item be removed from the order if the _Qty_ is zero.

- AA Cashier, I would like to be able to type in an item's SKU and press enter instead of clicking on the item in the UI because I'm less likely to get Carpal Tunnel Syndrome.

##### Notes

- Here's your array of items available for purchase. These can be passed in as state for a top-level component.

  ```js
  var items = [
    {category: "Meat & Poultry", sku: 1001, desc: "Rib-eye Steak", price: 12.95},
    {category: "Meat & Poultry", sku: 1023, desc: "Free-range Chicken", price: 6.95},
    {category: "Meat & Poultry", sku: 1045, desc: "Bacon", price: 3.79},
    {category: "Dairy", sku: 2005, desc: "American Cheese Slices", price: 5.59},
    {category: "Dairy", sku: 2012, desc: "Milk (Low-fat)", price: 1.99},
    {category: "Dairy", sku: 2014, desc: "Milk (Whole)", price: 2.29},
    {category: "Dairy", sku: 2034, desc: "Cream Cheese", price: 3.25},
    {category: "Produce", sku: 3002, desc: "Lettuce (Iceberg)", price: 1.25},
    {category: "Produce", sku: 3005, desc: "Lettuce (Romaine)", price: 2.39},
    {category: "Produce", sku: 3013, desc: "Tomato (Organic)", price: 0.99},
    {category: "Bread", sku: 4010, desc: "Loaf (White)", price: 1.99},
    {category: "Bread", sku: 4015, desc: "Loaf (Wheat)", price: 2.59},
    {category: "Bread", sku: 4021, desc: "Buns (Hotdog)", price: 1.75},
    {category: "Bread", sku: 4023, desc: "Buns (Hamburger)", price: 3.00}
  ];
  ```

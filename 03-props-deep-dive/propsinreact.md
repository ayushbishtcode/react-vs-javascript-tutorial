1. What are Props?
   Props = Properties (like properties of an object)

Think of props as "ingredients" you give to a recipe (component).

javascript
// Recipe (Component)
function Pizza({ cheese, toppings, size }) {
return `A ${size} pizza with ${cheese} cheese and ${toppings}`;
}

// Using the recipe with different ingredients
Pizza({ cheese: "Mozzarella", toppings: "Mushrooms", size: "Large" });

2. Props = Function Parameters (Your Example)
   Let's break down your example step-by-step:

javascript
// STEP 1: Normal JavaScript function
function makePizza(type) {
return `Making a ${type} pizza`;
}
// Calling it:
makePizza("Margherita"); // "Making a Margherita pizza"

// STEP 2: React Component (Same concept!)
function Pizza({ type }) {
return <h2>Making a {type} pizza</h2>;
}
// Using it:
<Pizza type="Margherita" />
// Output in browser: <h2>Making a Margherita pizza</h2>

See the similarity?

makePizza("Margherita") → passes "Margherita" as parameter

<Pizza type="Margherita" /> → passes "Margherita" as prop

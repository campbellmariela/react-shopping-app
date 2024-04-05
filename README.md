# React shopping app

The shopping app is a project developed following the guidelines offered by the IBM course “Developing front-end apps with React”.

The shopping app is a web page that calculates the total value of a purchase and changes the currency according to a selected location from a list provided.

The page has a list of predefined items with their prices and allows the user to add or reduce the quantity of a selected item. Once the quantity is modified it calculates the item's price and the cart value. The user can also remove the item from the shopping cart by clicking the icon from the "remove" row.

## Run
To run the shopping app on your desktop, you need to: 
1. Install [Node.js](https://nodejs.org/en/download).
2. Clone the repository.
3. Install all necessary packages. All packages required to be installed are listed in package.json. Run `npm install -s`, to install and save those packages.
4. Run the server using the following command: `npm start`. 
5. Finally, open [http://localhost:3000](http://localhost:3000) to view it in your browser.

## App structure

* src   
    * components 
        * CartValue 
        * ExpenseItem 
        * ExpenseList 
        * ItemSelected 
        * Location
    * context 
        * AppContext.js 

The shopping app has five components. All of these components will be using redux for state management through AppContext.js. 

In AppContext.js a reducer is created, which is used to update the state, based on the action. 

In AppContext.js we are setting the initial state of Expenses and Location. Also, we are creating a provider component, setting up the useReducer hook which will hold the state, and allow us to update the state via dispatch.

# Corner Store Refactoring Kata PHP

This is inspired by [Emily Bache's Gilded Rose](https://github.com/emilybache/GildedRose-Refactoring-Kata).

=============== Specifications ===============

Basic rules:
- All items have a daysUntilExpired value which denotes the number of days we have to sell the item 
- All items have a price value which denotes how valuable the item is 
- At the end of each day our system lowers both values for every item

Some additional rules:
- Once the sell by date has passed, price reduces twice as fast 
- The price of an item is never negative 
- "Twinkie" actually increases in price the older it gets 
- The price of an item is never more than 50 
- "Beef Jerky", being a legendary item, never has to be sold or decreases in price 
- "Lotto Tickets", like Twinkie, increases in price as its daysUntilExpired value approaches; price increases by 2 when there are 10 days or less and by 3 when there are 5 days or
less but price drops to 0 after the concert

Feel free to make any changes to the updatePrice method and add any new code as long as everything still works
correctly. However, do not alter the Item class or Items property.

Just for clarification, an item can never have its price increase above 50, however "Beef Jerky" is a legendary item and
as such its price is 80 and it never alters.

## Getting Started

1. Install the composer packages.
2. Run phpunit to generate the snapshot.
3. Run phpunit again to assert the snapshot stayed the same

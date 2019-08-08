**Handy Hardware**

Description: *Handy hardware is a text based storefront with a MySQL model to control Inventory.*

Technologies used: Node.js w/Inquirer, and MySQL.

Simply put, Handy Hardware is an Inquirer based text app. It prompts the  user to choose: *browse, search by name,* or *search by ID*.

The user then choose an activity and based upon their selection, the program calls the corresponding function. the function then prompts the user for more input.

The browse function displays a scrollable list of tools. the user can select a tool and buy it, or order more. if they select buy it asks for quantity and then validates the quantity vs. inventory  number. if the inventory is greater than the request, the inventory is reduced by the requested number.

The search function utilizes a *select-from-where* model to find the corresponding tool in the SQL tables. Then it calls the buy function which  adjusts the inventory based on the user selection. 


Search by ID does the same thing, but with an ID number instead of name. 

after each function the program checks to see if the inventory numbers are below a certain theshold. if they are that tools is then added to an *to order* table.





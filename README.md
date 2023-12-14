# python-challenge-1
## Dylan Ross

### Creating an order system

This challenge was issued to me by UNC to adapt an order taking system, which included storing the customer's order and outputting the receipt with the total price of all items ordered.

#### First steps

Firtly, we started with an empty menu called 'order_list', and then greeted the customer.
Next a while loop was already provided for in the file. it consisted of this.

![](<Screenshot 2023-12-11 084648.png>)

We then created a for loop to see what menu the customer chose, validating that their item was in the list and was a digit. Then a pre-created format for the menu was provided for in the file. If invalid we print an error message. After that a format for the menu was provided for.

![](<Screenshot 2023-12-11 085314.png>)

This was a good blueprint for the challenge.

After we stored the input as a variable, the custoemer is asked how many they would like, and as above check the validation. If it wasn't a number, their selection would be defaulted to 1.
We then .append their selection to the order_list.

![](<Screenshot 2023-12-11 090902.png>)

We we're then instructed to do a match:case statement inside the While loop, that checked for (Y) or (N) converting the string to upper case so that it validates. If we got a wildcard statement we promted them again.

#### The Receipt

A for loop was created so that we could iterate through the items that the customer ordered. It consisted of a space string and lines to replicate the formate provided for in these print statements.

![](<Screenshot 2023-12-11 091942.png>)

We created a space_str variable and substracted the length of the item name to correctly format this.

#### The difficult part for me

Printing the total using sum().
I had figure it out by settint total = 0 and doing a for loop that augmented  total += (quantity * prices).
This had the desired outcome, however the instructions imclipcitly stated they wanted sum() to be used.
The problem was i was trying to do this in a for loop, and to my discovery while in a for loop sum() doesnt work with floats, whereas in list comprehension is does work. I forgotten what list comprehension until Aditya Jamwal reminded me what it was.

Overall the project was straight forward, and easy to figure our once I realized where my mistake was.

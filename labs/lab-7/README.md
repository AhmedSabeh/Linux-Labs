# Lab 7: Text Editing Challenge

## Objective
Practice creating and editing text files using both interactive editors and direct command-line methods.

---

## Steps

1. **Use nano to create a file called `shopping_list.txt`**
   ```bash
   nano shopping_list.txt
Add 5 items to your shopping list
Example content inside nano:

nginx
Copy
Edit
Milk
Bread
Eggs
Apples
Coffee
Save with CTRL + O → Enter

Exit with CTRL + X

Add one more item to the end of the file without opening an editor

bash
Copy
Edit
echo "Cheese" >> shopping_list.txt
Display the final shopping list

bash
Copy
Edit
cat shopping_list.txt
Example output:

nginx
Copy
Edit
Milk
Bread
Eggs
Apples
Coffee
Cheese

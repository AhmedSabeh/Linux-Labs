# Lab 7: Text Editing Challenge

## Objective
Practice creating and editing text files using both interactive editors and direct command-line methods.

---

## Steps

1. **Use nano to create a file called `shopping_list.txt`**
   ```
   nano shopping_list.txt
   ```
2. **Add 5 items to your shopping list**
-   content inside nano:

<img width="925" height="485" alt="Screenshot (208)" src="https://github.com/user-attachments/assets/3004b914-fff5-42b2-96b0-451573326b9a" />


-   Save with CTRL + O → Enter

-   Exit with CTRL + X

3. **Add one more item to the end of the file without opening an editor**
```
echo "Cheese" >> shopping_list.txt
```
4. **Display the final shopping list**
```
cat shopping_list.txt
```
-   Output:

<img width="922" height="238" alt="Screenshot (207)" src="https://github.com/user-attachments/assets/d5a1b752-2e36-4d06-93b3-2ee3b223dbc7" />

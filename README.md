# Data Cleaning using MS EXCEL

In this project I have used a sample data set to perform data cleaning in Microsoft Excel and listed below are the steps that I have taken in this process.

### Removing Blank Cells

Select the column in which you want to perform the data-cleaning process. After this step, select the option named _blank_ and deselect other options

![Untitled](https://github.com/user-attachments/assets/6328c1c6-7bad-442b-9045-5f634274f653)

![image](https://github.com/user-attachments/assets/2a1f4628-9386-48b1-864f-b64074279015)

As observed below, blank cells get highlighted and we can rectify or remove the corresponding row from the dataset. 

Note: If you simply deleted the data from the row by tapping the backspace button, you will need to go a step further and delete the empty row entirely.

![image](https://github.com/user-attachments/assets/6def443c-d181-4200-b62b-d4591f7c9e4c)

Once you are done deleting the rows with blank values, right-click on the dropdown arrow on that column and select "Clear Filter" as shown in the image below. Repeat the above steps to delete all the blank cells and curate the dataset.

![image](https://github.com/user-attachments/assets/2a01f7c9-bd7e-4556-bba7-a44f2a153348)

### Transposing the data
The action of converting the data from the current long format (more rows than columns) to the wide format (more columns than rows) is called transposing. 

The below-given steps can be used to perform the Transpose function in Excel:

1. Select the entire table from A1 to H45 as seen below and copy the data using Ctrl+C

![image](https://github.com/user-attachments/assets/09ac7ea7-2adf-4e17-ba01-cc52d9b3acb3)

2. In the new sheet right-click on cell A1 and select "Transpose" under _Paste Special_ on the dropdown

![image](https://github.com/user-attachments/assets/2e16edc1-7e46-482b-b4ef-7e64368c1e02)

As you can see in the above image the long data gets converted into wide data

### Deleting extra spaces from data within the cells

Now that you have transposed the data, eliminate the extra spaces in the values of the cells using the TRIM function i.e ```=TRIM(text)``` in Excel.

![image](https://github.com/user-attachments/assets/bb1ca9d1-3e3e-418e-9dce-11d1222a966e)

As you can see we have an extra blank space in cell E2 for the word Binders.Using the Trim function we can eliminate this space from the cell which can be further done for the whole row by just dragging the corner of the cell.

![image](https://github.com/user-attachments/assets/baf3f28f-bf76-4e2a-83ec-50c7b9ac7646)

![image](https://github.com/user-attachments/assets/565ab4d7-3a5f-441e-aa82-ede536a943b5)

However, it is a challenge to perform the TRIM function on a column like the Dates column and hence we use the below-given steps. 

First, we change the format of the date and then 

![image](https://github.com/user-attachments/assets/06b1bed5-5b71-48ed-8022-12b2ff98d79a)

When we perform the TRIM function, the problem that comes up is that most of the values within the cells become non-visible for the date column.

![image](https://github.com/user-attachments/assets/734e1f45-728e-4b61-a82b-f117f6fd9e70)

To fix this simply press Alt + H + O + I to autofit the columns and  Alt + H + O + A to auto-fix the rows or perform the below steps.

![image](https://github.com/user-attachments/assets/04194c04-4c03-4851-bc52-7fa7d2c8ac7c)

Here we get our desired result.

![image](https://github.com/user-attachments/assets/aa68d56d-3667-412a-bb2e-c1dd4472ae07)

### Changing Lower/Upper/Proper case text

To change the format of the text to lowercase first create a new column by simply pressing Ctrl+Shift+Plus and we use the following function.
```
=LOWER(text)
```

![image](https://github.com/user-attachments/assets/c1e888d4-7210-49e8-9ab0-3ff7059fd806)

As we select the text in this new column, Excel reads it as a formula and not as a value as shown below.

![image](https://github.com/user-attachments/assets/4bb1d745-4404-4c8a-b5a8-5fd385737239)

To fix this we select the entire column by using the Ctrl+Shit+Down arrow. After this step, press Ctrl+C to copy the column and use the _Paste_ in the top left corner to select _Paste Values_ from the drop-down menu. Finally, press ctrl+minus to clear the previous column.

![image](https://github.com/user-attachments/assets/5135c9b1-4995-4f3f-8015-e3ec91f2e37c)

Now we can see the value instead of the formula as shown in the above picture.

![2](https://github.com/user-attachments/assets/62e07452-1941-473f-a058-03eb5a8a2438)

Similar steps can be performed to make the strings uppercase. To do this simply replace the _LOWER_ keyword in the formula with _UPPER_ keyword.

Finally, the last type of text-correction function i.e. Propercase function, is needed in scenarios where we have a string with a mix of uppercase and lowercase letters. Below is one such example where we have successfully fixed the characters using the Propercase function.

![image](https://github.com/user-attachments/assets/f4cec89d-7bc0-495d-b23e-ae8038ae2f07)

![image](https://github.com/user-attachments/assets/d0d27f51-a1ce-466b-905d-8d5a0de902b6)

By using the various functions discussed above, I was able to fix all the characters, remove blank values and finally have the dataset cleaned for analysis.

![image](https://github.com/user-attachments/assets/575d984c-e704-4878-bde3-5924a6c12071)

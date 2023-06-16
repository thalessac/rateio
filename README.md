# How to run the script

This script runs at Google Colab Virtual Machine. To access it, you'll need to create or log in into your Google Account. Code is executed in a virtual machine private to your account.

On `rateio.ipynb` Notebook file, click on 'Open in Colab' button in the very top of the file. You'll be redirected to the Notebook environment where you'll be able to run it.

All files and variables processed during runtime are removed when you close your session.

### User inputs

First you'll need to provide:


**1.   Invoice values:** 

Insert them in the forms you'll find on the top of the Notebook, as they appear on the invoice

*   `taxa_adm` (Taxa de administração)
*   `fetransp` (Repasse FETRANSPOR)
*   `desconto` (Total "Desconto ref. avisos de crédito" value)
*   `invoice_total_amount` (Total amount of the invoice - used to validate pro-rating calculation)


**2.   Excel files:**

When you execute the code, you'll be requested to upload the following files:

*   `exclusão.xlsx`: required columns ("matrícula", "funcionário", "total bilhete", "compõem aviso de crédito?")
*   `itens_processados.xlsx`: required columns ("matrícula", "funcionário", "total bilhete")
*   `cadastrão.xlsx`: required columns ("cpf", "centro de resultado - código")

Note that file and tables headers MUST follow the above mentioned predefined names, otherwise the script will fail. There is no problem having more columns in your input files, since the mandatory ones are included. Header and file names are not case sensitive, so just make sure the spelling is correct.

Beware that the headers of your tables MUST be on the first row of the Excel. Also make sure that your table is always located at first Row, Column and Sheet of the Excel file. The headers of your tables must be plain text, e.g. no line breaks allowed.

You can also directly upload your files on 'Files' section in the left side bar of the Notebook.

**3.   Missing CCs:**

It is possible that when joining information from `rateio.xlsx` & `exclusão.xlsx` with `cadastrão.xlsx`, some people, for different reasons, are not assigned to any CC. In such cases you'll be requested to manually input a CC value for this person. Write down the CC value on the corresponding field and press 'Enter' to continue.

![image](https://github.com/thalessac/rateio/assets/67764861/0b273db3-4f5b-454c-b08f-9983217f06c8)

### Running the script

Once you provided the invoice input values, press 'Execute cell' button:

![image](https://github.com/thalessac/rateio/assets/67764861/18299d3a-03f7-4e8c-aae9-97009ba6edf7)

Some useful information will be written below the forms for you to track the status of the execution. Possible error messages can also pop up - check them, most likely they'll be related to your data input. 

### Check the outputs
After a successful run, you'll see an output as follows, describing your input values and calculation steps of the script.

![image](https://github.com/thalessac/rateio/assets/67764861/aaee7e69-d0b7-4f12-a8fb-1c870170e838)

Finally, go to the 'Files' section on the left side bar and dowload the file named `rateio.xlsx`. If you don't immediately see it, right click on the 'Files' section and press 'refresh' button.

### Demo application

Run the script using the files found on `data_demo` folder and invoice values from this user guide to get familiar with the script.

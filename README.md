# How to run this script

This script runs at Google Colab virtual machine. In order to do so, you'll need to log in into your Google Account. 
On `rateio.ipynb` file, click on 'Open in Colab' button in the very top of the file. You'll be redirected to the Notebook where you'll be able to run it.

### User inputs

First you'll need to provide:


1.   Invoice values: insert them in the forms you'll find on the top of the Notebook, as they appear on the invoice


*   `taxa_adm` (Taxa de administração)
*   `fetransp` (Repasse FETRANSPOR)
*   `desconto` (Total "Desconto ref. avisos de crédito" value)
*   `invoice_total_amount` (Total amount of the invoice - used to validate pro-rating calculation)


2.   Excel files:
when you execute the code, you'll be requested to upload the following files:


*   `exclusão.xlsx`: required columns ("matrícula", "funcionário", "total bilhete", "compõe aviso de crédito")
*   `itens_processados.xlsx`: required columns ("matrícula", "funcionário", "total bilhete")
*   `cadastrão.xlsx`: required columns ("cpf", "cc")

Note that file and tables headers MUST follow the above mentioned predefined names, otherwise the script will fail. There is no problem having more columns in your input files, since the mandatory ones are included. Header and file names are not case sensitive, so just make sure the spelling is correct.

Beware that the headers of your tables MUST be on the first row of the Excel. Also make sure that your table is always located at first Row, Column and Sheet of the Excel file.

You can also directly upload your files on 'Files' section in the left side bar of this Notebook.

### Running the script

Once you provided the invoice input values, press 'Execute cell' button:

![image](https://github.com/thalessac/rateio/assets/67764861/18299d3a-03f7-4e8c-aae9-97009ba6edf7)

### Check the outputs
After a successful run, you'll see an output as follows, describing your input values and calculation steps of the script.

![image](https://github.com/thalessac/rateio/assets/67764861/aaee7e69-d0b7-4f12-a8fb-1c870170e838)

Finally, go to the 'Files' section on the left side bar and dowload the file named 'rateio.xlsx'. If you don't immediatly see it, right click on the 'Files' section and press refresh button.

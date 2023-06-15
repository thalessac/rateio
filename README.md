# How to run this script

### User inputs

First you'll need to provide:


1.   Invoice values: insert them in the forms you'll find on the cell right after this User Guide, as they appear on the invoice


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

You can also directly upload your files on 'Files' section in the left side bar of this Notebook.

### Running the script

Once you provided the invoice input values, press 'Execute cell' button below.
![image](https://github.com/thalessac/rateio/assets/67764861/930a520e-5c5a-4e42-a084-9b1b7b106b9b)


### Check the outputs
After a successful run, you'll see an output as follows, describing your input values and calculation steps of the script.

![image](https://github.com/thalessac/rateio/assets/67764861/47a5e010-ed7f-4f7b-bc5f-e9a066669d42)

Finally, go to the 'Files' section on the left side bar and dowload the file named 'output_table.xlsx'

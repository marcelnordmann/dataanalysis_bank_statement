Explanations:

1. The file "bank_statement.csv" is an example bank statement file.
2. The file "processed.ipynb" creates a processed bank statement by assigning categories, maingroups and subgroups to every transaction via pre defined search terms. Also the user can add cash payments.
3. The file "bank_statement_processed.csv" is created by executing the code in the file "processing.ipynb". It contains the bank statement info but in a processed way, ready to be plotted.
4. The file "plotting.ipynb" creates one sunburst chart and one bar chart to visualize the data based on the bank_statement_processed.csv file.
5. The directory "results" contains two files. First is an xlsx version of the bank_statement_processed.csv file created via "processing.ipynb". The second is a pdf file containing the three charts created via "plotting.ipynb".



If you want to execute the code yourself follow this guide:

1. Move the files "bank_statement.csv", "processing.ipynb" and "plotting.ipynb" to a new folder.
2. Open "processing.ipynb" with a code editor (I prefer jupyter notebook and would recommend it for data analysis). Execute the code from top to bottom. Answer the questions that pop up.
3. Check the folder for a results folder. It should contain an excel sheet. You can check the data in there.
4. Open "plotting.ipynb" with a code editor. Execute the code from top to bottom.
5. Check the results folder. It should contain a pdf file now. This pdf file contains both charts that visualize the given example bank statement data.




If you are familiar with python (in particular pandas) you can change things up a bit relatively easy:

1. You can add or change a few transaction lines to the "bank_statement.csv".
   If you add new descriptions you need to add them under: file: processing.ipynb -> block: "create categories, groups and searchterms" -> search_terms_expenses / search_terms_income
   
2. You can add new main- and subgroups or change up the order of them.
   You need to add/change them under: file: processing.ipynb -> block: "create categories, groups and searchterms" -> expenses_groups / income_groups.
   And also you need to add the maingroups and their color under: file: plotting.ipynb -> block: group and colors dict.
   
3. You can analyse your own bank_statement.csv. Therefore you can either replace the transaction lines of the example bank statement, edit the search terms, maingroups and subgroups and run the code as described.
   Or you read your bank statement with the processing.ipynb file and rename your columns to the ones used in the code (blueprint: file: processing.ipynb -> block: "initial setup of the df" -> rename columns). After that you need to edit the search terms, maingroups and subgroups and run the code as described.
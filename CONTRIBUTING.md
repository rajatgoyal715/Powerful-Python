To contribute to the project, please follow these steps:

1. Fork the repository.
2. Make changes to Notebook.ipynb file. 
3. Run the entire notebook (preferably block by block as it includes threading concepts).
4. Update Notebook.md file using the following command:
   ```jupyter nbconvert --to markdown Notebook.ipynb```
5. Add the updated content of Notebook.md file to README.md.
6. Run doctoc to update the table of contents by this command:
	```doctoc --github --maxlevel 2 README.md```
7. Push the changes to your repository.
8. Create a pull request.

# Import-Marvel

<strong>Powershell script and .CSV file that allows you to import Lord of the Rings characters as Users into Active Directory</strong>

<img src="https://media.giphy.com/media/g7SFZQGzS4HwQ/giphy.gif" width=900 />



<strong>Script:</strong>
1. Adds users into Active Directory
2. Adds users to appropriate groups based off of `LOTR_users.csv`.
3. Sets Service Prinipal Names (SPN)'s for user `gandalf`.


<strong>To run:</strong>
1. Download `./import_LOTR.ps1` and `LOTR_users.csv`.

2. Change domain name to match personal enviroment's domain.
 
**Note:** This will need to be done in both files. 	

-  Inside of `./import_LOTR.ps1`  on line: 59 & 76
	
-  Inside of `LOTR_users.csv` for each user in the 'ou' section

**Example:** `"CN=aragorn,DC=example,DC=com"` if desired domain is `example.com`
		
3. Change the path to which `LOTR_users.csv` is located on line: 6 for `./import_LOTR.ps1`.

4. Run `./import_LOTR.ps1`.



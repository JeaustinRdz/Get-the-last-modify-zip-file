# Get-the-last-modify-zip-file
Example to get the last zip file that was uploaded or modify in a blob storage


You can use the commands in Azure DevOps if you past it in a file.ps1 and use it in a powershell task as FilePath
![image](https://github.com/JeaustinRdz/Get-the-last-modify-zip-file/assets/163601125/af8288e0-9cea-4cae-8353-41fcdbe8097e)

Or copy and past it and use it as inline

For run the commands you required 2 variables

$storageAccountName that is the Storage Account name that is the file 

$sasToken that is the auth methot that I use, but you can changed as you required.

To get the sas token follow the next steps:

1- Go to Portal, to yout Storage Account and then to your container
2- Click in Shared access tokens
3- Add the permissions READ and LIST
4- Click in Generate Sas token and URL (You can modify the permissions and add an IP filter as you required based in your security)
![image](https://github.com/JeaustinRdz/Get-the-last-modify-zip-file/assets/163601125/dcd2886f-d456-48a3-8f32-4f2c66f9560f)


When you get the sasToken I suggest you add it as a variable in the pipeline and make sure to add it as variable type: secret

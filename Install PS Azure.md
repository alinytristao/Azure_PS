# Azure_PS

Install Azure PowerShell

From your computer, open an elevated PowerShell prompt.

Cmdlets for Service Manager (Classic) – also includes basic cmdlets such as subscription management

Run the Install-Module Azure command. This will install the Azure module which represents service management.

If you are notified that the repository is untrusted, confirm that you want to install the modules by typing Y and then pressing the Enter key.

Once the download and installation is finished, run the Import-Module Azure command.

Cmdlets for Resource Manager

Run the Install-Module AzureRM command. This will install the AzureRM module which represents resource management.

If you get prompted to install and import the NuGet provider, Type Y and then press the Enter key.

If you are notified that the repository is untrusted, confirm that you want to install the modules by typing Y and then pressing the Enter key.

The installation process will take several minutes as packages are downloaded and installed.

After the download and installation is finished, run the Import-Module AzureRM command.

Note: If you receive a message about running scripts on your computer has been disabled, temporarily change the execution policy:

Set-ExecutionPolicy Unrestricted

After the import command has completed, return the execution policy to restricted.

Set-ExecutionPolicy Restricted

Explore cmdlets and update the Help pages

To view storage cmdlets, run:

Get-Command *rmstorage*

to view syntax, description, and usage informatio for a command, run:

Get-Help New-AzureStorageAccount -full

If you have trouble installing the PowerShell modules from the PowerShell gallery, you can try the WebPI method instead. Visit http://aka.ms/webpi-azps to download and install the modules.

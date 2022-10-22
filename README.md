Ventura_Compatibility

This script is designed to be used as an Extension Attribute on Jamf Pro server to ensure specific requirements have been met to deploy macOS Ventura. 

**General Requirements:**

OS X 10.9.0 or later (It seems, as of the day I write this Apple has not yet made recommendations, this page and the script will be adapted if necessary when the information will become public)
4GB of memory (It seems, as of the day I write this Apple has not yet made recommendations, this page and the script will be adapted if necessary when the information will become public)
60GB of available storage, the required storage is different when upgrading from Catalina (33,5GB) or from older versions (44,5GB) and accounts for the size of the installer (almost 13GB)
These last 2 requirements can be modified in the first 2 variables (MINIMUMRAM and MINIMUMSPACE).
Creadit to Laurent Pertois

REQUIREDMINIMUMRAM: minimum RAM required, in GB
REQUIREDMINIMUMSPACE: minimum disk space available, in GB

**Exceptions**

The extension attribute will also display false for a computer that is compatible but already running Ventura.

**Installation**

Copy the content of the script (.sh file) to a new Computer Extension Attribute or just download the existing Extension Attribute (.xml) file and upload it to the Computer Extension Attributes of your Jamf Pro server.

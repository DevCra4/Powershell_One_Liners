# Powershell_One_Liners
This is my personal storage for the powershell commands I often for system administration. Hopefully you find them useful. 


Add-OnedriveAdmin

This is a function that solved what should have been a non-issue. When migrating to SharePoint utalizing the new Microsoft built in migration tools. It cannot (As of 7-15-21) detect other users OneDrive for buisness locations, even as a global administrator.
The function utalizes three cmdlets found in the SharePointOnline Powershell module. It works by connecting to SPO, listing all SharePoint sites, filtering that list to match the pattern located in OneDrive for Business URLs, and finally adding a user as a SiteCollectionAdmin to the matching sites.

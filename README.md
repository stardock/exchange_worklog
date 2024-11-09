# exchange_worklog
some solution tips for issues  

issue `“Object '<ServerName>' couldn't be found on '<DomainControllerName>'" error when trying to uninstall Exchange Server`  
Solution:  
\ \ `https://support.microsoft.com/en-au/topic/-object-servername-couldn-t-be-found-on-domaincontrollername-error-when-trying-to-uninstall-exchange-server-2dcfb94a-7f58-4a5e-8b59-d0ae12c63e1a`  

issue `the node is already a cluster member`  
solution:  
\ \ use `clear-clusternode clustername -force` to force clear the record  

issue `"Cannot convert null to type" error and Exchange 2019 CU14 RecoverServer fails`  
reason:  
\ \ This issue occurs because the value for a variable that's used in creating the virtual directory is not defined in Exchange Server 2019 CU14.   
solution:
\ \ `https://support.microsoft.com/en-us/topic/-cannot-convert-null-to-type-error-and-exchange-2019-cu14-recoverserver-fails-2f0e1202-8253-4bfc-a9bb-d575ccfa7cef`  



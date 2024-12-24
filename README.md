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

issue `recover exchange server`  
solution:  
  `https://learn.microsoft.com/zh-cn/exchange/high-availability/disaster-recovery/recover-exchange-servers?view=exchserver-2019`  

Exchange2019先决条件  
solution:  
  `https://learn.microsoft.com/zh-cn/exchange/plan-and-deploy/prerequisites?view=exchserver-2019`  

Recovering a Failed Exchange   
solution:  
  `https://practical365.com/recovering-a-failed-exchange-2016-database-availability-group-member/`  

iusse `Online - Data retrieval failures occurred`  
solution:  
  `https://blog.expta.com/2022/11/fix-for-online-data-retrieval-failures.html`  

issue `get wmrm details`
solution:  
  `https://learn.microsoft.com/en-us/archive/msdn-technet-forums/49c2a79c-0bc4-4dbd-8850-1e2615351495`  
  winrm get winrm/config  

reinstall:  
```
install cluster service and enable it
本地权限组
虚拟内存
```  

如何给shared mailbox添加Grantsendonbehalf:  
https://serverfault.com/questions/675223/how-to-give-send-on-behalf-permission-on-a-distribution-group-to-several-mailbox  
https://woshub.com/sendas-send-onbehalf-permissions-exchange/  
`Set-Mailbox secretary@woshub.com -GrantSendOnBehalfTo @{Add="jsmith@woshub.com"}`  

删除 运行 历史记录:  
`control folders`  

从pfx提取cert, key:  
https://www.ibm.com/docs/en/arl/9.7?topic=certification-extracting-certificate-keys-from-pfx-file  
`openssl pkcs12 -in [yourfile.pfx] -clcerts -nokeys -out [drlive.crt]`  
`openssl pkcs12 -in [yourfile.pfx] -nocerts -out [drlive.key]`  
You will be prompted to type the import password. Type the password that you used to protect your keypair when you created the .pfx file. You will be prompted again to provide a new password to protect the .key file that you are creating. Store the password to your key file in a secure place to avoid misuse.  
`openssl rsa -in [drlive.key] -out [drlive-decrypted.key]`  







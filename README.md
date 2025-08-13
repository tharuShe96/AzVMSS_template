# AzVMSS_template
Azure VMSS. Load balanced. running Nginx.

Azure Virtual Machine scale sets behind a Standard SKU Load balancer.

The Deployment_template is an ARM template. 

Pre-requisite - Have permissions to create resources. ie:Contributor role on the subscription or at resource group level.

Login to Azure portal > Create Resource Group > Custom Deployment > Build your own template in the editor > Load file/Copy paste code > Save >Review and Create
(Specify any changes required like resource group name. location, VMSS name, Admin username and password etc.)
(In case, if initial deployment fails for some resource, "Redeploy", and it will create the missing resources)

Estimated monthly Cost- Pay-as-you-go - 65aud

Assumptions:
-VM size chosen assuming the workload will just be running the nginx web page.
-Running for 730 hours
-Includes costs for public IP VmSS and load balancer(500GB data processed)

<img width="339" height="331" alt="Az-VMSS drawio" src="https://github.com/user-attachments/assets/31dd6e91-2094-4bae-a203-cab7d7e2e0af" />

Output:
Nginx welcome page displayed when the publicIP of the LB is queried    
  
<img width="339" height="331" alt="image" src="https://github.com/user-attachments/assets/a74cf120-8fab-497f-9fe5-c23480311a13" />

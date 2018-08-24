# Terraform-Templates

Terraform Templates to Deploy Infrastructure onto Azure
-------------------------------------------------------

PreRequisites:
-------------
 - Please see the section below pertaining to Credentials and Authentication

Credentials and Authentication:
------------------------------

  - An Azure Service Principal, with the proper role and permissions needs to be created prior to deploying
    workloads into Azure using terraform.
    ```
        See: https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-authenticate-service-principal-cli
    ```
  - Once the service principal has been created on Azure, edit the "Provider Info" section at the top of the "ENVIRONMENTNAME.tfvars" (file name could be anything
    but should end with .tfvars) with the following fields (pertaining to the service principal):

    ```
      # Provider info
        
        subscription_id = "<subscription_id>"
        client_id = "<client_id>"
        client_secret = "<secret used while creating the application>"
        tenant_id = "<tenant_id>"
      
    ```

Usage:
------

   run terraform: ```terraform apply```

 Support:
 --------

Feel free to fork this repository and use any or all of these templates, and to modify them in whatever way makes sense for your company. 

All feedback and suggestions (especially in the form of pull requests) are very appreciated. This is a work in progress that I hope will get better with more time and more contributors.

# Deploy a custom WordPress server to Azure

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fshidwalden%2FDeployWordpress%2Fmaster%2fazuredeploy.json" target="_blank">
    <img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fshidwalden%2FDeployWordpress%2Fmaster%2fazuredeploy.json" target="_blank">
    <img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.png"/>
</a>

This template deploys the following:
- Virtual Machine with your choice of size (limied to pre-selected ones) with VM Monitoring extentions
- Full LAMP Stack
- Public IP
- Network Security Group with ports 22 (SSH), 80 (HTTP) , and 443 (HTTPS) open
- a Resource Group of your choice (limited to specif regions)
- A VNet
- A DNS name using <vmname>.<region>.cloudapp.azure.com

Once the deployment is finished, you need to go to http://fqdn.of.your.vm/wordpress/ to finish the configuration, create an account, and get started with WordPress.
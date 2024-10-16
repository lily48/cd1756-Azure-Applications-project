# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

#### Compare Azure VM and Azure App Service
- Costs:
    * Azure VM: VMs can be more cost-effective for certain workloads, especially if we need to run multiple services on a single VM. However, costs can increase with the need for high availability and redundancy
    * Azure App Service: Typically more expensive than VMs for similar configurations.However, App Service can save on operational costs due to its managed nature
- Scalability
    * Azure VM: Requires manual setup for scaling, often using VM Scale Sets and load balancers. This can be complex and time-consuming
    * Azure App Service: Offers automatic scaling options that are fully managed by Azure that easily scale out by adjusting the number of instances via a slider in the Azure portal.
- Availability
    * Azure VM: High availability requires setting up multiple VMs and configuring load balancers. This setup can be complex and requires ongoing management
    * Azure App Service: Provides built-in high availability with automatic scaling and load balancing. This ensures your application remains available without manual intervention3
- Workflow
    * Azure VM: Offers full control over the environment, which is ideal for applications requiring specific configurations or legacy systems. However, this also means more responsibility for maintenance, updates, and security
    * Azure App Service: Simplifies deployment and management, allowing developers to focus on application codes. It integrates seamlessly with CI/CD pipelines and provides a streamlined workflow for web apps and APIs

#### Justify and selection
For deploying your Article CMS Flask Web Project, Azure App Service is generally the better choice due to its managed environment, ease of deployment, automatic scaling, and built-in high availability. This allows me to focus on development and deployment rather than infrastructure management.

### Assess app changes that would change your decision.
VM approach is more complex for the web solution for the use cases that my company has. I don't see any change from Azure App service to the VM in the future.

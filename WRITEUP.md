# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

-In this project I went with the App service solution (PaaS). This provide me with the conveninece of focusing on the development and not to worry about the hardware. App service support all the requirement I need for my project, as well as providing me with high availability and auto-scaling (both vertically and horizontaly) which will be suffecint for my article website. Also, app service allows me to use the dev/test environment for free, unlike the VM which I will have to to pay even for when I'm developing or debugging the code. Moreover, in app service microsoft enables me easly to use continuous deployment through github or any other git repo.

-Azure Virtual Machines has many features, as a IaaS, I will have full control of the virtual machine. VMs are far cheaper than buying and maintaining the hardware. I will be able to install any custom image and I will be able to install any software I need. If I build many VMs, I will have high availability, scalability, and redundancy. However, since they are more expensive than App service I will not be using them in this project as they require extra work and money while I don't need the power of VMs in my situation.

-As stated above, App service allows me to focus on the development, cheaper, and serves my needs. Therefore I went with this solution.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
I work as an AI Engineer, if I will deploy an AI solution I will need stronger computing power than what App service provide as a maximum of 14GB of memory and 4 vCPU cores per instance which doesn't serve my AI application.
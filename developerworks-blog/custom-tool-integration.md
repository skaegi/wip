#Introducing custom tool integration for Bluemix toolchains

As the development lead for Bluemix toolchain templates, I'm on the front line working with our technical sales and developer advocate teams regularly. Their goal is to develop new tool combinations to illustrate various DevOps practices and my goal is to make sure that toolchains meet those needs.

Toolchains come with out-of-the-box support for a number of common third-party tools like GitHub and Slack. Toolchains also support more specialized Bluemix tools, like Delivery Pipeline, that help deploy your applications. The list of out-of-the-box tools that toolchains support is growing rapidly. However, when we integrate directly with a customer's environment, we always find new or custom tools that we need to integrate that are not in the toolchain catalog.

We can go down the technical path and use the toolchain API to implement and contribute a tool broker, but we came up with a simpler approach that requires no coding or special hosting. If you only need to represent your tool visually on the toolchain and your initial tool integration needs are simple, the new custom tool integration is your best bet. The toolchain catalog includes a special catch-all integration called "Other Tool." 

I'll demonstrate the "Other Tool" option to add one of my favorite tools, OpenWhisk, to a toolchain.

Let's go to [Bluemix Devops](https://new-console.ng.bluemix.net/devops/). If this is your first visit, I recommend that you take a quick look at the [Toolchain Getting Started](https://console.ng.bluemix.net/docs/toolchains/toolchains_overview.html) documentation.  

Let's create an empty toolchain to try this out.

1. From the DevOps Toolchains page click **[+]**
1. Select the "Build your own toolchain" template. 
1. On the next screen,  ive your toolchain a clever name like "My OpenWhisk Toolchain" and click **Create**.
1. After your toolchain is created, add our custom tool by clicking **[+]** and select **Other Tool**.

Fill it in as follows:
![](OpenWhisk-CTI.png)


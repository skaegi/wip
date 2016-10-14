#Custom Tool Integration for Bluemix Toolchains

I'm the development lead for Toolchain Templates and in that capacity find myself on the front-lines working with our technical sales and developer advocate teams regularly. Their goal is to develop new combinations of tools that help illustrate various aspects of DevOps and mine is to make sure that Toolchains can be used to meet those needs.

Toolchains come with out-of-the-box support for a number of common 3rd party tools like GitHub and Slack as well as more specialized Bluemix tools that help deploy your applications like the Delivery Pipeline. The set of built-in tools directly supported by Toolchains is continuing to grow rapidly however especially when we integrate more directly with a customer's environment we always find the need to integrate with a tool that is not in the Toolchain catalog.

At this point one could go down the technical path and use the Toolchain API to implement and contribute a tool broker however there is a much easier approach that requires no coding or special hosting that should be considered first. If you just need to represent your tool visually on the toolchain and for the time being your tool integration needs are simple using a "Custom Tool" integration is going to be your best bet. The Toolchain catalog contains a special catch-all integration labeled "Other Tool". I'll use this to show we might add one of my favorite tools, "OpenWhisk" to a toolchain.

Let's go to [Bluemix Devops](https://new-console.ng.bluemix.net/devops/). If this is your first visit I'd recommend having a quick look at the excellent  [Toolchain Getting Started](https://console.ng.bluemix.net/docs/toolchains/toolchains_overview.html) documentation.

1. Let's create an empty toolchain to try this out. From the DevOps Toolchains page press [+] and then select the "Build your own toolchain" template. On the next screen  give your toolchain a clever name like "My OpenWhisk Toolchain" and press "Create"
2. Once your toolchain is created let's add our custom tool. Press [+] and select "Other Tool".

Fill it in as follows:
![](OpenWhisk-CTI.png)


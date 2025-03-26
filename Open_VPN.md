# OpenVPN – installation and set-up

## 1.	OpenVPN

When I visited the OpenVPN website, I was surprised to find that they offer multiple VPN solutions rather than a single product, adding another layer of decision-making. OpenVPN provides three distinct packages, each catering to different needs. Below, you’ll find a brief overview of these options.

### 1.1	 OpenVPN - Community Edition

If you are seeking a free, open-source option, the OpenVPN Community Edition is an excellent choice. It is a versatile and widely trusted VPN solution, popular among freelancers and organizations. However, while it provides robust features, setting it up and configuring it may require some technical expertise. You can download it for free and access documentation at **https://openvpn.net/community/**.

If you are strictly looking for free and open-source options, the OpenVPN Community Edition is the most suitable choice, though it does come with a steeper learning curve.

### 1.2	 OpenVPN – Access Server

For a more user-friendly experience while still leveraging the power of OpenVPN technology, consider the Access Server. It is designed for small teams or individuals and includes a free license for up to two simultaneous VPN connections. Access Server features an intuitive web-based admin interface and supports major operating systems like Windows, macOS, and Linux. This solution simplifies deployment while maintaining OpenVPN's robust security standards. Learn more at: **https://openvpn.net/access-server/**.

If you are a freelancer or remote worker with limited technical expertise, Access Server is an excellent option to consider. Its guided setup process and the availability of a free license for basic use make it a user-friendly choice for individuals. 

Since I was looking for a free and easy-to-use VPN, I will later introduce the Access Server solution step by step, showing how to download and configure it.

### 1.3	 OpenVPN – CloudConnexa

For a fully managed VPN experience, CloudConnexa offers a modern solution designed for effortless connectivity and remote access. It is an ideal choice for freelancers who want to avoid the complexities of setting up and managing a server. Although it is not free, CloudConnexa delivers an excellent out-of-the-box experience with minimal configuration required. You may explore this product at: **https://openvpn.net/cloud-connexa/**.

If you still have questions after reading the above descriptions and suggestions, I recommend visiting **[OpenVPN's product comparison page](https://openvpn.net/product-comparison/)** for more detailed information. Here, you can see the comparison of the products Access Server and CloudConnexa.

![](http://hdoc.csirt-tooling.org/uploads/upload_6ce1ea87ac5eddb0545872135ce6d0ae.png)

Further below, you can compare the two products based on the following categories by expanding the dropdown menus.

![](http://hdoc.csirt-tooling.org/uploads/upload_053292f155bf7f45368938fdfaa8ca0a.png)

## 2. OpenVPN – Access Server

In this chapter, I will guide you through the process of installing and configuring the OpenVPN Access Server solution, providing you with a free, feature-rich, reliable, and secure VPN for your computer.

Visit the **[Access Server website](https://openvpn.net/access-server/)** and click the "Get Access Server for Free" button.

![](http://hdoc.csirt-tooling.org/uploads/upload_73dd51ff30be40a042392519bc672973.png)

Next, either sign in if you already have an account or sign up by providing your work email and a password, or using your Google or Microsoft account.

![](http://hdoc.csirt-tooling.org/uploads/upload_48eaf8b55869aa300ddd1459594905ad.png)

Fill out the form and click 'Confirm' to proceed to the next screen.

![](http://hdoc.csirt-tooling.org/uploads/upload_bfac8f4bb6a016ef0f2675c45ced9912.png)

The next step will take you to the Access Server Portal screen, where you can decide whether to continue with the free version or subscribe to the service. In the lower-left corner, you see your email address, confirming that you are logged in. You can also access the functions on the left vertical bar, including the product's documentation.

![](http://hdoc.csirt-tooling.org/uploads/upload_4564b4e390a419a868da5ab5892a340e.png)

Let’s start with the Free Version. After you click the ’Try Free Version’ option, you will be directed to the Get Access Server screen. You have a vertical menu on the left, whereas you can check which cloud providers, containers and virtual machines are available. 

Also, at the bottom of the screen, you can find links to the release notes, technical documentation, and FAQs, and can also ask direct questions from Gary (Open VPN’s AI chatbot) by clicking on the speech bubble in the lower right-hand corner.

![](http://hdoc.csirt-tooling.org/uploads/upload_10a71d33cf56b5385a321d2d171442c6.png)

From the possible Cloud provider options, I chose Microsoft Azure.

![](http://hdoc.csirt-tooling.org/uploads/upload_0f16253faeab61fcddce405ed2134c1f.png)

Regardless of which cloud provider you choose the steps are very similar. On the next screen, you can watch a detailed step-by-step video on how to install the Access Server. I selected (for demonstration purposes) Microsoft Azure.  As shown on the right side of the screenshot below, you can also read a Start Guide on the process, but you can always ask for help via chat.

To get to the next step, click the ’Go To The Marketplace’ button at the bottom:

![](http://hdoc.csirt-tooling.org/uploads/upload_a00655b881431a2a2d8641187b98fffb.png)

On the Marketplace, you can read an overview of OpenVPN Access Server, check the plans and pricing section, or read reviews about the product. Once you gathered enough info, click the ’Get it Now’ button on the left (circled in red):

![](http://hdoc.csirt-tooling.org/uploads/upload_06b24ceee61c8ffa71454b8f6fc8c806.png)

You need to create an account by providing an email address and a password. From the screenshot below, you can see that even if you are on the free plan of OpenVPN, you should still pay for the Azure infrastructure costs:

![](http://hdoc.csirt-tooling.org/uploads/upload_f3e1d026df968337bfda7e69d61e8110.png)

On the next screen, the product (OpenVPN Access Server) and the button (Start with a pre-set configuration) are pre-selected, allowing you to proceed by clicking the 'Create' button in the center.

![](http://hdoc.csirt-tooling.org/uploads/upload_a7e5ee43fc664d646a07aed812465e80.png)

As stated above, you do not pay for OpenVPN itself, still, you need to pay for using Microsoft Azure infrastructure fee. I got the below offer:

![](http://hdoc.csirt-tooling.org/uploads/upload_737ddd4bd1548a907db70b49160b1742.png)

The pricing is the same with all the other options (Amazon AWS, Google Cloud, Digital Ocean, or Oracle Cloud): while the VPN itself is free, you will need to cover the infrastructure costs of the cloud provider. To optimize costs, consider contacting the cloud providers directly to negotiate pricing if you plan to use OpenVPN.

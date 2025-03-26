# Tailscale: how to create a peer-to-peer VPN connection?

Tailscale is a great tool for creating a peer-to-peer VPN connection, especially for freelancers who need a secure and simple way to connect with others. It is based on WireGuard and offers a zero-configuration approach to setting up a VPN, making it easy for people to work together securely without needing advanced networking knowledge.

## 1. A short description of how to set up Tailscale

Here is how you can set up a peer-to-peer VPN connection with other freelancers using Tailscale:

### 1.1. Sign up for Tailscale

* Go to the **[Tailscale](https://tailscale.com/)** website and sign up for a free account (or a paid one if you need additional features).
* You can sign up using Google, GitHub, or another method of your choice.

### 1.2. Install Tailscale

* Install Tailscale on your device (laptop, desktop, etc.) by downloading the app from the website. Tailscale is available on multiple platforms like Windows, macOS, Linux, iOS, and Android.
* Follow the installation instructions based on your operating system.

### 1.3. Log in and create a network

* Once installed, open the Tailscale app and log in using the account you just created.
* When you first log in, you will be asked to create a network. This is where you will connect with your peers (other freelancers).

### 1.4. Invite your freelancer peers

* To invite others to your network, you need to send them an invitation.
* Open the Tailscale admin panel (on the Tailscale web portal) and invite other freelancers by sharing a link or adding their email addresses.
* Your peers will receive an invite to join your network, and they will need to install Tailscale on their devices and log in to accept the invitation.

### 1.5. Connect to your peers

* Once your peers have joined the network, you can see their devices in your Tailscale admin panel, and they will appear on your Tailscale app as well.
* You can easily establish a peer-to-peer connection by selecting their device from the Tailscale interface.

### 1.6. Secure communication

* With Tailscale, you will automatically be using end-to-end encryption for all data shared between connected devices.
* The connection is direct (peer-to-peer) unless there is a network issue, in which case Tailscale will use its relay servers to ensure the connection remains intact.

### 1.7. Set permissions (optional step)

* You can set granular access controls if you do not want everyone to have access to everything. For example, you might want to give only certain peers access to specific files or services.
* You can manage permissions from the Tailscale admin console.

### 1.8. Use Tailscale for file sharing and collaboration

* Now that you are connected, you can securely share files, access each other’s machines (if permission is granted), and collaborate just like you are on the same local network.
* You can even run internal services or use remote desktops as if you were in the same physical office.

### 1.9. Mobile access (optional step)

* Tailscale also works on mobile devices. This can be particularly useful if you are collaborating with freelancers on the go. Once logged in on mobile, you can connect securely to your peers no matter where you are.
 
## 2. Step-by-step guide to set up Tailscale

### 2.1. Sign up for Tailscale

First, you need to sign up for Tailscale. You have several options to choose from (please check the screenshot below). I chose to register with my GitHub account, so the following screenshots show the process accordingly.

![](http://hdoc.csirt-tooling.org/uploads/upload_7bc54c5844d95d3ca52dbcf48cae22db.png)

### 2.2. Add your device

Once authenticated, you will be directed to the Tailscale portal, where you can add your first device to your Tailscale network. Your email address will be displayed in the top-left corner, while your avatar will appear in the top-right corner.

![](http://hdoc.csirt-tooling.org/uploads/upload_390dd3bf95e0fdf37e028b3bc9043318.png)

### 2.3. Download the app

After adding your device to your Tailscale network, you should download the Tailscale application. You can choose from several different operating systems. For this demonstration, I chose 'Tailscale for Windows,' and the following screenshots will guide you through this process.

![](http://hdoc.csirt-tooling.org/uploads/upload_a273a3dc65136b77a9d449f890e1e7ba.png)

You can easily see the process on your screen, and once it is finished you need to run the .exe file.

![](http://hdoc.csirt-tooling.org/uploads/upload_1f748b5e3f1d8fe370f252f01d0ed1f3.png)

In the popup window, please check the checkbox and click ‘install’.

![](http://hdoc.csirt-tooling.org/uploads/upload_f608f034eae71dd4389dfb6d212558f5.png)

Again, the progress of the setup process can be followed easily:

![](http://hdoc.csirt-tooling.org/uploads/upload_4b223d79034c9093fa1f287bf7ba279a.png)

Once the installation is complete, you will be greeted with the 'Installation Successfully Completed' message.

![](http://hdoc.csirt-tooling.org/uploads/upload_a825f3ff4f2720d0137ea826bc5df2ef.png)

### 2.4. Sign in and connect your device

Now, you can sign in and connect your device to your Tailscale network:

![](http://hdoc.csirt-tooling.org/uploads/upload_be4bf11dcd3a9e032aeb7167a0c2feae.png)

To do that, you need to log in again to be able to connect your device to the Tailscale network:

![](http://hdoc.csirt-tooling.org/uploads/upload_a27dd0bfeff38f5e293e1f922f68cf33.png)

Once you log in to the application of your choice, the next step is you authorize Tailscale to access your account (in the example below, Tailscale wants to get access to my GitHub account). 

![](http://hdoc.csirt-tooling.org/uploads/upload_1c3bd51fed41b4e5742194c3105a4ae6.png)

To authorize Tailscale to get access to your account, click the ‘Authorize Tailscale’ button.

![](http://hdoc.csirt-tooling.org/uploads/upload_74b1cf5e11f2e83e3e835a391d67debf.png)

Tailscale adds your device to Tailnet and offers you that you can add a second device (if you want to).

![](http://hdoc.csirt-tooling.org/uploads/upload_938175545bf439788b8dee2dc2bfc867.png)

### 2.5. Log in to the Tailscale portal

Now you can see the Tailscale portal and can manage your apps, services, users, and many more. You can add additional devices by clicking on the ‘Add device’ button.

![](http://hdoc.csirt-tooling.org/uploads/upload_b819e3349aba203b8262a084f7a8004b.png)

By clicking on the three-dot-icon (circled in the screenshot below), you can share your Tailnet with one of your freelancers creating a peer-to-peer connection:

![](http://hdoc.csirt-tooling.org/uploads/upload_1b74ca38d60c851e1ab9fbfd705dec89.png)

Chose the option ‘Share…’ from the dropdown menu

![](http://hdoc.csirt-tooling.org/uploads/upload_a06ed3157034f7eef141240ae9630006.png)

and share access to your machine via email (you can send an invite to an email address or copy the share link and share the link in a separate email). In case you want to share access to your machine with several peers, put their email addresses in the field and separate the email addresses with commas.

![](http://hdoc.csirt-tooling.org/uploads/upload_fe69b29ee6b6dca1e7fd9dbe41627b8b.png)

### 2.6. Invite others to your network

You can also invite users by generating an invite link to share with them if you click the ‘Users’ tab in the Tailscale console and click the ‘Invite external users’ button:

![](http://hdoc.csirt-tooling.org/uploads/upload_faf818bab72fe7682dd9c06b2b880d93.png)


## 3. Summary

By using Tailscale, you can create a secure, encrypted, and straightforward connection with your freelancer peers, making remote collaboration much easier and safer.
Key Features for Freelancers:

* **Zero configuration**: Tailscale handles all the complexity of VPN, so you do not have to worry about complicated network setups.
* **Peer-to-peer**: Tailscale prioritizes direct peer-to-peer connections, which improves both speed and security.
* **Private network**: Your network is private, so only those you invite can join.
* **Cross-platform**: Works across Windows, macOS, Linux, Android, and iOS, which is useful when working with different devices.
* **No central server**: Tailscale does not route your traffic through a central server. The traffic is encrypted end-to-end between devices.


# WireGuard VPN – installation and set-up

## 1. WireGuard VPN

WireGuard is a modern, open-source VPN designed for speed, simplicity, and strong security. With a lightweight design and state-of-the-art encryption, it delivers faster connections and enhanced privacy compared to traditional VPNs. Its user-friendly setup makes it ideal for freelancers and remote workers seeking an efficient way to protect their online activity.

## 2. Installation

Go to the WireGuard homepage and click the 'Installation' link in the top menu bar. Choose the operation system you use on your machine and click the relevant ‘Download’ button. Since I have a Windows machine, I will show the steps by using the ‘Download Windows Installer’ option.

![](http://hdoc.csirt-tooling.org/uploads/upload_e97194f61cd3a9f6f8346d544ca6eced.png)

Click the download icon and run the application by selecting its name.

![](http://hdoc.csirt-tooling.org/uploads/upload_f2d5614f597c544a43caf85a0a9eabbe.png)

The Windows Installer starts the process and prepares the installation:

![](http://hdoc.csirt-tooling.org/uploads/upload_9478e8afb35f1652a72dbce9f4e11397.png)

During the installation of WireGuard on a Windows machine, you’ll need to create a tunnel to establish a VPN connection. 

![](http://hdoc.csirt-tooling.org/uploads/upload_849330dd507ffde524ffe32be5dc6699.png)

Click the down-pointing arrow next to the ‘Add Tunnel’ and choose either to import a tunnel from a file or add an empty tunnel.

![](http://hdoc.csirt-tooling.org/uploads/upload_643e123a7cae95d236b2bdc78434e567.png)

If you choose to add an empty tunnel, you need to manually set up your tunnel: enter your public/private key and other necessary information).

![](http://hdoc.csirt-tooling.org/uploads/upload_78591ed4f7983309b2402f3ec05d10dd.png)

Give a name to your tunnel and click ‘Save.’ The interface changes and you can see that the tunnel named ‘Test’ is still inactive. Click ‘Activate’ to make it active.

![](http://hdoc.csirt-tooling.org/uploads/upload_ed4a614e5ecbce41f1f9537255c1f672.png)

The status of the tunnel changes to ‘Active’:

![](http://hdoc.csirt-tooling.org/uploads/upload_8515e58f2a70f21929c302273ac16e76.png)

You can deactivate the tunnel by clicking on the ‘Deactivate’ utton. You can also remove (delete) the tunnel by clicking the red ‘X’ in the lower left corner. You can also check the logs if needed (click the ‘Log’ tab highlighted in yellow in the screenshot below).

![](http://hdoc.csirt-tooling.org/uploads/upload_a51d577c75543b3f5668d468e57b784e.png)

## 3.	Step-by-step installation guide

Here's a step-by-step guide for setting up WireGuard VPN on a Windows machine, using either a pre-configured configuration file or creating a tunnel from scratch:

### Step 1: Install WireGuard

1.	Download and install WireGuard for Windows from the official website.

2.	Run the installer and follow the on-screen instructions.

### Step 2: Create or Import a Tunnel

You have two main options here: create a tunnel from scratch or import a pre-configured file.

#### Option 1: Importing a Pre-Configured Tunnel (Recommended for beginners)

**1.	Obtain the Configuration File:**

* If you are using a third-party VPN provider (like Mullvad or IVPN), log into their site, generate the WireGuard configuration, and download the .conf file.
* Alternatively, if you are setting up your own WireGuard server, generate the configuration file (.conf) containing the server’s public key, endpoint, and other relevant settings.

**2.	Import the Configuration File:**

* Open the WireGuard app.
* Click on "Add Tunnel" > "Import from File".
* Browse to the .conf file you downloaded or created and open it.

This will automatically populate the necessary fields like the Private Key and Server Endpoint.

**3.	Activate the Tunnel:**

* Once the configuration is imported, you will see the tunnel listed on the main screen.
* To activate, click the Activate button on the tunnel you just created.
* Your VPN connection will be established.


#### Option 2: Creating a Tunnel from Scratch (Advanced)

**1.	Generate Keys:**

* You need to generate a Private Key and a Public Key for both the server and client.
* On Windows, you can use the WireGuard command line tool or a third-party generator.
* To generate keys, you can run the following commands in a terminal or use the WireGuard application to generate them:
bash
CopyEdit
wg genkey | tee privatekey | wg pubkey > publickey
* Save the output in two files (e.g., privatekey and publickey).

**2.	Create a New Tunnel:**

* Open WireGuard.
* Click "Add Tunnel" > "Create from Scratch".
* Enter a Name for the tunnel (e.g., "MyWireGuardVPN").

**3.	Configure the Tunnel:**

In the [Interface] section, add your PrivateKey:
ini
CopyEdit
PrivateKey = <your private key>
Address = 10.0.0.2/24  # Choose a local IP address for your device

* In the [Peer] section, add the server’s details:
    
ini
CopyEdit
[Peer]
PublicKey = <server public key>
AllowedIPs = 0.0.0.0/0  # Route all traffic through the VPN
Endpoint = <server IP>:<port>

**4.	Save and Activate the Tunnel:**

* Click Save to store the tunnel.
* Then, click Activate to start the VPN connection.

### Step 3: Verify the Connection

1. To verify your connection, you can check the status in the WireGuard app.
1. Additionally, you can go to a website like whatismyip.com to check if your IP has changed, confirming that your VPN is active.

### Step 4: Disconnect the VPN

To disconnect, simply go back to the WireGuard app and click ‘Deactivate’ on the active tunnel. This setup should cover most cases for both importing and manually creating a tunnel. 




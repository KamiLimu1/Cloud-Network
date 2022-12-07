# CLOUD NETWORKING 101

- Access the IIS server and host a simple website on the server


## PROCEDURES FOR CONFIGURATION
 
 We were able to access the server with RDP for Windows Operating system.
 Remmina for Linux Operating System.

### Install IIS(For Windows Users)
- From the Windows start menu, open Server Manager.
- Click Add roles and features.
- Select Role-based or feature-based installation, and choose your server.

 ![Role Services](https://github.com/Emmanuel-9/Cloud101/blob/master/Images/IIS%20iNSTALLATIONS.png)

- Scroll through Server Roles and click Web Server (IIS).
- Add any additional IIS features you wish to install.
- Click Install to start the installation process.

![Installation](https://github.com/Emmanuel-9/Cloud101/blob/master/Images/IIS%20Installation%20Progress.png)


![Installed Roles ](https://github.com/Emmanuel-9/Cloud101/blob/master/Images/Roles%20and%20Servers.png)


### Create the web application
- Using Windows Explorer, create a new folder in the default IIS web server directory to store your domain's web files. For example, you could create a folder named ` C:\kamilimu\example.com `

![Installation](https://github.com/Emmanuel-9/Cloud101/blob/master/Images/IIS%20Site%20Configuration.png)


### Setup the IIS Site with your Domain Name
- Open the Windows start menu and navigate to the Windows Administrative Tools subgroup.
- Select Internet Information Services (IIS) Manager from the list.
- In the IIS Manager Window, click ` > ` next to your server name to expand the list.
- Expand Sites, and click Add Website on the right Actions bar.
- Enter your Web Application name in the Site Name: field.
- Under Content Directory, click ` ... ` to browse and set the Physical path: to your domain web files directory.
- Keep ` http ` as the Type under Binding, and ` 80 ` as the port.
- To assign your domain a specific IP address, select it from the drop-down list, or keep All Unassigned to use all Server IP addresses.
- Enter your domain name in the ` Hostname: ` field.
- Click OK to save changes and automatically start the website.
- Visit your domain to confirm successful integration.


![Installation](https://github.com/Emmanuel-9/Cloud101/blob/master/Images/Domain%20Setting.png)
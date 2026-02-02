<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket - Prerequisites and Installation

This project demonstrates hands-on experience with web server and application management, including full installation and configuration of web platform components and Microsoft Visual C++ Redistributables. It covers MySQL database setup and security, deployment and configuration of the osTicket web application with required PHP extensions, and file permission management to ensure operational readiness. The project reflects real enterprise IT responsibilities, including web server configuration, application deployment, and secure management of system and database resources.

## Environments and Technologies Used

- **Windows 10 (21H2)**
- **Internet Information Services (IIS)**


## Skills Demonstrated

- Enabling and configuring Internet Information Services (IIS)
- Installing and managing web platform components (PHP Manager, URL Rewrite)
- Installing and configuring Microsoft Visual C++ Redistributables
- Database installation, configuration, and security management using MySQL
- Deploying and configuring web applications (osTicket) with required PHP extensions
- Managing file permissions and completing web-based application setup


## Tasks for this project

### 1. Enable Internet Information Services (IIS) and Required Features
Access **Control Panel** via the Windows search bar and navigate to:
**Programs** → **Turn Windows features on or off** → **Internet Information Services (IIS)**.
Under **Web Management Tools**, ensure **IIS Management Console** is selected.
Under **World Wide Web Services** → **Application Development Features**, enable **CGI** and **Common HTTP Features**.

![Screenshot](https://github.com/alexandrpaul/ost-pni/blob/9a9a2903f2c890fe6c027e06c4e96336ff088927/Screenshots/img1.png)



### 2. Install Web Platform Components for IIS
Install the Web Platform Installer along with the following dependencies:
  - PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)
  - URL Rewrite Module (rewrite_amd64_en-US.msi)
  - PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip)

![Screenshot](https://github.com/alexandrpaul/ost-pni/blob/9a9a2903f2c890fe6c027e06c4e96336ff088927/Screenshots/img2.png)



![Screenshot](https://github.com/alexandrpaul/ost-pni/blob/9a9a2903f2c890fe6c027e06c4e96336ff088927/Screenshots/img3.png)



### 3. Install the Microsoft Visual C++ 2015–2022 Redistributable package

![Screenshot](https://github.com/alexandrpaul/ost-pni/blob/9a9a2903f2c890fe6c027e06c4e96336ff088927/Screenshots/img4.png)



### 4. MySQL Installation and Configuration
Install MySQL using the Typical Setup option and complete the **Standard Configuration** process.
Configure and secure the instance by assigning a root password.

![Screenshot](https://github.com/alexandrpaul/ost-pni/blob/9a9a2903f2c890fe6c027e06c4e96336ff088927/Screenshots/img5.png)



![Screenshot](https://github.com/alexandrpaul/ost-pni/blob/9a9a2903f2c890fe6c027e06c4e96336ff088927/Screenshots/img6.png)



### 5. Install and Configure osTicket
Install osTicket and enable the following PHP extensions: **php_imap.dll**, **php_intl.dll**, and **php_opcache.dll**.

  - Navigate to ost-config.php located at:
    **C:\inetpub\wwwroot\osTicket\include\ost-config.php**
    and configure its permissions for **Everyone**.

Proceed with the **osTicket** setup via a web browser. Once configuration is complete, click **Install Now** to finalize the installation.

![Screenshot](https://github.com/alexandrpaul/ost-pni/blob/9a9a2903f2c890fe6c027e06c4e96336ff088927/Screenshots/img7.png)



<h2> Final Thoughts </h2>

<p> Completing this implementation provided hands-on experience managing a Windows-based web application stack in a controlled environment. The work reinforced practical skills in IIS configuration, dependency and runtime management, database setup and security, and application deployment using industry-standard tools. Configuring PHP extensions, managing file permissions, and completing web-based installation workflows emphasized attention to detail and operational readiness. Overall, the experience strengthened foundational skills in web server administration and application support, directly aligning with real-world enterprise IT and help desk responsibilities. </p>

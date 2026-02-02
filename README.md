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

Proceed with the osTicket setup via a web browser. Once configuration is complete, click **Install Now** to finalize the installation.



![Screenshot](https://github.com/alexandrpaul/ost-pni/blob/9a9a2903f2c890fe6c027e06c4e96336ff088927/Screenshots/img7.png)

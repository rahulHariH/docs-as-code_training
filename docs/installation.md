# Installing BMC Defender Server

This topic provides a quick guide to install the _BMC AMI Command Center for Security_ product (also known as the _BMC Defender Server_) on a Microsoft Windows platform.

You can use the installation package to install at a new site or upgrade an existing site to the latest version. If you are upgrading, see the [Upgrading](upgrading.md) section for information about the different options.


## Before you begin

Before you begin the installation process, ensure the following:

 - Close all windows and disable any port blocking or virus scan software on the system.
 - Download the installation files from the [BMC Electronic Product Download website](https://www.bmc.com/). Your ability to access product pages on the EPD website depends on the license entitlements purchased by your company.
 - Apply and configure the installation requirements for BMC Defender Server, including the antivirus considerations.
 - Exclude the BMC Defender Server folders from on-access virus scans.
   > [!WARNING]
   > On-access virus scans can seriously degrade BMC Defender Server operations. The operation of the server relies heavily on fast disk access to store log data.

## To install the BMC Defender Server

1. Log on to the target Windows platform with an administrator type login.
1. Download the relevant self-extracting file from the EPD website:
   - **BMC AMI Command Center for Security Version 6.2.00** (the downloaded file name is BMC-AMI-Command-Center-for-Security-6.2.00.bbbb.exe)
   - **BMC Defender SIEM Correlation Server Version 6.2.00** (the downloaded file name is BMC-Defender-SIEM-Correlation-Server-6.2.00.bbbb.exe)
1. Execute the self-extracting file to the target directory. Select a target directory (by default, **C:\Program Files\BMC Software\BMC Defender** and click **Next**.
   > [!IMPORTANT]
   > If you see a warning for a missing **mfc140.dll** file, go to the Microsoft website. Download and install the redistribution package for Visual Studio 2015 (**vc_redist.x86**).
1. Follow the wizard prompts. You can usually use all defaults during the installation.
   1. On the BMC Defender Installer Program page, review the content and select Click, if you agree to the terms of the software license. Click Next.
   1. On the Configure Apache HTTP Server page, enter a service port number for HTTP and HTTPS. You can use the default values of 80 for HTTP and 443 for HTTPS. Click Next.
   2. On the Enter Site Certificate Information page, enter certificate information or use the defaults. Click Next.
On the Ready To Begin Installation page, you can select to Overwrite Existing SSL/TLS Certificate Information. Click Next to start the installation.
On the Installation Complete page, the URL and default user name and password are displayed. Note these values and click Finish.
When the installation process finishes, the CO-syslog.exe program is running on the platform, awaiting messages.

During the installation process, detected errors stop progress of the installation and an error dialog indicates the cause of failure.

No other steps are needed to install the program. BMC Defender does not require you to reboot the server after installation. Review all previous notices for SPEs and patches. See Notices.
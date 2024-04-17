### UiPath RPA Challenge
# Invoice Extraction with OCR

[![GitHub](https://badgen.net/badge/icon/GitHub?icon=github&color=black&label)](https://github.com/MaxineXiong)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform - UiPath RPA](https://img.shields.io/badge/Platform-UiPath_RPA-fa4616)](https://www.uipath.com)

<br/>

This repository hosts an [UiPath](https://www.uipath.com/) automation solution designed to address the [RPA challenge of Invoice Extraction](https://rpachallengeocr.azurewebsites.net/) outlined in the requirements below.

### **Instructions**

1. The goal of this challenge is to create a workflow that will read every table row and download the respective invoices.
2. From the invoices, you will have to extract the **Invoice Number, Invoice Date, Company Name and Total Due** through **Optical Character Recognition (OCR)**.
3. You will have to build and upload a CSV file with the data extracted from each invoice, the ID and Due Date from the table, **only for the invoices for which the Due Date has passed or is today**.
4. The actual countdown of the challenge will begin once you click the **Start** button and will end once the CSV file is uploaded; until then, you may play around with the table on the right without receiving penalties.
5. Below is the snapshot of an example CSV file in order to see the required format for the end result and two sample invoices. The formats of the invoices will be exactly as in the samples and they will not change. **The challenge
   expects the uploaded CSV to be in the exact same format as the example CSV, including the formatting of the cells, and the rows should be in the same order as they appear in the table. Any difference will result in a failed challenge.**


![image](https://github.com/MaxineXiong/Invoice-Extraction-OCR-Challenge-RPA/assets/55864839/06d96162-f67e-418c-b033-6fc11252daa7)


_You can check out the **automation demo video for the solution** below_:

https://github.com/MaxineXiong/Invoice-Extraction-OCR-Challenge-RPA/assets/55864839/e9a608c4-1e0d-415d-a303-bd431ec71daf


<br/>

*Please note that as of 12 April 2024, the server for rpachallenge.com seems neglected and unable to score the output results. It will consistently 
display a failed status in the end, regardless of whether the uploaded CSV file matches the correct result. Please disregard the challenge website's score rating for your uploads.*


<br/>


## **Installation**

Before installing **UiPath Softwares**, please make sure your system meets the hardware and software requirements outlined in the **[UiPath documentation](https://docs.uipath.com/studio/standalone/2022.10/user-guide/hardware-and-software-requirements)**.

The **Uipath Platform** includes the following tools:

- **UiPath Studio**
- **UiPath Assistant**
- **UiPath Automation Cloud, including UiPath Orchestrator**

<details>  
<summary> To run this project successfully, please follow these steps to install UiPath Studio:
</summary>

***

Step 1 : Visit [uipath.com](https://www.uipath.com/) and click **Try UiPath Free** button.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_1.png">
</p>

Step 2: **Sign up** for a personal account.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_2.png">
</p>  

Step 3: **Verify** your account in email.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_3.png">
</p>  

Step 4: **Log into** the **UiPath Automation Cloud** using your account, and click the **Download Uipath Studio** button.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_4.png">
</p>   

Step 5: Click **Sign in**.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_5.png">
</p>    

Step 6: Select **UiPath Studio Pro**.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_6.png">
</p>  

Step 7: Follow the system instructions to complete the installation of **UiPath Studio Pro**.
<p align="center">
<img width="900" src="https://github.com/YenLinWu/RPA_UiPath/blob/master/Installation/README_Images/Install_UiPath_Studio_7.png">
</p> 

</details> 

<details>  
<summary> Please also follow these steps below to connect your local machine to the UiPath Automation Cloud for deploying this workflow (if desired):
</summary>

***

Step 1: Sign up and log into [UiPath Automation Cloud](https://cloud.uipath.com/).

Step 2: Add a **Tenant**.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/a8c8e306-afc5-46bf-bae7-a6b2a06a6d1b">
</p>

Step 3: **Edit** the user and assign the **Automation Users** role to grant them permission to execute processes.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/3ab0a0cb-14d4-47d9-a6c6-6983ad5b966b">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/04c68432-f3c6-4f84-b477-2ace8a2d859c">
</p>

Step 4: Go to the **Orchestrator** interface and click on **Tenant** in the left pane.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/d3ace46c-7e98-4a41-a5a8-d2347be85c47">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/0e248abb-93cb-4480-a548-a955b168bb92">
</p>

Choose **Folders** and then click the **+** icon to create a new folder.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/1523c9ba-86d9-4ebd-bf4d-54d2fbcf305b">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/337937fc-f4c1-4e8f-ae3a-631e57349d9e">
</p>

Step 5: Navigate back to **Tenant** interface and follow the steps below to start adding an Automation User for Unattended Robot in **Manage Access**.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/a0fc74fa-8c5a-4584-abd0-2d708ea6f468">
</p>

a) Scroll down to locate the target user, then assign the **Automation User** role to grant them the necessary permissions. Click **Next** button to move on to the next page.   
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/6e5c95e4-a9dd-4b95-8509-f0434f323cdf">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/6ac2c4ab-98e8-488b-82c1-e8959dfc5e29">
</p>

b)  In the *Personal automations setup* page, select the options to **Enable user to run automations** and **Create a personal workspace for this user and enable optimal Studio Web experience**, then click on the **Next** button.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/53761113-4175-4558-b02e-78f4bd039b04">
</p>

c) On the *Unattended setup* page, check the option to **Enable this user to run unattended automations**, choose **Specific Windows credentials** for local machine connection to Orchestrator, provide **Domain\Username** of your user account on local machine (which can be found by executing `whoami` in Command Prompt), and enter the **Password** for accessing your local machine. Finally, click on the **Update** button.

<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/94e0f224-e466-4670-b981-4714cd48a02c">
</p>

Step 6: Now, go to the **Machines** page where you should see the workspace machine for the target user already created. Click the ellipsis to select **Edit Machine**.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/17f0363b-ee02-4e64-a4ef-7c6ae23b5b45">
</p>

Enter **1** for both the *Production (Unattended)* and *Testing* fields, then click the **Update** button.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/29ebf986-e7b9-4429-9976-4c0e5ed5d37e">
</p>

Step 7: Now return to the newly created folder, choose the **Machines** menu, and click **Manage Machines in Folder** button to assign the machine you just configured to the folder.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/9587d8d7-b07f-41ba-adc3-f0af6d44893b">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/f83c9899-8f4e-4360-aaae-0d546f731dbc">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/d4e2b0c0-11dd-47b4-adfe-c8ceeb2a2b04">
</p>

You should now have both the **User** and **Machine** assigned to the new folder.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/a82ee8b6-6975-404e-a0c2-91e3da9f70d9">
</p>

Step 8: Open **UiPath Assistant** and click **Sign In**. If you see the **green circle** in the top right corner, you’ve successfully connected your local *UiPath Studio* to the *UiPath Automation Cloud*.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/10ba5c72-cef7-4821-80a9-d02428c09362">
</p>
You can confirm the connection by opening UiPath Studio and checking for a green circle at the bottom.
<p align="center">
<img width="600" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/10bfea30-4871-49cc-b038-13d05ae5b09b">
</p>

***

To **publish a process** from UiPath Studio to Orchestrator, **switch to the new folder** you just created in the Orchestrator, and then click to **Publish the process** as a package.
<p align="center">
<img width="900" src="https://github.com/MaxineXiong/Data-Migration-Into-CRM-Apps-RPA/assets/55864839/c591ee81-f7d4-4dba-9b8a-57e4a2c0148d">
</p>

To learn more about other best practices on Orchestrator, please refer to the [Orchestrator User Guide](https://docs.uipath.com/orchestrator/standalone/2023.4/user-guide/introduction).

</details> 


<br/>

## **Usage**

To run the RPA workflow on your local machine, follow these steps:

1. Either **download** this repository to your local machine or **clone** it directly within your UiPath Studio.
2. Open the **UiPath Studio** software on your machine.
3. Locate and **open** the **Main.xaml** file from the downloaded repository in **UiPath Studio**.
4. **Run** the **Main.xaml** file to start the RPA process.

<br/>

## **Acknowledgement**

I would like to express my gratitude to the **[UiPath community](https://community.uipath.com/)** for providing resources, tutorials, and a platform for automation enthusiasts to learn and collaborate.

<br/>

## **License**

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/), which means you're free to modify, distribute, and use the code in your own projects.

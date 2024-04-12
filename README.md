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

*Please note that as of 12 April 2024, the server for rpachallenge.com has been deprecated and is unable to score the output results. It will consistently 
display a failed status in the end, regardless of whether the uploaded CSV file matches the correct result. Please disregard the challenge website's score rating for your uploads.*


<br/>


## **Installation**

Before installing **UiPath Softwares**, please make sure your system meets the hardware and software requirements outlined in the **[UiPath documentation](https://docs.uipath.com/studio/standalone/2022.10/user-guide/hardware-and-software-requirements)**.

The **Uipath Platform** includes the following tools:

- **UiPath Studio**
- **UiPath Robot**
- **UiPath Orchestrator**

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

# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop




<img width="440" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/e9a54ac9-a7d1-4197-8966-f1233f3ba897">






2.	Install java1.8 in folder /usr/local



<img width="446" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/4fa14b17-cc86-49b5-902f-04034afd115d">






3.	Install Hadoop




<img width="447" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/6b0b44a9-03cc-4242-ae77-763e8e2426f6">






4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file




<img width="479" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/9d770881-9ff9-46a6-a71f-8ec6e5d1bf02">






 
5.	Set hadoop environment variables: Include the following lines /etc/profile file




<img width="475" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/fd31bae2-7569-4e41-b7ea-e07d5ddd86b0">







6.	Run the.bashrc & profile files from the $ prompt for updating the changes

<img width="477" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/b2e9df9e-ed35-4595-afc3-6ef8743a79c8">




<img width="559" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/5de4db99-9947-4725-88bc-8b723aedf20d">





7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file



<img width="462" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/317948b5-f245-47f2-9480-bfcbb52bd818">






b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)




<img width="460" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/39072af6-33b5-4a63-a49b-7e81dcb70b98">



 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags




<img width="450" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/65c1f822-c76f-4546-8662-f6c713dba246">






c)	mapred-site.xml


 <img width="452" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/c2c391c9-dbab-4c8c-8008-d758519c548f">


Include the following lines in mapred-site.xml file



<img width="460" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/3d759eba-1bf3-4fa2-a899-7a4423aeb94a">



 

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file



<img width="519" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/026d72ed-39ef-443d-a265-24f4297c0aac">






e)	yarn-site.xml
Include the following lines in yarn-site.xml file



<img width="441" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/5bb2be68-c58f-4955-b5eb-997ed0cca9a6">





8.	Format the Hadoop File system implemented on top of the local file system using


<img width="459" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/3b4691b4-47be-4cd1-b262-967c3d1cfd0c">




9.	Start Hadoop using


<img width="583" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/cfe2f313-4783-439d-ac78-12f6e8e9814a">





10.	The commonly used HDFS Commands are as follows:





<img width="491" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/ae994846-74cc-4f88-9ccc-7048aa291f8e">







11.	Create a directory ‘/input’ in HDFS



<img width="529" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/9e0711e7-41bd-4320-a1c8-37da17182237">


12.	Copy the input files into the distributed file system



<img width="562" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/d895d7cc-5279-4fa1-966c-c41f811a0703">





13.	Run some of the examples provided



<img width="515" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/300907ec-be70-4ab4-907b-ba4c65269a5f">




14.	Examine the output files
Copy the output files from the distributed file system to the local file system and examine them:



<img width="526" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/cd3418ef-34e5-4324-b43b-2bee16b9646a">




 
or
View the output files on the distributed file system

<img width="541" alt="image" src="https://github.com/KayyuruTharani/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209319/26dc3c7f-f08d-4d1c-aa4e-ac9ef9d56a54">




## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.

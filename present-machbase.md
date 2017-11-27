# Introduction



**Table of Contents**

* [Basic Concept](http://doc.machbase.com/introduction$Basic%20Concept)
* [Appearance of New Data](http://doc.machbase.com/introduction$Appearance%20of%20New%20Data)
* [Format of Machine Data](http://doc.machbase.com/introduction$Format%20of%20Machine%20Data)



### Basic Concept



Machbase is a time series database which not only stores massive "Machine Data" in real-time generated from various environments but also performs real-time data analysis.  
Machine data are the time serial log data generated from IoT devices including servers, network devices and applications which are releasing non-stop and real-time data on their status.



### Appearance of New Data



In the IT industry, the wired and wireless communications based IoT \(Internet of Things\) has become a new wave of innovation, and a massive amount of data is being accumulated through it. Thus, if we could analyze the data in realtime, we will be able to point out the problems of the past, and even prevent future challenges.



The number of devices generating data has increased dramatically in recent years and the amount of data that the devices are generating is increasing exponentially as well. On the other hand, the data processing technology still remains outdated. Thus, it is difficult to expect real-time analysis of new data with the conventional software. These are the reasons why the outdated software is not suitable for the processing new data.

  
First, the amount of data is exploding. As the number of data source increases, the number of new types of data also  
increases dramatically. In addition, these lead to the ever-increasing speed of data storage. In reality, the optimized software solution has no other way, but to store data in plain text files in the file system in order to process from tens of thousands to hundreds of thousands data within a second.



Second, the demand for real-time data analysis has been increasing as the rapid increase in data generation. In order to make better decisions with the help of big data, utilizing data is vital, however, the existing solutions have not advanced enough to index hundreds of thousands of data in real-time, and deliver the results to the users after selecting and analyzing data.



Third, the characteristics of "machine data" are completely different than other data. The architectures of traditional database are not suitable for processing the machine data. So new technical approaches are needed in order to solve this issue. With these reasons, Machbase was developed with the best architecture that processes a new form of "machine data" and it is the most ideal solution which can store, process and analyze data in real-time which couldn't be processed with traditional technologies.





### Format of Machine Data



![](http://dzf8vqv24eqhg.cloudfront.net/userfiles/4858/9741/ckfinder/images/2017_04_18_01_50_221.png)

The picture above shows the format of typical machine data.



It has four parts of properties and characteristics as follows.  
• ID: It is expressed in signs or numbers that represent the uniqueness of the device \(original source\) which generates  
machine data. It is composed of a serial number of a machine or sensor, and it is either a 32-bit or 64-bit integer.  
•TIME: It is the exact time that a machine datum is generated, and increases continuously. It is generally represented in a  
unit of seconds, but in special cases, it can be represented in micro-seconds.  
• Binary Information: It is the binary data expressed in integers, real numbers or IP addresses. Typically, it includes  
numbers such as temperature, acceleration, brightness or fixed-data of 4 or 16 bytes such as IPv4 or IPv6.  
• Text log: It refers to text strings in specified languages. This is used when information is impossible to be expressed in normalized numbers or characters. Typical examples of text log include application errors in text strings, like "cause of error, source code, line and error number."



**Figure 1-1 Typical Time Series Data, syslog​**  
![](http://dzf8vqv24eqhg.cloudfront.net/userfiles/4858/9741/ckfinder/images/2017_04_18_01_51_212.png)


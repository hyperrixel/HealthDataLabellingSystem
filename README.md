# HealthData Labelling System

## Project video

[![HealthData Labeling System](https://github.com/hyperrixel/HealthDataLabellingSystem/blob/main/asset/logo.png "HealthData Labeling System")](https://youtu.be/BnRRAaQdzy8)

## Info graphics

### Lifecycle of the data

![Lifecycle of the data](https://github.com/hyperrixel/HealthDataLabellingSystem/blob/main/asset/data_life_cycle.png "Lifecycle of the data")

### Impact of the project

![Impact of the project](https://github.com/hyperrixel/HealthDataLabellingSystem/blob/main/asset/data_route.png "Impact of the project")

### Development work

![Development work](https://github.com/hyperrixel/HealthDataLabellingSystem/blob/main/asset/development_workflow.png "Development work")

### Legal workflow

![Legal workflow](https://github.com/hyperrixel/HealthDataLabellingSystem/blob/main/asset/legal.png "Legal workflow")

### Our vision

![Our vision](https://github.com/hyperrixel/HealthDataLabellingSystem/blob/main/asset/vision_data_tags.png "Our vision")

## Project' description

### The Problem

#### 👉 Description of the problem as we see it:

As the description of the challenge states “More and more healthcare data is being generated by an exponentially increasing number of medical devices and applications.” 


##### 🏥 General healthcare problems

Healthcare system is usually on the bottom section of any government’s budget. Hospitals struggle from underfunding. Doctors and nurses are overwhelmed. The COVID-19 pandemic gives a lot of extra pressure on the healthcare system and on hospitals’ staff as well.


##### ⛔ Accessibility

There are a lot of standards in different fields of healthcare like the Dicom file format in radiology. Companies that operate near the healthcare industry, usually provide data via API services, but those APIs are not synchronized, they do not use the same labeling and tagging method. That’s why using that data is heavy and expensive. Doctors or third party companies have no deep programming knowledge, so if the hospitals have well trained IT staff, they can access data easily.We have personal experiences, since we tried smart bracelets already. When we went to a doctor to show the result, they didn’t know what to do with the exported data file. A properly labelled data stream with a useful UI provides accessibility for users who do not have IT skills.


##### 💪 Competition

Companies could not solve the problem of uniformization since they are competitors and it is bad for the brand if their data labelling method is not chosen for the standard. From the other side, the company that provides the method for standardization has a great advantage over others. 


##### ♻ Not so big data

Nowadays everybody talks about big data and AI systems. At the same time, a lots of data in healthcare are still unlabeled. To train a better AI network, we should provide more and more data. Besides the quantity, the quality is also important. A rich labelled data helps to process the old data as well. For example a well trained NLP solution can process those documents better, that was written and stored before our labelling method. For example, one of the most famous datasets in healthcare related deep learning research is the NIH Chest X-ray Dataset made by the National Institutes of Health. It contains 14 different diseases and 1 label for negative cases. The creators use* Natural Language Processing to text-mine disease classifications from the associated radiological reports. The labels are expected to be >90% accurate. This seems a quite accurate dataset, but it can be better. Besides this, the biggest limitation is that the original associated radiological reports are not publicly available. That’s why we cannot make a cross-validation process or get a second opinion about data.

* link to the original paper: https://arxiv.org/pdf/1705.02315v5.pdf


#### 👉 How this problem impacts us?


##### 🧔 as average people

This is a tricky question, since most of the people say data labelling has no real and present effect on an average human’s daily life. This is incorrect. As an average human, we are visiting doctors and hospitals as others. As we mentioned earlier, we had experience when a doctor could not read the exported data of a smart bracelet. We have a lot of personal health data from smart devices to the official health documents that cannot be merged into a whole dataset, since there is no proper labelling system yet. We could manage each type of data independently from others with the existing softwares. It is kind of funny and sad at the same time, but we have 5 different smart bracelets or watches and we have to use 5 different software or APIs. 


##### 👨‍🔧 as a professional

We are deep learning developers, so we struggle daily with small and poor quality datasets. We had to code a lot to implement an API solution into our workflow. So the problem impact on us not just as normal people, but as a professional as well. 


#### 👉 Why we selected this challenge?

We are committed to healthcare and we like hackathons. Since we are data scientists or deep learning developers, a lot of experience was gained during the years. In the last year we won a hackathon with a healthcare related idea: a file format, which is called DoF*, that helps to store and share datasets easily. Originally we are lawyers, so we can solve the legal issues such as meeting the regulation of GDPR, HIPAA or CCPA. DoF is now integrated into Seagate’s CORTX framework. We think, we can add new viewpoints to solve the problem of this challenge and we have the necessary skills to build something useful, feasible and sustainable.

* link to DoF’s github repository: https://github.com/hyperrixel/dof

### The Solution

#### 👉 Short presentation

We made a video presentation and some code to demonstrate that we are committed to build up our idea. On the github repository there are python codes with a mock example file and C++ header files.

- 🧮 GitHub: https://github.com/hyperrixel/HealthDataLabellingSystem

- 🎥 YouTube: https://youtu.be/BnRRAaQdzy8


#### 👉 Description of the idea

The HealthData Labelling System is a data tagging system where various labels are added to the data while it is moving through the network. There are two main categories for tags:

- 🔷 First is a descriptor that can contain any information that describes a distinct data point.

- 🔷 Second group is a legal layer where the tag describes the legal property of data, like how it has to be handled, whether it is personal or protected data or not.

The goal of the first group of tags is to provide more flexibility during storing and processing the data. While the second group of tags is made for handling who can see the affected data point or it can help during any data point anonymization process.

Giving tags to data points can be automated and the addition process can be built in an already existing workflow. Creating tagging rules are easy due to the JSON-based configuration. However, when the data maker or owner cannot decide which tags should be used, the labelling process can be applied later. Data can be created by sensors, it can be a measurement or dependent from an event or it can be made by a doctor. There is a widely used label-driven file format in healthcare for screening data. This file format is called dicom. It is an old format and we want to create an IoT-ready system that fits the requirements of the modern world. HealthData Labelling System is made not only for screening data, but for any data that can be produced or created in healthcare from sensor data of smart bracelets, during smart ECG devices, to the position of a pump in a respiratory machine. Nowadays big data is essential for the tech industry or healthcare. Our solution can handle data from smart or non-smart devices at the same time. Smart devices can create a lot of new data seconds by seconds, but we should not forget about the old non-smart devices. Working with cutting-edge technologies is really good and interesting, but most of the world has no chance to work with the gadgets of tomorrow.

So industrial entities can create their own standard and labelling system, but these processes can handle the data that is made by their own smart device. It can be good, if a company wants a low-level solution. Our tagging system connects data from different devices independently from the manufacturers.  Besides the data from devices, we aim to tag each kind of data that can occur in healthcare. So basically, we label all kinds of data: sensor, measurement, event, screening, sound, text, other. Let’s see what these categories mean. 

- 🔷 sensor data: any data that is created by a sensor, for example a smart watch, a smart thermometer or pressure sensor from a respiratory machine.

- 🔷 measurement data: numerical data to describe the world such as weight or length of a bad ECG signal as well.

- 🔷 event data: when the data comes from an event in the real world, for example a log when the patient can breathe without the respiratory machine.

- 🔷 screening data: radiology images.

- 🔷 sound: any sound data that can be a notes from a doctor or an analog ECG signal

- 🔷 text: written data.

- 🔷 other: any data that cannot be categorized above.


#### 👉 The main concept of our code

Our code consists of four main types of functionality:

- 🔶 engines

- 🔶 data models

- 🔶 data holders

- 🔶 templates


##### ⚙ Engines

Engines provide the core functionality of our system. The most important engine types are:

- 🔶 collector engines, that collect data from different sources

- 🔶 labeling engines, that label data automatically

- 🔶 storing engines, that stores data based on source and labeling

- 🔶 retrieving engines, that are responsible to allow or deny the data according to permissions or legal circumstances

- 🔶 search engines, that are responsible to find all the data

- 🔶 update and correction engines, that are responsible to provide the possibility of updating data in the given context. These engines repair the system as well if needed.


##### 🔗 Data models

Data models provide system wide structure, naming conventions and constants that help labeling and retrieving processes to store and find the adequate data with the best labels.


##### 🧺 Data holders

Data holders are building blocks used by engines. They provide strict yet flexible structure to serve all the needs of the system.


##### 📜 Templates

Templates can be either simple translation or transcription script or sophisticated algorithms or even artificial intelligence powered software to help labeling. Templates help engines to decide.


#### 👉 The solution

It labels all kinds of data that can occur in healthcare. Label can be a detail label or a legal label. Detail label describes the specific attribute of data, while legal label grants the permissions for users and it provides the system meets the requirements of GDPR or HIPAA regulations. We handle data as a chain where each data point has its own life cycle. Raw data is stored after the first occurrence with the labels and each time when that data is used, the new state is stored with the new labels.


#### 👉 Progress

During this part of hackathon, we write the base structure of code such as abstract functions, classes and a working mock example. We usually use Python for prototyping and C++ or Java for the final, optimized code. However, we wrote C++ headers to show the basics of our concept. We made a development workflow where the marked parts are done till submission:

- 🔷 planning ✅

- 🔷 creating main structure of the code ✅

- 🔷 data integration I. ✅

- 🔷 data integration II.

- 🔷 business planning

- 🔷 creating templates

- 🔷 alpha testing

- 🔷 device and use-case integration

- 🔷 beta testing

- 🔷 contribution with the industry and preparation to version 2.0

The contents of each part are in our presentation video or in the github page of our project.

### The Impact

#### 👉 Impact in the business

Our project has more advantages that spares money and other resources for actors of the healthcare industry in the European or in the global market as well.


##### 📗 Globally unified labeling

At the moment sometimes even two hospitals near each other use totally different labeling habits and labeling systems. The situation is even worse if we compare the habits and systems of different countries. Unifying the labels spares a lot of costs and human resources globally. With the decrease of these entering the market can be cheaper and even small businesses with big ideas can make business globally.

On the other hand unified labeling is essential to build better artificial intelligence solutions. With these new software more lives could be saved and the time to reach the most adequate treatment can be much shorter.


##### 🚏 One-stop before the big step

In our system not just labeling is simple but entering and retrieving are significantly simplified. Joining our system is a low-cost decision with the promise of high return.


##### 💠 The value of the brands 

Since our solution starts as a hackathon project no significant influence of any big company is connected to the idea. Therefore joining our solution in the future doesn’t mean value-loss of a big brand, because the company joins a global and independent service provider.


#### 👉 Impact in the healthcare industry

Our solution impacts the healthcare industry from more directions since it promises business, data and service advantages as well.


##### 🏭 Why will large healthcare providers and manufacturers use our system?

Even large companies suffer from difficulties with data labeling and data management in general. To build a very precise model or artificial intelligence based software an enormous amount of data is needed. In this situation some level of cooperation can help a lot. With our solution we provide this useful level of working together with an easy-to-use and highly scalable system.


##### 🏡 Why will SMEs use our solutions?

Our solution promises the biggest impact for SMEs in the industry because accessing data was never that easy and cheap than with our system.


##### 🧑‍⚕️ Why will healthcare use our solution?

By our experiences doctors don't like to care about labeling or software solutions in general. They used to have their taxonomy in their heads which is based partially on the academic knowledge but partially on individual experience or way of thinking. Therefore waiting until doctors and healthcare will use the same labeling on the whole planet would be an endless challenge. This is where our solutions come into play since we offer the unified labeling systems. Doctors and healthcare staff can focus on their profession to give their best, anything else with the data is yet the responsibility of our system.


##### 💻 Why will data science use our solution?

As we already mentioned, we are deep learning developers, so we struggle daily with small and poor quality datasets. Weaknesses of datasets come from two main sources, bad labeling and not enough data points. Our solution helps to solve both problems since labeling is unified and there will be a lot of data due to the global scope of the system. It is an interesting fact, that the quality of a dataset more characterised by the understandable labeling than the good use of labels, since bad labeling can be filtered out with statistical methods while bad labels cannot be corrected.


#### 👉 Impact for the individuals

Hopefully individuals just enjoy the advantages of our system, like getting the more precise diagnosis faster, or getting much detailed information about diseases, or buying cheaper yet more precise smart devices to measure healthcare related circumstances or factors. However we don't count on individuals as direct business partners we work for making their life much better and for helping to live a healthier life.


#### 👉 Impact to the society

From the view of a much longer perspective this kind of a project can impact even the thinking about data and information inside the data. This whole process can lead to new habits or legislation as well but saying anything concrete in this field is far beyond the scope of this hackathon and beyond the scope of our view too.

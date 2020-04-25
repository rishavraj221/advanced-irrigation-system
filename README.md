# advanced-irrigation-system

This is eedesigned approach with Implementation of Decision Tree for better parameter analysis with alert and control provided by 3rd party app project by Rahul Narang, Indore, India

My basic purpose is to analyze which, why and how the things are used in this project along with the code...

HARDWARE REQUIRED:

* ARDUINO UNO
* TEMPERATURE SENSOR LM35
* RAIN SENSOR
* SERVOMOTOR
* WATER LEVEL SENSOR
* BOLT IOT KIT
* LIGHT SENSOR
* HUMIDITY SENSOR DHT11

INTRODUCTION

The Smart Irrigation System is an IoT based device which is capable of automating the irrigation process by analyzing the moisture of soil and the climate condition (like raining). Soil Parameters like soil moisture, pH, Humidity are measured and the Pressure sensor and the sensed values are displayed in an OLED panel and also on a mobile application.

Thus there came the need to automate it and make a Smart irrigation system so that all the process can be improved.

The shortcomings of the Smart irrigation system were:

1. It only worked for paddy crop

2. Only the temperature predictions were being done in real time

3. There was no advanced control given only three cases were there.

4. Connectivity issues were there which are removed and better connectivity has been provided.

5. In the previous version there was no option to control it from the third party apps which has been provided here.

6. There was issues of serial data transfer which affected the system.

7. Performance optimization has been provided here.'

Hence we are re-engineering the system as Advanced Irrigation System which would be very accurate in nature due to the various machine learning techniques which have been applied on to it so as to make the system as efficient as possible in nature.

Thus in this project we aim to achieve an Advance Irrigation system which offers complete automation by taking in parameters like temperature, water content, humidity, light etc, and then predicting the future values and according to these predictions controlling the entire process on it’s own and hence making the process fully automated in nature. Thus achieves the name Advanced Irrigation System.

CURRENT TRENDS

The current trends in the smart irrigation market include the following techniques which are:

1. Drip Irrigation: allows for precise control of the application of water and fertilizer, which can greatly reduce the amount of water needed for crop irrigation.

2. Measuring Water Flow: Precise measurement of water usage with water flow meters can prevent overwatering and reduce costs for farmers.

3. Data Analytics: New software products that crunch large amounts of data can provide farmers with important information that they previously didn’t have access to.

4. Drilling More Wells: Farmers are relying more on groundwater sources for irrigation and as the water table falls due to unsustainable levels of pumping.

INTERNET OF THINGS (IoT)

The Internet of things (IoT) is the extension of Internet connectivity into physical devices and everyday objects. Embedded with electronics, Internet connectivity, and other forms of hardware (such as sensors), these devices can communicate and interact with others over the Internet, and they can be remotely monitored and controlled. The definition of the Internet of things has evolved due to the convergence of multiple technologies, real-time analytics, machine learning, commodity sensors, and embedded systems.

MACHINE LEARNING

Machine learning (ML) is the scientific study of algorithms and statistical models that computer systems use to perform a specific task without using explicit instructions, relying on patterns and inference instead. It is seen as a subset of artificial intelligence. Machine learning algorithms build a mathematical model based on sample data, known as "training data", in order to make predictions or decisions without being explicitly programmed to perform the task. Machine learning algorithms are used in a wide variety of applications, such as email filtering and computer vision, where it is difficult or infeasible to develop a conventional algorithm for effectively performing the task. Machine learning is closely related to computational statistics, which focuses on making predictions using computers. The study of mathematical optimization delivers methods, theory and application domains to the field of machine learning. Data mining is a field of study within machine learning, and focuses on exploratory data analysis through unsupervised learning. In its application across business problems, machine learning is also referred to as predictive analytics.

4.3 VPS (Virtual Private Server)
A virtual private server (VPS) is a virtual server that the user perceives as a dedicated/private server even though it is installed on a physical computer running multiple operating systems. A virtual private server is also known as virtual dedicated server(VDS). The concept of a virtual private server can be better explained as a virtual machine that caters to the individual needs of a user just as a separate physical computer that is dedicated to a particular user. The virtual dedicated server provides the same functionality and privacy as that of a normal physical computer. A number of virtual private servers can be installed on a single physical server with each one running its own operating system.

A virtual private server can consist of Web server software, a File Transfer Protocol program, a mail server program and different types of application software for blogging e-commerce. Virtual private servers connect shared Web hosting services and dedicated hosting services by filling the gap between them. Because virtual dedicated servers can have their own copy of the operating system, VPS provides the user with super-user privileges in the operating system. VPS enables the user to install any kind of software that is capable of running on that operating system.

BOLT LIBRARY

Bolt is a C++ template library optimized for GPUs. Bolt is designed to provide high-performance library implementations.

For common algorithms such as scan, reduce, transform, and sort. The Bolt interface was modeled on the C++ Standard Template Library (STL). Developers familiar with STL will recognize many of the Bolt APIs and customization techniques, C++ templates can be used to customize the algorithms with new types (for example, the Bolt sort can operate on int, float, or any custom type defined by the user). Additionally, Bolt lets users customize the template routines using function objects(functions) written in OpenCL ™ for example, to provide a custom comparison operation for sort, or a custom reduction operation. Bolt can directly interface with host memory structures such asstd::vector or host arrays (e.g. float*). On today GPU systems, the host memory is mapped or copied automatically to the GPU. On future systems that support the Heterogeneous System Architecture, the GPU will directly access the host data structures. Bolt also provides a bolt::cl::device_vector that can be used to allocate and manage device-local memory for higher performance on discrete GPU systems. Bolt APIs can accept either host memory or the device vector.

DATA FLOW

This script implements the server side analyzing of parameters and generates results.

1. It gathers data from the Arduino hardware using IOT module with the help of bolt library.

2. After acquisition of sensor data, Dataset is imported for further analysis.

3. The Decision Tree model is then trained using the above data set.

4. After training it is tested for accuracy.

5. The new values are fed to the model for output prediction.

7. CIRCUIT DIAGRAM

ALGORITHM

 1. DECISION TREE
Decision Tree algorithm belongs to the family of supervised learning algorithms. Unlike other supervised learning algorithms, the decision tree algorithm can be used for solving regression and classification problems too. The goal of using a Decision Tree is to create a training model that can use to predict the class or value of the target variable by learning simple decision rules inferred from prior data(training data).In Decision Trees, for predicting a class label for a record we start from the root of the tree. We compare the values of the root attribute with the record’s attribute.

Types of decision trees are based on the type of target variable we have. It can be of two types:

1. Categorical Variable Decision Tree: Decision Tree which has a categorical target variable then it called a Categorical variable decision tree.

2. Continuous Variable Decision Tree: Decision Tree has a continuous target variable then it is called Continuous Variable Decision Tree.

Decision trees classify the examples by sorting them down the tree from the root to some leaf/terminal node, with the leaf/terminal node providing the classification of the example.

Each node in the tree acts as a test case for some attribute, and each edge descending from the node corresponds to the possible answers to the test case. This process is recursive in nature and is repeated for every subtree rooted at the new node.





 2. POLYNOMIAL REGRESSION
 
Polynomial Visualizer is a popular data analytics/ML algorithm which helps fit a non-linear curve to a given data-set. The trend can be then used to understand where other data points might lie. The Visualizer aims to help you decide whether Polynomial Visualizer is the right way to go for their ML system, and in case the model works for the data, the Visualizer helps to find the best possible parameters to use with the Visualizer model.

· Prediction points: This number tells the Visualizer how many future data points need to be predicted.

· No. Polynomial coefficients: Polynomial Visualizer processes the given input time-dependent data, and outputs the coefficients of the function of the form:

Data (t) = (Cn*tn) + (Cn-1*tn-1) + (Cn-2*tn-2) + …………… (C1*t1) + C0
which most closely resembles the trend in the input data. This number tells the Visualizer how many elements should be present in the function i.e. the value of n.

· Frame Size: These are the number of previous data points the Visualizer will use to predict the trend of the data. For example, if you set this value to 5, the Visualizer will use the previous 5 points to predict the trend.

VENTING & HARVESTING:

The venting operation has been provided in the sense for the future application of this model in the form of sustainable management field.

The basic operation is quite simple and efficient to preserve the water.

1. The level is checked in comparison to the threshold value

2. Then if it is found that the value crosses the threshold value then the irrigation valve is closed by the system automatically.

3. Then the other servo-motor connected to the tank that stores the excess water becomes active.

4. This servo starts to work and takes the excess water from being wasted and sends it all to the tanks and stores that water.

5. This way the system automatically incorporates the sense of a sustainable system for farming and irrigation purposes and finds a new sense of application.

6. This venting operations works automatically when the auto-mode is selected and hence achieves a kind of efficiency in it’s working thus becoming a completely automated system.

ANOMALY DETECTION

Anomaly detection is the process of identifying unexpected items or events in data sets, which differ from the norm.

In basic graph visualizations anomaly can be easily detected using thresholds being defined Ie.

But what about the visualizations where thresholds cannot be set.

Z-score Analysis is technique used for anomaly detection.

Basically, Z-score is used to compute bounds ie. Upper and lower bounds for the given plotted data.

ALERT & CONTROL

The alert and control feature which has been provided in the project becomes very essential for activities related to farming. This feature basically ensures that the user can get real time information which might affect the different kinds of operations being carried out.

So, basically the anomaly detection algorithm detects any kind of significant change above or below the threshold value which is set.

Then this change is reported to the user as soon as it occurs informing and providing the real time changes.

This information is reported by two ways:

Via e-mail
Through Telegram application





FUTURE SCOPE

There are a lot of applications in which our project can further advance. Since it involves irrigation application of farming it can be further converted into a smart farming system which will in the later stages undertake all the farming applications and completely automate the whole system all while providing the ease of access to the user.

Another application would involve using the techniques used in our project to create a system which could analyse the soil parameters and content of the land also finding out it’s fertility and then further on give an output in terms of suggesting which crop is suitable to grow hence making it a crop prediction application.

Since it’s important to conserve natural resources and water being a very important. Our project provides the opportunity to explore that area too. Hence controlling the flow of excess water and preserving the extra water through various means also while providing an adequate estimate as to which farming application uses most water content. Thus making it an application suitable to be used for sustainable water management.

CONCLUSION

An Advanced Irrigation has been proposed so as to automate the irrigation system and reduce the wastage of water in large areas. The system mainly monitors the behavior of soil moisture, air humidity and air temperature and see how it contributes to evaluate the needs of water in a plant. The system uses machine learning to compare real values obtained from sensors with a test value that has been fed to the machine learning for analysis. The result decides whether irrigation needs to be done or not. The farmer receives an alert on his mobile through which he can choose to turn on the water pump or to turn off. The system has been calibrated for paddy crops. As the future is all about finding alternative ways for different tasks, thus the advanced irrigation system provides ways for getting the desirable results and future predictions. Also while doing this, the paper gives the opportunity to explore the full automation and control of the irrigation system employed and hence offering the option to control the flow of pump. Thereby achieving advanced control functions.

Thank you

ntroduction

Healthcare use cases cover a broad range of scenarios, from personal wearables for health monitoring, through diagnosis and treatment in a medical setting, to high-speed mobility communication between Biomedical sensors to the device and to an ambulance and hospital. However, as technology improves, new devices are being created that can take a more proactive role in healthcare such as providing connectivity to a medical team for remote diagnosis and treatment. These new devices herald the coming of 5G healthcare for Electrical impedance tomography or EMG (Electromyography).From these Biosensors, such immense and diverse data needs special treatment concerning the end-to-end delay, bandwidth, latency, and other attributes. Therefore, the 5G networks are being designed and developed to tackle the diverse communication needs of health-careapplications in the Internet of Things (IoT). 5G assisted smart healthcare networks are anamalgamation of IoT devices that require improved network performance and enhanced cellular coverage. Current connectivity solutions for IoT face challenges, such as the support for amassive number of devices, standardization, energy efficiency, device density, and security.

Salient features

1) Main goal of the project is to build a hand gesture recognition system that can be turned into a wearable device or incorporated into future smart watches. In addition to this, research is going on to find out how the same technology can be used to detect changes in body conditions like sudden spike or drop in blood sugar levels or onset of a seizure.

2) The value added feature of the project can be defined as Non Invasive Biomed Sensing for Cross Section Imaging and Gesture Recognition

Why SMART WEARABLE DEVICE Monitoring USING Blockchain Technology For Healthy Lifestyle By enhancing with Reward System?

Smart Watches and Wearable Devices are rapidly being adopted by customers, bring them more closer to powerful technologies. At the same time, hand based input still remains the best mode of human machine interface (HMI) and we envision a future where hand gestures is all we need to effectively interact with a machine. Leap Motion, Kinect and similar sensors can be seen as earlier implementations of this technology. Wearable versions of the same implementation uses EMG sensor (Myo band) and/or pressure sensors to approximate various gestures.

Bridging the gap between HMI and Wearable Lowe Power devices two is what Project is about - Developing a Hand Gesture recognition system that can be incorporated into a smart watch strap or as a stand alone bracelet, which is low power and much more accurate compared to existing technologies in this field.

Project Objective

The Objective of our project is to build a Bio sensing technology that future wearable devices can incorporate. This technology will then enable gesture recognition for these devices adding better Human Machine Interfacing. Leveraging 5G, IoT and AI on the cloud and with Blockchain makes the patient data tamper proof, this will also be able to sense changes in the users body and take necessary actions as part of our project Biomedical data used :The type of data considered in the proposed blockchain application, e.g. medical health records, personal health records, consent forms, drug information, environmental data, location, Reports, etc. to encourage the patients with diseases like diabetes to monitor their blood sugar by rewarding them with points to obtain items and get some medical tests for free. The Reward system is so extensive with Healthy lifestyle of patients.AI Smart Band that can detect hand gestures and also monitor body for sudden changes in body conditions that may point to seizures or other conditions.

Solution Approach

Leveraging Biosensing Devices with Blockchain so as to maintain tamper proof data of patients The main motive and intent in considering The blockchain is to make use of data from Bio sensable devices :The type of data considered in the proposed blockchain application, e.g. medical health records, personal health records, consent forms, drug information, environmental data, location, medical evidence data. Blockchain defined as a chain of blocks that are time-stamped and connected using cryptographic hashes. A block may contain transactions of many users and generally is publicly available to all users of the network. Additionally, each block contains the hash of the previous block and the transaction data, thus creating a secure and immutable, append-only chain. This chain continuously increases in length as each new block is being added in its end. The blockchain is organized in a peer-to-peer network.

Application area: the specific biomedical area considered in the project, e.g. health records, clinical trials, medicines, medical evidence databases, medical education.

Maturity of approach: using the following scale (a) research proposal of a novel blockchain application; (b) architectural design of a system or system component employing blockchain technologies; (c) implementation of a working prototype of the proposed blockchain system component, with details on the technical platforms and tools used; and (d) evaluation in the real setting.

Reasons for using blockchain: to what end blockchain technology is exploited in each application, for example, access control, non-repudiation, data auditing, data provenance, data versioning and integrity.

Our Project imagine a world where where Smart Wearable device:- 1. The smart band acts as a standalone device, is smart enough to let the user control connected devices, and also monitors their health. 2. Biomonitoring in hospitals is non-invasive and all bands are connected only to a central NextUnit of Computing residing within their premises.

Technology Stack

Blockchain and Python

Advantages of the Smart Wearable devices for the project are defined as follows :-

Non-invasive imaging modality Does not apply any kind of ionizing radiation Electrodes are attached on the surface of a subject Current is injected into the subject through electrodes Real-time radiation-free monitoring tool Neonatal friendly Smaller form factor An unobtrusive system that provides gesture-based input to mobile devices Affords quick access and the capability to interact with a mobile device while being engaged in other physical activities Portable & inexpensive Low power requirements Easy to use and comfortable

The project,aimed to realize proactive, continuous and personalized virtual healthcare utilizing health and fitness data collected from Samsung Galaxy Watch. We work to propose machine learning based healthcare analytics and maximize automated and continuous collection of user data like calories, exercises, sleep, heart rate, step count, contextual data and etc.

Photoplethysmogram (PPG) signals collected by Galaxy Watch were also utilized to estimate continuous blood pressure. Using the proposed feature engineering and selection techniques, we worked to address the limited, noisy, unaligned and irregularly sampled data collected from various sources.

For each chronic condition addressed, like blood pressure and diabetes, we worked to develop personalized prediction and feature importance models based on the collected data and the proposed ML techniques. Not only would the accuracte prediction on chronic conditions indicator based on past health behaviors and context be tailored for the users, but also the most important features influencing the tendency of blood pressure would be given for reference.


## Content Overview
* [Prerequisites](#Prerequisites)
* [Code Organization](#Code-Organization)
* [Dataset](#Dataset)
* [Data Collection](#Data-Collection)
* [Data Visualization](#Data-Visualization)
* [Model Training](#Model-Training)

## Prerequisites
<pre>
1. numpy
2. pandas
3. matplotlib
4. requests
5. json
6. authlib
7. oauthlib
8. base64
9. csv
10. seaborn
11. sklearn 
12. pickle

</pre>

## Code Organization
<pre>
<b>DataRequestAndParsing: for requesting and parsing data </b><br>
  1. read_BP.ipynb: request and parse blood pressure data from Omron
  2. read_samsung_data.py: request and parse health and fitness data from Samsung
  3. new_data_merge.py: combine health and fitness features into one data frame
  
<b>DataUpdate: for regular data maintenance </b><br>
  1. refresh_omron_token.py: refresh tokens for accessing blood pressure data from Omron
  2. refresh_samsung_token.py: refresh tokens for accessing health and fitness data collected by Samsung Galaxy Watch
  3. update_info.py: create csv file with updated health and fitness data

<b>DataVisualization: for data visualization and exploration of correlation </b><br>
	1. visualize_merged_df.py: visualize different features and their underlying relationships
  2. visualize_merged_df.ipynb: for running the script with user index specified
  3. Results: folder of data visualizationr results
  
<b>ModelTraining: for training model to fit blood pressure, health and fitness data </b><br>
	1. aggregate_24h.py: aggregate data in past 24 hours based on the timestamp of each record of blood pressure measurement
  2. build_models.py: extract additional features, convert time form, interpolate data and prepare training model
  3. slp_duration.py: for processing sleep data and computing daily sleep duration
  4. slp_processing.py: for preprocessing sleep data
  
</pre>

## Dataset
- [Omron Blood Pressure Data](https://omronwellness.com/Home/Landing)<br>
  The mobile application <b>Omron Connects</b> helps to transfer the data from the BP monitors to the <b>Omron Cloud Service</b>. We could either download the data from <b>Omron Cloud Service</b> to our server or directly request the data from <b>Omron Connect</b> by OAuth authentication.
  - [diastolic](https://www.verywellhealth.com/systolic-and-diastolic-blood-pressure-1746075) 
  - [systolic](https://www.verywellhealth.com/systolic-and-diastolic-blood-pressure-1746075) 
- [Samsung Health Data](https://developer.samsung.com/health/partner-only/server/api/data-types)<br>
  For the access of data, the <b>Samsung Health</b> mobile application is connected to <b>Samsung Cloud Service</b>, from which we are able to download all related data
  - [calories](https://www.samsung.com/au/support/mobile-devices/galaxy-watch-samsung-health/)
  - [step count](https://developer.samsung.com/health/partner-only/server/api/data-types/step-count)
  - [floors](https://developer.samsung.com/health/partner-only/server/api/data-types/floors-climbed)
  - [exercise](https://developer.samsung.com/health/partner-only/server/api/data-types/exercise)
  - [sleep stage](https://developer.samsung.com/health/partner-only/server/api/data-types/sleep-stage)
  - [heart rate](https://developer.samsung.com/health/partner-only/server/api/data-types/heart-rate)
  - [step daily trend](https://developer.samsung.com/health/partner-only/server/api/data-types/daily-step-count-trend)

## Data Collection
Data collection procedure can be briefly summarized in the following chart.
<p float="left">
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/data_collection.png" width="450"/>
</p>


## Data Visualization
There are some examples demonstrated below.
- <b>Heart Rate Daily and Weekly Pattern</b> & <b>Heart Rate Stacked Plot vs Blood Pressure</b>
<p float="left">
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/heart_rate_weekly_pattern.png" width="400"/>
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/hr_stacked_plot2.png" width="400"/>
</p>


- <b>Daily Sleep Stage</b> & <b>Daily Sleep Duration vs Blood Pressure</b>
<p float="left">
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/daily_sleep_stage.png" width="350"/>
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/slp_bp.png" width="450"/>
</p>

- <b>Daily Step Count</b> & <b>Daily Step Count vs Blood Pressure</b>
<p float="left">
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/daily_step_count.png" width="350"/>
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/step_bp.png" width="450"/>
</p>

- <b> Exercise Event Visualization</b>

![Running](https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/running_trajectory.gif)
![Swimming](https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/swimming_trajectory.gif)

- <b>Daily Proporrion of Sedentary Time vs Blood Pressure</b>
<p float="left">
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/sedentary_bp.png" width="500"/>
  <img src="https://github.com/kwanmolee/Blood-Pressure-Prediction-and-Peronalized-Health-Behavior-Recommendation/blob/master/DataVisualization/Results/sedentary_bp_reg.png" width="300"/>
</p>

## Model Training

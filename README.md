# CyberSecurity-Suspicious-Web-Threat-Interations
This project analyzes web traffic data to detect and classify suspicious or potentially malicious activities using Machine Learning (ML), Feature Analysis (FA), and Data Analysis (DA) techniques.
The dataset, sourced from AWS CloudWatch logs, contains labeled suspicious web traffic records, making it ideal for cybersecurity analytics and threat detection modeling.

📂 Dataset[CloudWatch_Traffic_Web_Attack.csv]
Source: Download Dataset(https://github.com/user-attachments/files/21690064/CloudWatch_Traffic_Web_Attack.csv)

Source: Download Dataset
Description: Includes 282 web traffic records with features such as:
bytes_in, bytes_out
src_ip, dst_ip, src_ip_country_code
protocol, dst_port, response.code
rule_names, detection_types
Timestamps (creation_time, end_time, time)

🛠 Tech Stack
Languages: Python, SQL, Excel
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow, NetworkX
Tools: Jupyter Notebook, VS Code

🎯 Objectives
Import, clean, and preprocess the dataset.
Perform EDA (Exploratory Data Analysis) to understand traffic patterns.
Engineer features like session duration and average packet size.
Visualize suspicious activity trends by country, port, and time.
Implement Anomaly Detection (Isolation Forest).
Build classification models (Random Forest, Neural Networks, CNN) to detect suspicious interactions
Evaluate and report findings.

📊 Key Steps
1. Data Preprocessing
Handle missing values & duplicates.
Convert timestamps to datetime.
Standardize categorical data.
Feature engineering: session_duration, avg_packet_size.

2. Exploratory Data Analysis
Distributions of bytes transferred.
Protocol usage counts.
Country-based suspicious activity analysis.
Port-based suspicious traffic visualization.

3. Modeling
Isolation Forest for anomaly detection.
RandomForestClassifier for binary classification.
Neural Network (Dense layers) for prediction.
CNN for feature-rich classification.

4. Evaluation
Accuracy scores & classification reports.
Visualizations of anomalies and detection results.

📈 Results
Isolation Forest successfully identified suspicious sessions.
Random Forest & Neural Networks achieved 100% accuracy on the given dataset.
High suspicious activity observed on specific non-standard ports and from certain country codes.

📌 Insights
High bytes_in with low bytes_out may indicate infiltration attempts.
Repeated activity from the same IP range could indicate bots or targeted attacks.
Non-standard ports often correlate with unauthorized access attempts.
It can be executed for real time datasets, if datset containing threat detections.




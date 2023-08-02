# Open Weather Pipeline

### This project is my try on integrating AWS, Airflow and python to perform extract, transform and load Openweather climate data.
### The local I chose for this project is Chennai, India. The place that is close to my heart ;)

## Objective of this project

### What value does this project give to an organisation, by taking weather data:
### Insurance and Risk Management:
  <img align="center" src="https://github.com/jayavarshini6/OpenWeather_data_pipeline/blob/master/header.gif">
  
#### Insurance companies leverage weather data for risk assessment and underwriting. Weather-related risks, such as hurricanes, floods, and wildfires, can be better evaluated, allowing insurers to determine appropriate premiums and coverage options.

### Transportation and Logistics:
  <img align="center" src="https://github.com/jayavarshini6/OpenWeather_data_pipeline/blob/master/Transportation-hero-2.gif">
  
#### Weather data plays a vital role in transportation and logistics industries. It helps optimize routes and schedules for ships, aircraft, trucks, and trains, ensuring timely and safe deliveries while considering weather-related disruptions.

### That being said as a Data Engineer I have to address why ETL process play a cruical role?

#### It is essential to collect data and integrate it in a platform so that data can be used for next stages like data visualization, prediction and analysis.
#### Kinda like meal prep so to speak, we cut the ingredients, check our recepie and what masala to use, so that we can get an delicious and visually colourful meal.

### My ETL Architecture

<img align="center" src="https://github.com/jayavarshini6/OpenWeather_data_pipeline/blob/master/Archi.png">


### My take on the tools used in this architecture
#### AWS EC2: EC2 allows you to create and manage virtual machines (instances) on-demand, allowing you to scale up or down based on the workload. This ensures that your ETL pipeline can handle varying data volumes efficiently. And with this it enabled me to get access to Airflow with its instance.

#### Airflow: The main hero in this project, it is a workflow orchestration tool. Airflow provides a powerful and flexible platform for orchestrating complex ETL workflows. It allows you to define, schedule, and monitor data pipelines with dependencies, making it easier to manage the entire ETL process. I personally find airflow every useful with use of DAGS we can visually see and pin point where the process is failing. The DAG logs helped me to figure out what's the issue and solve it. As a visual person Airflow DAG is a great way to understand and keep an eye on your process.

#### AWS S3 (Simple Storage Service): It gave a storage scalability and provides virtually unlimited storage capacity, allowing you to store massive amounts of raw data, intermediate results, and processed data efficiently. The weather data files were stored as a CSV file, with Airflow and AWS credentials it is easy to store all the files in one place.

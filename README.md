
## streaming-04-bonus-Naiema
    
This project demonstrates a data processing pipeline using RabbitMQ with a producer and two consumers.

<br>Author: Naiema Elsaadi</br>
<br>Date: September 10, 2023</br>


## Introduction
The provided Python code is a solution designed to streamline the processing of data from a multi-column CSV file through the utilization of RabbitMQ queues. This project offers an efficient way to split and process data from an input CSV file and apply specific transformations to the extracted information. By distributing the workload to multiple worker processes, this code demonstrates the power of RabbitMQ in managing concurrent data processing tasks.


## Getting Started

 <br><B> Before You Begin </b></br>

**To run this project, follow these steps:**

1. Clone the repository to your local machine.
2. Set up a RabbitMQ server (if not already done).
3. Modify the producer script (producer.py) to send data to RabbitMQ queues.
4. Run the producer script to populate the queues.
5. Run consumer1.py and consumer2.py to process the data and write results to CSV files.

## Project Structure

- `producer.py`: Sends data from `data.csv` to two RabbitMQ queues.
- `consumer1.py`: Monitors the first queue, performs transformations, and writes to `data-result1.csv`.
- `consumer2.py`: Monitors the second queue, performs transformations, and writes to `data-result2.csv`.
- `data.csv`: original csv file, input CSV file with multiple columns.
- `data-result1.csv`: Output CSV file for processed data from consumer 1.
- `data-result2.csv`: Output CSV file for processed data from consumer 2.
- `README.md`: Project documentation.

## Usage

1. Run the three python files in the bash:
in anaconda Prompt (miniconda3) run these: 
  1. **python producer.py**
  2. **python consumer1.py**
  3. **python consumer2.py**
  
  ![My Screenshot](Bonus4.png)


   ## Reference

- [RabbitMQ Tutorial - Work Queues](https://www.rabbitmq.com/tutorials/tutorial-two-python.html)

## Source Data for csv file:
https://www.kaggle.com/datasets/yasserh/housing-prices-dataset

## The following modules are used in this project:
<br> csv	
<br> random	
<br> signal	
<br> sys	
<br> time	
<br> pika

## Prerequisites
<br>Git
<br>Python 3.10+ 
<br>VS studio Code 
<br>anaconda prompt (miniconda3)
<br>RabbitMQ


## Multiple Terminals Screenshots

![My Screenshot](Bonus4.png)
![My Screenshot](Bonus.png)
![My Screenshot](Bonus1.png)
![My Screenshot](Bonus2.png)

## RabbitMQ WebInterface screenshot:

![Streaming in Action](Bonus4_1.png)
![Streaming in Action](Bonus4_2.png)
![Streaming in Action](Bonus4_3.png)


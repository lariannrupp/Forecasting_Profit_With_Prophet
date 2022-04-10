# Forecasting_Profit_With_Prophet

---
![11-4-challenge-image](https://user-images.githubusercontent.com/95719899/162643175-3ac58ec2-d2a4-4cae-b80a-b2bec5f44cc2.png)
---


For the purpose of this exercise, I am a growth analyst at [MercadoLibre](http://investor.mercadolibre.com/investor-relations). With over 200 million users, MercadoLibre is the most popular e-commerce site in Latin America. I've been tasked with analyzing the company's financial and user data in clever ways to make the company grow. So, I want to find out if the ability to predict search traffic can translate into the ability to successfully trade the stock.


---

## Technologies

**A Python 3.9.7 (ipykernal) in JupyterLab** was used to write this notebook.


Additional Python libraries are imported into the start of the app: 


![Screenshot 2022-04-10 165024](https://user-images.githubusercontent.com/95719899/162643270-06f005fa-938f-4551-b5b1-309d46529587.jpg)



---

## Installation Guide

To use the app, from the Github repository, download:
- **forecasting_net_prophet.ipynb** Jupyter file 
- **Resources** folder that contains source data

Use either Terminal or Git Bash to run the app in a conda dev environment. 
To enter a conda dev environment, type
'conda activate dev'

To run the app, navigate to the root directory, which contains all the files adjacent to one another, and then type
'jupyter lab'

---


## Usage:

## Step 1: Find unusual patterns in hourly Google search traffic

<img width="370" alt="image" src="https://user-images.githubusercontent.com/95719899/162643299-3d42c506-d745-49dc-ad3a-209f43c732f2.png">
Google search traffic increased by about 8.5% during the month (May) that Mercado Libre released its financial results

## Step 2: Mine the search traffic data for seasonality
<img width="359" alt="image" src="https://user-images.githubusercontent.com/95719899/162643345-bb6c42e4-2d68-4ad7-a2e2-873df4c77898.png">
Search data is concentrated from hours 20 to hours 3.

<img width="358" alt="image" src="https://user-images.githubusercontent.com/95719899/162643358-24640c13-68f0-40ce-80a1-d343c2b9a2c8.png">
there is an increase during the holiday period (weeks 40-52), and it drops off sharply for a week, that is presumably during the holiday itself.


### Step 3: Relate the search traffic to stock price patterns
<img width="353" alt="image" src="https://user-images.githubusercontent.com/95719899/162643401-b37ac693-b405-41ad-b019-8e36859199a9.png">
The time series indicate that there was a drop in closing price at the same time the seach trends had a steep drop.


### Step 4: Create a time series model with Prophet
<img width="266" alt="image" src="https://user-images.githubusercontent.com/95719899/162643494-fe981496-f6b9-4654-a40e-e7464cecfa17.png">
The near term forecast for Mercado Libre sales, based off Google search traffic


### Step 5: Forecast revenue by using time series models
<img width="271" alt="image" src="https://user-images.githubusercontent.com/95719899/162643533-c2ed5d25-a94c-4147-abf8-6e5274446abd.png">

![Screenshot 2022-04-10 165920](https://user-images.githubusercontent.com/95719899/162643599-ef858e90-d26d-4e7d-8a1a-882a88709e92.jpg)




---

## Contributors

This exercise was based on a challenge problem from UC Berekely Fintech Bootcamp Module 5, accessed on 2022.04.10. 

For any questions, please reach out to me on [LinkedIn](https://www.linkedin.com/in/lari-rupp-5baa49153/)

---

## License

Creative Commons Zero

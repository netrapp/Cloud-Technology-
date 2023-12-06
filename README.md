In this project, I assumed the role as an analyst for MSBA Financial Group, a specialized investment firm. MSBA holds information on publicly traded companies from three different sources, saved in the following tables:

• A Vendor, DataCorp, provides a collection of data from company balance sheets and income statements into the table, datacorp_financials.csv.
• Analyst A is responsible for calculating certain important accounting ratios, using data from DataCorp. These ratios are stored in a table called msba_fg_ratios.csv.
• Finally, Analyst B is responsible for tracking publicly traded companies that have filed for bankruptcy. They store this data in a table called msba_fg_bankruptcy.csv.

The new Chief Information Office (CIO) is frustrated with the decentralized nature of MSBA’s data architecture. She has tasked me with prototyping a cloud-native data architecture in AWS that will achieve the following objectives:
1. Provide a landing place for incoming data of various data types, sizes, and sources.
2. Provide a data warehouse that can facilitate a more centralized “single source of truth” of data for the company’s analyst teams to use regularly. This prototype warehouse should house a table with balance sheet financials, income statement financials, and bankruptcy status consolidated for easier downstream consumption.
3. Make future data ingestion easy to replicate or automate. (You are not tasked with automating data ingestion, only creating a system that could be easily upscaled when the need arises.)
4. Connect to Machine Learning tools that can:
a. Perform cursory Exploratory Data Analysis, and
b. create a Machine Learning model that can predict a company’s likelihood of bankruptcy in the next fiscal year.
5. Use the model to make a prediction. MSBA is considering 10 companies for a new portfolio. Use the model to determine each of the 10 companies’ likelihood of filing for bankruptcy.

In this project, I will demonstrate how to: 
1. How to build an data architecture pipline in AWS for MSBA Financial Group
2. How to think critically about what MSBA Financial Group's data says and reccomend next business steps 

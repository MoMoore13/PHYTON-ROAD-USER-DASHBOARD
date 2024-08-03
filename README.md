# PHYTON-ROAD-USER-DASHBOARD
# Problem Statement

This dashboard shows the number of accident that happened in the month of September 2021. It shows the number of gender per crash, age group by crash, speed limit for each crash and the type of road user crash. Through different ratings, we got the number of crash for each day, & thus how the Law Enforcemnt Agencies can improves their servitude by identifying these areas. It also lets them know the average speed limit for different locations & rush hour time, also the number of high duty vehicle and single crash. By using this dashboard they will identify the problem, which they can further work on factors responsible for these unavoidable crash.

## Questions
1. Total Number of Accident for each day
2. Average Speed for Each Road User
3. Total Number of Accident for Each Road User
4.Total Number of Accident for Gender
5. Average age for Each Road User
6. Total Number of Accident for Each Day of Week 

## Library Used
1. Numpy
2. Pandas
3. Matplotlib

## Steps followed 

- Step 1 : Load Anaconda Prompt.
- Step 2 : In Jupyter homepage, Upload the dataset which is an excel file.
- Step 3 : Go to New to create a new jupyter notebook and rename the notebook.
- Step 4 : Import the libraries(Numpy,Pandas and Matplotlib), Numpy to change the NA values to np.nan, Pandas to deal with changing the data type and the error values, matplotlib for plotting.
- Step 5 : Import the excel file into the notebook to check the information using .info().
- Step 6 : After discovering the content in the dataset, proceeded to clean the data.
- Step 7 : Filling the NA with zero(0) where the column contains numerical values, using fillna
- Step 8 : Replaced Unspecified values to zero(0),<40 to 40, and changed the data type using .astype(int) to integer.

## Question 1

- Step 9 : Using .groupby(), to get the total number of accident for each day.
- Step 10 : Extracted the index and values for plotting.
- Step 11 : Proceed to plotting the graph using bar chart.
    
    ![Screenshot (10)](https://github.com/user-attachments/assets/60b977ce-afe0-4dad-8320-b1ff9e6653ca)

## Question 2

- Step 12 : Using .groupby(), to get the average speed by.
- Step 13 : Extracted the index and values from the groupby result for plotting.
- Step 14 : Plotted the graph using horizontal bar chart.

![Screenshot (11)](https://github.com/user-attachments/assets/a170eed7-a26f-4c4f-b48b-2fff041e6ba5)


## Question 3

- Step 15 : Got the total number of accident for each road user using the groupby function.
- Step 16 : Extracted the index and values from the groupby result for plotting.  
- Step 17 : Plotted a pie chart.

![Screenshot (12)](https://github.com/user-attachments/assets/033c8fa2-c3e9-4dfe-9efd-c594387facb5)


## Question 4

- Step 18 : Got the total number of accident by gender using the groupby function.
- Step 19 : Extracted the index and values from the groupby result for plotting.  
- Step 20 : Plotted using pie chart.

![Screenshot (13)](https://github.com/user-attachments/assets/351921e7-dec2-40e0-8a59-13e07d69be86)


## Question 5

- Step 21 : Using the groupby function to get the age of each road user.
- Step 22 : Extracted the index and values from the groupby result for plotting.  
- Step 23 : Plotted using bar chart.

![Screenshot (14)](https://github.com/user-attachments/assets/3e07f996-5865-4d29-9204-6e1fd3c54f72)


## Question 6

## Question 6

- Step 24 : Using the groupby function to get the total number of accident for each day of week.
- Step 25 : Extracted the index and values from the groupby result for plotting.  
- Step 26 : Plotted using bar chart.

![Screenshot (15)](https://github.com/user-attachments/assets/966f4901-58cc-4969-ac56-3746cc5eaf3a)


- Step 27 : Using subplots to join the different charts together, specifying the number of columns,rows and the figure size inside a variable(ag).
- Step 28 : Gave the charts a title using suptitle, making it bold with font color as red and fontsize at 20.
- Step 29 : Used horizontal bar for the first chart with the title Accident
- Step 30 : Used the scattered chart for the second chart with title Average Speed and color as black
- Step 31 : Used plot chart for the third with the title Road User Accident with colour pink
- Step 32 : Bar chart was used to plot the chart of the fourth with title Accident by Gender
- Step 33 : With the title Average age for Road User, plot chart was used for the fifth chart
- Step 34 : Used pie chart for the sixth chart with the Accident of Dayofweek, giving the chart a shadow and also showing the percentage.

-- fig,ag=plt.subplots(nrows=2,ncols=3,figsize=(10,5))
-- fig.suptitle('CRASH DATA',fontsize=20,fontstyle='oblique',fontweight='bold',c='r')
-- ag[0,0].barh(Name,Values)
-- ag[0,0].set(title='ACCIDENT')

-- ag[0,1].scatter(Name1,Value1,c='black')
-- ag[0,1].set(title='Average Speed')

-- ag[0,2].plot(Names,Value,c='pink')
-- ag[0,2].set(title='Road User Accident')

-- ag[1,0].bar(Nims,Vals)
-- ag[1,0].set(title='Accident by Gender')

-- ag[1,1].plot(Age,Average)
-- ag[1,1].set(title='Average age for Road User')

-- ag[1,2].pie(Num,labels=Days,autopct='%1.0f%%',shadow=True)
-- ag[1,2].set(title='Accident of Dayofweek')

-- plt.tight_layout()
-- plt.savefig('Crash Datas.png')
-- plt.show()

![Crash Datas](https://github.com/user-attachments/assets/4d8a1912-5b54-4b9c-9c35-fe78366985a9)

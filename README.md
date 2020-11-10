# Medical_Appointments_No_Shows

## Tool
Python -- Data wrangling, cleaning, and exploratory data analysis(EDA) 

## Summary
> In this project, I have explored the data related to the dataset Medical Appointment No-show in Brazil. The patients had made the appointment, but did not show up. The whole purpose for this project is to find out what's the feature that influence patients decision.

> * PatientId --Identification of a patient
> * AppointmentID --Identification of each appointment
> * Gender --Male or Female . Female is the greater proportion, woman takes way more care of they health in comparison to man.
> * ScheduledDay --The day someone called or registered the appointment, this is before appointment of course.
> * AppointmentDay --The day of the actuall appointment, when they have to visit the doctor.
> * Age --How old is the patient.
> * Neighbourhood --Where the appointment takes place.
> * Scholarship --True of False . whether or not the patient is enrolled in Brasilian welfare program Bolsa Família.
> * Hipertension --True or False
> * Diabetes --True or False
> * Alcoholism --True or False
> * Handcap --True or False
> * SMS_received --1 or more messages sent to the patient.
> * No-show --True or False. For the No-show: it says ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up.
 
>
>The original dataset can be found here: [kaggle](https://www.kaggle.com/joniarroba/noshowappointments/home)
## Install Package
```{py}
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline
```

## Observations
>In this project, I had done the data wrangling, cleaning, and exploratory data analysis(EDA) to explore the potiential relationship between most of the variables and outcome variable "No show". This is not the end of the analysis, instead, this project is ready for the further analysis to discover more.

>Findings:

> * Around 20% of the patient schedual a appoiment but no show.
> * This dataset contains the appointment for 2016-04-29 to 2016-06-08, where patients can scheduled the since 2015-11-10 to 2016-06-08.
> * The average age of patients are 37. 75% of the patients are lower than 55, and the oldest age is 100 years old.
> * The rate of not showing decrease along the age growth, female tend to be having more no show than male under 35 years old, the tend inverse above 35 years old.
> * The location of the hosipital the contain highest no show rate is SANTOS DUMONT (28.91%), follow by SANTA CECÍLIA (27,46%), and SANTA CLARA (26,48%).
> * Most of the patients made an appointment in the same day and only 4.65% did not show up.
> * The average waiting days for an appoinment is 10 days, 50% of the patients waited for less than 4 days and most of them waited less than 15 days. The longest one had wait for 179 days.
> * In 20 days waiting, it seems that the rate of no shows are growing along with increase of days.
> * Wednesday and Tuesday are the most popular dates for patients to made appointment, Saturday has only 39 times, and None for Sunday. The no-show seems happend less frequency on Thursday.
> * For more appointments one patient made, no-show rate did not go along with it. It manitain the same amount of rate around 20%.
> * It seems the relationship between no show and illness or Scholarship are not clear due to the small sample size of the patients who has the illness.
> * The SMS message does help the patient to show up.
> * Please see [Medical_Appointments_No_Shows](https://github.com/salmoncan0110/Medical_Appointments_No_Shows/blob/main/Medical%20Appointments%20No%20Shows.ipynb) for more detail.


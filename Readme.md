 #                                             TELCO PROJECT:
                                           
  In this project I will be looking at the telco data in order to learn more about what drives customer churn. It will be useful to  first identify the most relevant features in my data by exploring the data and running statistical tests on different attributes of my dataset. I will than use the most relevant features in order to create several models that I can tweak around until I find the parameters that most accurately predict customer churn.
                                           
#                                                     Pipeline:
Plan:
                                            
Aquire: acquire data through functions saved in my acquire.py along with my encrypted credentials.

Prepare: Prepare and clean my data in such a way that I can plug it in to my classification models without causing error and with the prepared data still holding true to its original meaning.

Explore: Ask statistical questions of my data and create visualizations of the results in order to improve comprehension by people reading the report without clarifications from my presentation.

Model:Create models that try to accurately predict customer churn, along with visuals that highlight important findings and help the audiance understand their significance. Validate that all of your models are accurate not just on your train data but on outside data as well.

Deliver: Put all of my findings together in a final report where I make things as easy to understand as possible.

#                                         QUESTIONS TO ANSWER:

1.  Is monthly charges the same amongst people that do and don't churn?
    Hnull - monthly charges is the same amongst people that do and dont churn.
    Halt - monthly charges is not the same amongst people that do and dont churn.

2. Are Fiber Optic customers more likely to churn than other customers?
   Hnull - Fiber optic customers are not more likely to churn than customers with other internet types.
   Halt - Fiber optic customers are more likely to churn than customers with other internet types.

3. Do fiber users on month to month plans churn more than fiber users on other plans?
   Hnull - Fiber users on month to month plans do not churn more than fiber users on other billing plans.
   Halt - Fiber users on month to month plans do churn more than fiber users on other billing plans.
   
4. Do month to month users with fiber churn more than month to month users without fiber?
   Hnull - month to month users without fiber are churning the same amount as month to month users with fiber.
   Halt - month-to-month users without fiber are churning less than month-to-month users with fiber.
#                                                     Data Library

     Column                    Non-Null Count  Dtype  
---  ------                    --------------  -----  
 0   customer_id               7043 non-null   object 
 1   senior_citizen            7043 non-null   int64  
 2   tenure                    7043 non-null   int64  
 3   internet_service_type_id  7043 non-null   int64  
 4   contract_type_id          7043 non-null   int64  
 5   payment_type_id           7043 non-null   int64  
 6   monthly_charges           7043 non-null   float64
 7   total_charges             7043 non-null   float64
 8   is_female                 7043 non-null   int64  
 9   has_partner               7043 non-null   int64  
 10  has_dependents            7043 non-null   int64  
 11  has_phone_service         7043 non-null   int64  
 12  uses_paperless_billing    7043 non-null   int64  
 13  did_churn                 7043 non-null   int64  
 14  has_mult_lines            7043 non-null   float64
 15  has_online_security       7043 non-null   float64
 16  has_online_backup         7043 non-null   float64
 17  has_device_protection     7043 non-null   float64
 18  has_tech_support          7043 non-null   float64
 19  can_stream_tv             7043 non-null   float64
 20  can_stream_movie          7043 non-null   float64
dtypes: float64(9), int64(11), object(1)

   
#                                                    Key Findings:
 
I found 4 important features to focus on in the name of reducing churn, and created a few good models that beat the baseline and one that even broke through 80%. In the future I would like a little more time to tamper with the features I include in my models as I believe doing do could garner further gains in accuracy.
 
#                                                  How To Reproduce:
In order to reproduce my report you will need:
- a personal env with your credentials to access the SQL database.
- you will need to download and move my aquire.py prepare.py into the same directory
-Than you will need to run my report from the same directory.


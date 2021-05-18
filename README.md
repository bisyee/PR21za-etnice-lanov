# PR21za-etnice-lanov
## Initial findings
So far we've looked at data pertaining to the number of hospitalizations in Slovenia by year based on diagnosis, gender, and region. We started off by trying to find any 
correlations between some of the attributes. Since we didn't find anything important we decided to look for the 5 diagnoses that resulted in the highest number of
hospital occupancy. These ended up being: {'Bolezni sečil in spolovil (N00-N99)': 735056, 'Bolezni prebavil (K00-K93)': 955578, 'Bolezni dihal (J00-J99)': 962024, 
'Neoplazme (C00-D48)': 1234724, 'Bolezni obtočil (I00-I99)': 1376298}.

## Findings regarding hospitalizations by diagnosis
We wanted to learn more about these types of diseases so we decided to write a function that would graph the number of people hospitalized for a given diagnosis. We decided to omit people who identify as non-binary and those who did not disclose their gender because their number was very low, rendering them statistically insignificant. We noticed that certain diagnoses are more common among men (Bolezni prebavil, Bolezni dihal, Bolezni obtočil), whereas Bolezni sečil in spolovil are more common among women and Neoplazme are about the same for both genders. Overall, women required more hospital care than men (but this is most likely due to the fact that women outnumber men in Slovenia); the most **dangerous** (i.e. resulting in the need for more hospital care) diagnoses are more common with men. Some of these can be explained, for instance, the number of respiratory problems (Bolezni dihal (J00-J99)) could be explained by the fact that there are more male spokers than female ones [Data found here](https://www.euro.who.int/__data/assets/pdf_file/0016/312046/Fact-Sheet-tobacco-control-Slovenia.pdf). 

## Hospital occupancy by region and period
We made a comparison of the occupancy between the statistical regions and we can see that the region "Osrednjoslovenska" is the most occupied, after it come "Podravska" 
and "Savinjska". The least occupied is the statistical region "Tujina" which says that most of the Slovenian people are treated in Slovenian hospitals. After normalizing the data
we found out that Pomurska, Zasavska and Koroska had the highest number of hospitalizations for their population size. Also we made a graph that shows us the occupancy over the years. We can see that the occupancy in the hospitals over the years increases and that the peak was 2015. From there the occupancy slowly decreases. 

## Deaths by most frequent causes of death
Furthermore we analyzed the number of deaths in hospitals and the causes of deaths. We found out that the most prevalent diseases in Slovenia are the diseases of the urinary tract and genitals, gastrointestinal diseases, respiratory diseases, circulatory diseases and neoplasms. However we continued with analyses and realized that some of them are not in the most deadly diseases. We listed the most deadly diseases: respiratory diseases, gastrointestinal diseases, injuries or poisonings and some other consequences of external causes, neoplasms and as a most dangerous we listed circulatory diseases which is normal since most of the conuntries in the world are fighting with this cause of death. Moreover we analyzed the death rate based on the regions and after normalizing date based on the population we concluded that Primorsko-notranjska has highest death rate, Zasavska is on the second place and Koroska on the third place.
## Prediction model
We wanted to see the relation between the hospitals occupancy and the death rate so we built regression model. We also made a prediction model
## Time series forecasting
We noticed that we use time series forecasting to try and find out how many deaths would occur in the year 2020. We used AR, SARIMA and HWES.

# Education Project


> This project is looking at the relationship between ACT scores and socioeconomic factors of schools to see if there is a statistically significant relationship between them.


---


## Project Overview


This project seeks to determine whether socioeconomic factors are related to average ACT scores in schools across the United States. This project uses NCES data, which contains basic information about each school, and EdGap data, which includes information about average ACT scores for schools and several socioeconomic characteristics of the school district. By creating linear regression models between the socioeconomic characteristics and the average ACT scores for the schools, this project came to the conclusion that socioeconomic factors are statistically significantly correlated with average ACT scores.


## Project Structure


```
├── data/                 # Raw data
├── code/                 # Jupyter notebook
├── reports/              # Communication report
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```


---


## Data


- **Source:** This data was sourced from NCES and EdGap.org.
- ed_gap data: https://raw.githubusercontent.com/brian-fischer/DATA-5100/main/EdGap_data.xlsx
- school_information data: https://www.dropbox.com/scl/fi/fkafjk8902sq8ptxh94r2/ccd_sch_029_1617_w_1a_11212017.csv?rlkey=gucrdz5f6e38bezz2y3yalxbw&e=1&dl=0
- student_teach_ratio data: https://www.dropbox.com/home/SU/Classes/DATA_5100/education?preview=ELSI_csv_export_6389564675853507038315.csv
- **Description:** This data is all downloaded as csvs. The school_information and student_teach_ratio datasets were downloaded from NCES, while the ed_gap dataset was downloaded from EdGap.org.


---


## Analysis


The notebook used in this analysis is education_final.ipynb, located in the code folder. This was the only notebook used in this analysis, and should be run in the order specified in the document. The data was processed by merging the three datasets together, filling in any missing values by imputing them with an iterator, and then creating both single variable linear regression models of every socioeconomic factor and the average ACT scores, and then a multiple linear regression model using all the socioeconomic variables together. Statistical testing is run to determine whether these relationships between variables are statistically significant.


---


## Results


My results showed that there is a statistically significant relationship between each socioeconomic variable and average ACT scores individually. Additionally, the results showed that there is a statistically significant relationship between the variables: student-teacher ratio, percent of married couples, unemployment rates, and percent of students using free and reduced lunches with average ACT scores when put together into a multiple linear regression model. 


---


## Authors


- Jamil Ditter - [@jamilditter]


---


## License


This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


---


## Acknowledgements


- EdGap.org
- NCES
- Brian Fischer

# Olympics
Forecast Paris 2024 Olympics Champions: Insights from Tokyo Olympics
# Paris 2024 Olympics Champions: Insights from Tokyo Olympics

<aside>
💡 The challenge stated to analyze the 2021 Tokyo Olympics dataset to predict who will win the 2024 Paris Olympics. The Tokyo 2020 Summer Olympics, which took place in 2021 due to the COVID-19 pandemic, left a lasting impact:

1. Tokyo 2020 introduced new sports like skateboarding, surfing, sport climbing, and breaking (a dance-based sport). These additions brought fresh energy to the Olympic stage during uncertainty.
2. The Tokyo 2020 Games included athletes from countries like Turkmenistan and San Marino who won their first-ever Olympic medals.
- The Paris 2024 Summer Olympics, which will be hosting the world's top athletes from July 26 to August 11, have faced more interesting coverage regarding the location in which they are taking place. Besides that, notable changes include:
    1. Paris 2024 will feature 28 returning sports and four exciting additions: sport climbing, skateboarding, surfing, and breaking. Breaking, in particular, will make its Olympic debut.
    2. In a historic decision, the International Olympic Committee awarded both Paris (2024) and Los Angeles (2028) the hosting rights simultaneously. Below is a display of all the insights we have gathered after analyzing datasets concerning Tokyo 2020 Olympics and Paris 2024 Olympics:
</aside>

## **Analysis based on the comparison between the number of Medals, Gender and Athletes from Tokyo 2020 Olympics and Paris 2024 Olympics**

1. America remains the highest in 3 medal categories: Gold, Silver, and Bronze

[Top 10 Teams by Total Medals](https://trusted-margin-5ad.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F705a1c89-c5d3-45db-9aa9-ad3c0a10869f%2F0d452d85-7104-49ca-b170-f3a66adf0357%2FUntitled.png?table=block&id=759163b4-87c1-4191-947a-94a039cf5f46&spaceId=705a1c89-c5d3-45db-9aa9-ad3c0a10869f&width=1420&userId=&cache=v2)

- The United States of America was the champion in Tokyo 2020 Olympics

[Top 10 countries by Total Medals](https://trusted-margin-5ad.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F705a1c89-c5d3-45db-9aa9-ad3c0a10869f%2F8abdce2e-1ce0-412a-bfdc-97b5eb632e98%2FUntitled.png?table=block&id=7db43c84-7420-4ee4-a214-f04139f8b426&spaceId=705a1c89-c5d3-45db-9aa9-ad3c0a10869f&width=1420&userId=&cache=v2)

[Total Medals won by each countries](https://trusted-margin-5ad.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F705a1c89-c5d3-45db-9aa9-ad3c0a10869f%2Ff8a9a938-d52c-4e77-b7fc-b9f0dc7f4a9f%2FUntitled.png?table=block&id=0822fa97-0917-4c8c-a22c-24f8e5e150be&spaceId=705a1c89-c5d3-45db-9aa9-ad3c0a10869f&width=1530&userId=&cache=v2)

[Total Medals won by each countries Outliers removed](https://trusted-margin-5ad.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F705a1c89-c5d3-45db-9aa9-ad3c0a10869f%2F9048f770-ca4d-4540-ba9d-5b3a4645da6e%2FUntitled.png?table=block&id=488a1900-2b75-4430-a85e-ebbb3c031a05&spaceId=705a1c89-c5d3-45db-9aa9-ad3c0a10869f&width=1530&userId=&cache=v2](https://trusted-margin-5ad.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F705a1c89-c5d3-45db-9aa9-ad3c0a10869f%2F9048f770-ca4d-4540-ba9d-5b3a4645da6e%2FUntitled.png?table=block&id=488a1900-2b75-4430-a85e-ebbb3c031a05&spaceId=705a1c89-c5d3-45db-9aa9-ad3c0a10869f&width=1530&userId=&cache=v2))

- Scatterplot of athlete count and total medals by discipline
    
    [Athlete count and total medals by discipline](https://prod-files-secure.s3.us-west-2.amazonaws.com/705a1c89-c5d3-45db-9aa9-ad3c0a10869f/3d84cfb2-80c2-4411-8051-26042f2025ef/Untitled.png)
    

# **Applying Random Forest Regressor to predict the number of medals based on Team/NOC**

---

<aside>
💡 We chose Random Forest because of its various abilities:

1. **Handles Large Datasets:** Random Forests efficiently handled the large dataset we created despite it having high dimensionality. They perform well even when there are thousands of input variables.
Feature Importance: Random Forests provided a feature importance score, which helped us understand which variables have the most significant impact on the predictions. This was crucial for interpreting the model and making informed decisions.
2. **Versatility:** Due to uncertainty surrounding the type of prediction, Random Forest could be used for both regression and classification tasks, making them versatile across different types of predictive modeling problems. 
</aside>

[Result]([https://prod-files-secure.s3.us-west-2.amazonaws.com/705a1c89-c5d3-45db-9aa9-ad3c0a10869f/8f4c4c02-ed59-467d-8304-863129a1b444/Untitled.png](https://trusted-margin-5ad.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F705a1c89-c5d3-45db-9aa9-ad3c0a10869f%2F8f4c4c02-ed59-467d-8304-863129a1b444%2FUntitled.png?table=block&id=555f0de5-9cb8-4689-a148-a4d48c2f8f88&spaceId=705a1c89-c5d3-45db-9aa9-ad3c0a10869f&width=1530&userId=&cache=v2)

### Further analysis into the Hypothesis of the Prediction dilemma-

<aside>
💡 A country's success in sports is directly related to the GDP per capita

</aside>

[Correlation between GDP per capita and total medals](https://trusted-margin-5ad.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F705a1c89-c5d3-45db-9aa9-ad3c0a10869f%2Ff156aa95-a75c-4149-a09f-3586f3623ff8%2FUntitled.png?table=block&id=9597f265-f6a2-43e6-b28e-655b1e301383&spaceId=705a1c89-c5d3-45db-9aa9-ad3c0a10869f&width=1260&userId=&cache=v2)

- Being thorough in the process, as well as considering the diversity in a huge event like the Olympics, it’s only natural to dig deeper into the problem beyond the initial obvious factors.
    
    Our studies into the broader frame revealed quite several overlooked factors that indirectly affect the performance of a country and the athletes in the Olympics.
    
- One big factor is the GDP of a country, as the higher the GDP, much better the lifestyle and opportunities to be availed by the populace, leading to better performance in all fields including Sports.
- Other factors include the population size of a country, socio-political interests in the events and so forth.
- Hence from a machine learning angle- the scope of the data involved expands, and incorporating these underlying factors into a concise collection of data and then working on a predictive model with it will yield a much more precise, closer-to-reality prediction.

<aside>
💡 Our efforts revealed work to be done at a much bigger scale than we have anticipated, which we tried to implement yet it went beyond the scope of the hackathon considering the limitations.

</aside>

# **As the Paris 2024 Olympics progress, more data about Athletes and countries involved can be gathered. There is an unlimited scope to this study, but based on our analysis, it is very likely USA will win the most medals again.   This study can be further improved using optimization methods and more information.**

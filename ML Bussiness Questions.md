# ML Questions
## Q1. When should you update your Marketing Mix Models (MMM)?

Predominantly, a ML model needs to be updated for two reasons

1. Model Drift 
2. Business Reasons (`Companies failing to match the pace of this change in customer behavior were hit the worst`.)

Let's first breakdown scenarios where MMM models need updating.

◾️ Seasonality - Some brands in CPG/ FMCG space exhibit seasonality. For e.g. Packaged Juices may sell more during summer.
If your models' last few data points were say of 'Winter months' then the same level of sales demand may not be applicable to the spring and summer months.
To factor this, MMM model needs to be updated.

◾️ Campaign Launch - Sometimes post model building, the brand might have launched a big campaign or perhaps the competitor might have launched a campaign. To capture this effect in the Model, the model may need to be updated.

◾️ Past Error Corrections - Often it comes to light that a campaign spend / TV Spends / Digital Spends etc. were either inflated or under stated due to some error.
Now the model has already been built but it does not mean that we keep the model as it is in light of this error.
In order for the model to capture the reality on the ground, the model needs to be updated. 

◾️ Economic / Geo political and Covid factors

Economic and Geo political factors do affect the MMM models. The current Ukraine - Russia War is already causing high inflations. These changes will be reflected more in certain markets.

Similarly, Covid waves brings with it frequent lockdowns like situations and these too in return affect the economy.
To reflect the effect of these macroeconomic, geo- political and force majeure factors in the model, the model needs to be updated.

### When should you update your MMM model?

MMM models typically needs updating in the frequency of 

Monthly
Quarterly
Half Yearly

How frequently the model needs to be updated depends on :

◾️ **How quickly things have changed on the ground**.
◾️ **How quickly you want to capture the effect and react to these changes**.

📌 Monthly - Generally companies in the non CPG / FMCG tend to prefer monthly level updates since the variables change that quickly and its effect on the outcome variable be it sales, CTR, lead conversion etc. could be reflected early. This is not to say CPG/ FMCG brands don't / won't require monthly updating.

📌 Quarterly - CPG/ FMCG brands typically opt for quarterly updates. This is because some of the initiatives of the brand do take a longer period of time to show effect on real ground.

Moreover, some of the data capture cycle too happens at a quarterly level. Having said this, if there is a frequent change in the market due to macroeconomic, geo political or pandemic, then perhaps the CPG /FMCG brands too can opt for monthly updates.

📌 Half Yearly - Updates this long drawn out is pretty rare. However there are some CPG brands which may not see frequent changes in the market and hence opt for half yearly updates.

### Model Drift::
Model drift can be classified into two broad categories. 
1. **Concept drift**: This happens when the statistical properties of the target variable itself change. As is evident, `if the very meaning of the variable that we are trying to predict, changes, the model wouldn’t really work well for this updated definition`.
2. **Data drift**: This happens when the statistical properties of the predictors change. Again, if the underlying variables are changing, the model is bound to fail. So obvious! A classic example of when this might happen is when the patterns in the data change due to seasonality. Another example is when personal preferences change.

How to address Data Drifting?
* Best way to address this issue is to continuously re-fit the models.
* A more complex methodology to fight model drift is to model the change itself. The first model developed is kept static, and serves as a baseline. 
* The best way to detect drift, however, is continuous monitoring. Metrics related to the stability of the model need to be monitored at continuous intervals.

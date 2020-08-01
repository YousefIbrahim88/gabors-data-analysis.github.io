---
title: "Part IV: CAUSAL ANALYSIS"
author_profile: false
collection: casestudies
---

## CH19	Food and health
Does eating a lot of fruit and vegetables helps remain healthy? Can we use available data on people’s eating habits and health to uncover those effects? What are the most important problems with using such data to answer our question, and can we do anything about them?

This case study uses the `food-health` dataset, cross-sectional data collected on the health and eating habits of people as part of the National Health and Nutrition Examination Survey (NHANES) (USA, 2009-2013). We focus on the subsample of people aged 30-59 years old. The case study illustrates how to define an effect using the **potential outcomes framework**, how to use **causal maps** to visualize our assumptions about the causal relationships between variables, how to translate **latent variables** into their measured **proxy variables** that can be used in actual analysis, how to think about the **sources of variation** in the causal variables, and what variables we should **condition on** in an analysis that attempts to uncover the effect. The case study also illustrates the difficulty of uncovering effects from cross-sectional observational data.


## CH20	Working from home and employee performance
What is the effect of working from home on employee performance? How can we design an experiment that could inform measure these effects? Once the data is collected from the experiment, how should we assess its quality, estimate the effects, and evaluate the internal and external validity of the results?

This case study uses the `working-from-home` data, from an experiment that was carried out at a large travel agency in China, in one of its call centers. The case study illustrates how to design a **field experiment**, what are potential **issues with internal validity** and how to address them in the design or the analysis of the experiment, and how to analyze experimental data. It shows how to check **covariate balance** and how to interpret its results, how to assess **compliance**, and how to use regression analysis to estimate the effects of the experiment. The case study also illustrates how the results of the experiment can be **used in business decisions**, and what issues may arise with the **external validity** of the results.


## CH20	Fine tuning social media advertising
There are many choices to make when designing an online advertisement, inlcuding text content and details of appearance. Having alternative versions of these details, how can we select the version that would yield the most return? 

This case study describes an A/B testing that we carried out on a social media platform. We tested two versions of a text advertising a data analysis program and measured the number of clicks on the ad and the number of actions (leaving one's email address). The case study illustrates the steps of **designing an A/B test** in general, and **power calculation** or **sample size calculation** in particular.


## CH21	Founder/family ownership and quality of management
Many firms are owned by their founder or family members of their founder. Ar such founder/family owned firms as well managed as other kinds of firms and, if there is a difference, how much of that that is due to their ownership as opposed to something else? Can we uncover that effect using cross-sectional observational data on firms and their management practices?

This case study uses the `wms-survey-management` dataset that we introduced in case study 1C. It is a large multi-country multi-sector survey of companies, measuring their management practices and other company characteristics. We use the cross-sectional sample collected from 24 countries between 2004 and 2015. The case study illustrates the use of **thought experiments** to clarify what effect we want to measure, how to think about **what variables to condition on**, and how we may **sign the omitted variables bias**. Besides **multiple regression**, it illustrates **exact matching** and **matching on the propensity score**, discussing their feasibility, advantages and disadvantages, and comparing their results. The case study is another example illustrating the difficulty to uncover an effect using cross-sectional observational data.


## CH22	How does a merger between airlines affect prices?
When two companies merge, the new firm has more market power, and it may use that power to increase prices or decrease quality. How can we measure the effect of a merger between two firms on the price they charge? How can we use panel data from many markets to uncover this effect?

This case study uses the `US-airlines` dataset that is based on 10 percent of all tickets sold on the U.S. market, collected and maintained by the U.S. Department of Transportation. We use this data to evaluate the efect of the merger of American Airlines and US Airways. We define markets and aggregate the data to market-year level and compare price changes across markets with and without the two airlines before the merger. The case study illustrates the use of **transaction data** to carry out a market-level analysis, the difficulties of **defining markets**, and the use if **difference-in-differences** analysis to estimate an effect. It shows how to examine **pre-intervention trends** to assess the **parallel trends assumption**, and how to estimate generalized versions of difference-in-differences analysis adding covariates or using a **quantitative treatment variable**.


## CH23	Import demand and industrial production
How does import demand of a large target country affect the industrial production of a medium-sized open economy? With time series data on imports of the large receiving country and indistrual production of the small open economy, we can estimate a time series regression to uncover the effect. But the the typical time series we can use are not very long, leading to uncertain estimates with wide confidence intervals. How can we use comparable data from other, similar countries to get more precise estimates?

This case study uses the `asia-industry` dataset with monthly time series of industrial production in several Asian countries and imports in the USA. The case study illustrates the use of time series regression to uncover an effect, including **contemporaneous effects**, **lagged effects** and their sum, **cumulative effects**. It then shows how we can use **pooled time series**, time series of the same varables from similar subjects (here countries), to arrive at more precise estimates of the same effect. 


## CH23	Immunization against measles and saving children
Immunization against measles is an effective way to prevent the disease and may save the lives of children. How can we use data from many countries and several years with immunization and child mortality rates to uncover the effect of immunization on the survival chances of children? 

This case study uses the `world-bank-immunization` dataset with data from the World Development Indicators data website maintained by the World Bank to look at countries’ annual immunization rate and GDP per capita. The case study illustrates **panel data regressions** with **fixed-effects (FE)** and estimated in **first differences (FD)**. It shows how the inclusion of **time dummies** can condition on **aggregate trends** of any form, the need to estimate **clustered standard errors** that are robust to heteroskedasticity as well as serial correlation. It shows that the inclusion of **lagged right-hand-side variables** can help capture lagged effects and, in the case of FD models, estimate **cumilative effects**, and the inclusion of **lead terms** of the right-hand-side variables can capture **pre-intervention trends**. It also shows how including unit-specific cosntants in an FD model can help capture **time trends specific for cross-sectional units**. The case study compares the results of FE and FD regressions and discusses their differences. 


## CH24	Estimating the effect of the 2010 Haiti earthquake on GDP
In January 2010, a strong earthquake hit the Caribbean island country Haiti, with an epicenter very close to the country’s capital. What was the effect of the earthquake on the Haitian economy in the short and the longer run? We can easily measure how total GDP changed in the year of the earthquake and how it evolved in the following years. However, to estimate the effect of the earthquake we need to estimate the counterfactual: how total GDP would have changed if Haiti hadn't experienced an earthquake. How van we estimate such a counterfactual?

This case study uses the `haiti-earthquake` dataset with yearly observations of several macro variables for many countries. The case study illustrates **comparative case studies** and how to construct a **synthetic control** observation (here country) from data from other countries to estimate the counterfactual. It shows how to select  **donor pool** of observatons similar to the case study observation (Haiti), how to select the variables whose **pre-intervention values** we want to be similar between the case study observation and the synthetic control observation, and how to use the **algorightm** of the synthetic control method to assign **weights** to each observation in the donor pool to construct the synthetic control observation. The case study also illustrates the **visualization** of the results of synthetic control analysis and the potential issues with the method to uncover the counterfactual.


## CH24	Estimating the impact of replacing football team managers
Success in team sports depends on many things, and the work of the coach, or manager, is likely one of them. When a team performs below expectations, replacing the manager is one of the options teams can consider. How can we use data on all games for several seasons from a professional football (soccer) league and their managers to show how team performance tends to change after a manager is replaced? And how can we use the same data to estimate the counterfactual: how how the performance of low-performing teams would have changed if the manager hadn’t been replaced?

This case study uses the `football` dataset with all games of the English Premier League (EPL) in 11 seasons and who the team manager was at each game. It illustrates the **event study** method to estimate contemporaneous and lagged effects with **xt panel data**. It shows how we can **select a control group** from all observations that is similar, on average, in pre-intervention variables (here team performance) to estimate the counterfactual post-intervention outcomes, and how to define and select **pseudo-interventions** that are necessary to define the control group. We used the same dataset in case study 2B.

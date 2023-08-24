# Interest_NeuralNetwork
## This is the first project I am currently working on to practice some machine learning in PyTorch taking data that influences inflation and then attempting to see, given appropriate time lags if we can predict when it might spike. Here are the inputs:
* Data gathered from the Federal Reserve Bank of St. Luis [here](/fred.stlouisfed.org/series/M1SL/)
* Data gathered from BEA on Gross Domestic Product [here](/https://apps.bea.gov/iTable/?reqid=19&step=2&isuri=1&categories=survey#eyJhcHBpZCI6MTksInN0ZXBzIjpbMSwyLDNdLCJkYXRhIjpbWyJjYXRlZ29yaWVzIiwiU3VydmV5Il0sWyJOSVBBX1RhYmxlX0xpc3QiLCIzIl1dfQ==/)
* Data on JSTOL or the number of jobs not filled by the end of a month again from the Federal Reserve Bank of St. Louis [here](/https://fred.stlouisfed.org/series/JTSJOL)
* Finally, the consumer price index from the Bureau of Labor and statistics [here](/https://data.bls.gov/timeseries/CUUR0000SA0&output_view=pct_12mths)
  * It is worth noting that some of these metrics were decided upon after reading articles [such as this one](https://hbr.org/2022/12/what-causes-inflation)

<p align="center">💵 💶 💴 💷 💰 💸 </p>
<font color="blue"> So, how does all of this come together when using regression and machine learning?</font>

For now, take a look at the code and write up, and there will be more here to emphasise the different techniques used in the process, but as of right now this project is still in development. A few notes on this:
* This is not a traditional use of PyTorch programming as it generally is aimed at breaking down image data, auditory data, or text.
* However, due to the power of neural networks, and the opportunity to learn here, I thought this is a great way to test aptitude, and perhaps perform some powerful work that might be fodder for even more advanced machine learning study of inflationary metrics.
* There was a bit of prep work implemented in the study that also attempted to account for lag times and other factors influencing inflationary pressures.

**It is worth noting that I haven't been able to get the accuracy values up or the loss values down at this point, and am finding inconsistency between different epoch values.**

## Right now, we are in the process of identifying the best ways of tuning the model and have tried the following approaches:

* Using data augmentation by transforming the original dataset to expand.
* Looking at different parameters like momentum, and optmiization functions.
* Addressing loss functions that work with regression and continuous data.
* Setting up an accuracy function that can look at whether a predicted value is within a certain percentage of the target value.



*A quick side note: there are some interesting reports addressing that some of the inflationary data is from corporate profits that are in excess of what market conditions would dictate further increasing inflation. It might be worth further study to read [this article](/https://www.ineteconomics.org/perspectives/blog/profit-inflation-is-real) and compare with the machine learning done here.* 

# Interest_Prediction model
## This is the first project I am currently working on to practice some machine learning in PyTorch taking data that influences inflation and then attempting to see, given appropriate time lags if we can predict when it might spike. Here are the inputs:
* Data gathered from the Federal Reserve Bank of St. Luis [here](https://fred.stlouisfed.org/series/M1SL/)
* Data gathered from BEA on Gross Domestic Product [here](https://apps.bea.gov/iTable/?reqid=19&step=2&isuri=1&categories=survey#eyJhcHBpZCI6MTksInN0ZXBzIjpbMSwyLDNdLCJkYXRhIjpbWyJjYXRlZ29yaWVzIiwiU3VydmV5Il0sWyJOSVBBX1RhYmxlX0xpc3QiLCIzIl1dfQ==/)
* Data on JSTOL or the number of jobs not filled by the end of a month again from the Federal Reserve Bank of St. Louis [here](https://fred.stlouisfed.org/series/JTSJOL)
* Finally, the consumer price index from the Bureau of Labor and statistics [here](/https://data.bls.gov/timeseries/CUUR0000SA0&output_view=pct_12mths)
  * It is worth noting that some of these metrics were decided upon after reading articles [such as this one](https://hbr.org/2022/12/what-causes-inflation)

<p align="center">💵 💶 💴 💷 💰 💸 </p>
<font color="blue"> So, how does all of this come together when using regression and machine learning?</font>

For now, take a look at the code and write up, and there will be more here to emphasise the different techniques used in the process, but as of right now this project is still in development. A few notes on this:
* This is not a traditional use of PyTorch programming as it generally is aimed at breaking down image data, auditory data, or text. Due to this the project was modified to use more of a Numpy/Scikit Learn approach but there are a few PyTorch tensors left in case a similar study would lend itself to deep learning.
* The data was tested for lag times, and used polynomial regression fitting to perform regression analysis.
* After accounting for lag times and curve fitting, the input columns went through a multi-variate regression analysis. 


*A quick side note: there are some interesting reports addressing that some of the inflationary data is from corporate profits that are in excess of what market conditions would dictate further increasing inflation. It might be worth further study to read [this article](/https://www.ineteconomics.org/perspectives/blog/profit-inflation-is-real) and compare with the machine learning done here.* 

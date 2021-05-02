# VBA_Challenge
##Overview
The purpose of this challenge was to refactor solution code so as to more efficiently analyze stock data that would otherwise take much longer to run. The provided dataset displays the recorded volumes of 12 tickers over the years 2017 and 2018, totalling in over 3000 rows of data. The first macros run from Module 2 may work on this dataset but the sheer measure of data will cause it to work more slowly than a refactored version. 
##Results
When applying our original code to our large stock dataset for 2017, the time in seconds it took for the code to run was 0.5546875 as seen below. 
![2017_before](https://user-images.githubusercontent.com/82029390/116830206-9dfc9980-ab76-11eb-89d4-9d02c3ddcdad.png)

When this same code is applied to the stock dataset for 2018, the code took 0.5859375 seconds.

![2018_before](https://user-images.githubusercontent.com/82029390/116830231-d69c7300-ab76-11eb-84a9-e8f65a503a07.png)

After refactoring the solution code, the same data generated for 2017 only took 0.1015625 seconds to run

![2017_after](https://user-images.githubusercontent.com/82029390/116830382-abfeea00-ab77-11eb-9c85-cc8e497a195a.png)
The refactored code was then applied to the dataset for 2018 and took only the same time as refactored 2017
![2018_after](https://user-images.githubusercontent.com/82029390/116830436-eff1ef00-ab77-11eb-8d06-284433f27ecb.png)
Three output arrays were generated to assess the total daily volumes and returns for each ticker per year. The generated tables are below.
2017
![2017_volumes_returns](https://user-images.githubusercontent.com/82029390/116830439-fd0ede00-ab77-11eb-9206-f075ac5389ba.png)
2018
![2018_volumes_returns](https://user-images.githubusercontent.com/82029390/116830444-0d26bd80-ab78-11eb-9963-8e36aacf797d.png)
2017 appears to have been an overall good year to invest in most of these stocks as they all have positive returns and relatively high total daily volumes. This worked particularly well for Steve's parents, as they invested all they have into DQ and DQ had the greatest return of all. TERP exhibited the only negative return of 2017 with a recorded value of -7.2%. 2018 displays a stark contrast to 2017, with nearly all tickers exhibiting negative returns except for ENPH and RUN. 
##Summary
It is evident that refactoring code can generate data faster and allows us to work with larger subsets with more ease. It is however a very time-consuming practice and can prove cumbersome to those who arent very familiar with excel VBA. The original script works well and fast enough to the naked eye that I don't think refactoring introduces a substantial benefit for our purposes. However I can imagine that small measurements of time are very important regarding data generated by stocks every day as they can both increase and decrease significantly in less than a second. 

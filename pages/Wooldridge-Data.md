> The datasets in the table below are referenced in the [Wooldridge
> undergraduate econometrics
> textbook](https://www.cengage.com/c/introductory-econometrics-a-modern-approach-7e-wooldridge/9781337558860PF/)
> with explanations and models described in-text. The original list of
> data is compiled by Boston College, and can be found
> [here](http://fmwww.bc.edu/ec-p/data/wooldridge/datasets.list.html).

Download data and export to Excel
---------------------------------

Using the `wine` dataset as an example, the following code chunks will
export the data to a CSV file, which you can open with Excel.

Stata:

    cd "<directory_path>"
    ssc install bcuse
    bcuse wine  
    outsheet using wine.csv, comma replace

R:

    setwd("<directory_path>")
    install.packages("wooldridge")
    library(wooldridge)
    data('wine')
    write.csv(wine, "wine.csv")

Note that you need to replace the text in the `<brackets>` above. If you
want to clean the data before exporting to Excel, do so after importing
the data, but before exporting to CSV.

List of available data sets
---------------------------

<table>
<colgroup>
<col style="width: 28%" />
<col style="width: 19%" />
<col style="width: 52%" />
</colgroup>
<thead>
<tr class="header">
<th>Name</th>
<th>Sample Size</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>401K</td>
<td>N=1534</td>
<td>cross-sectional data on pensions</td>
</tr>
<tr class="even">
<td>401K-50</td>
<td>N=767</td>
<td>50% sample of 401K dataset</td>
</tr>
<tr class="odd">
<td>401KSUBS</td>
<td>N=9275</td>
<td>cross-sectional data on pensions</td>
</tr>
<tr class="even">
<td>ADMNREV</td>
<td>N=153</td>
<td>timeseries data on offenses</td>
</tr>
<tr class="odd">
<td>AFFAIRS</td>
<td>N=601</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>AIRFARE</td>
<td>N=4596</td>
<td>cross-sectional data on airfares</td>
</tr>
<tr class="odd">
<td>APPLE</td>
<td>N=660</td>
<td>cross-sectional individual data on consumers</td>
</tr>
<tr class="even">
<td>ATHLET1</td>
<td>N=118</td>
<td>cross-sectional individual data on schools’ athletic programs</td>
</tr>
<tr class="odd">
<td>ATHLET2</td>
<td>N=30</td>
<td>cross-sectional individual data on schools’ athletic programs</td>
</tr>
<tr class="even">
<td>ATTEND</td>
<td>N=680</td>
<td>cross-sectional individual data on classes attended</td>
</tr>
<tr class="odd">
<td>AUDIT</td>
<td>N=241</td>
<td>cross-sectional individual data on job offers</td>
</tr>
<tr class="even">
<td>BARIUM</td>
<td>N=131</td>
<td>time-series data on barium export</td>
</tr>
<tr class="odd">
<td>BEVERIDGE</td>
<td>N=135</td>
<td>time-series data on unemployment and vacancies</td>
</tr>
<tr class="even">
<td>BWGHT</td>
<td>N=1388</td>
<td>cross-sectional individual data on birth weights</td>
</tr>
<tr class="odd">
<td>BWGHT50</td>
<td>N=694</td>
<td>cross-sectional individual data on birth weights (50% sample)</td>
</tr>
<tr class="even">
<td>BWGHT2</td>
<td>N=1832</td>
<td>cross-sectional individual data on birth weights</td>
</tr>
<tr class="odd">
<td>CAMPUS</td>
<td>N=97</td>
<td>cross-sectional data on crime in colleges</td>
</tr>
<tr class="even">
<td>CARD</td>
<td>N=3010</td>
<td>cross-sectional individual data on consumers</td>
</tr>
<tr class="odd">
<td>CEMENT</td>
<td>N=312</td>
<td>time-series data for 1964-1989</td>
</tr>
<tr class="even">
<td>CEOSAL1</td>
<td>N=209</td>
<td>cross-sectional firm-level data</td>
</tr>
<tr class="odd">
<td>CEOSAL2</td>
<td>N=177</td>
<td>cross-sectional firm-level data</td>
</tr>
<tr class="even">
<td>CONSUMP</td>
<td>N=37</td>
<td>time-series data on consumption</td>
</tr>
<tr class="odd">
<td>CORN</td>
<td>N=37</td>
<td>cross-sectional individual data on consumers</td>
</tr>
<tr class="even">
<td>CORNWELL</td>
<td>N=630</td>
<td>country panel data</td>
</tr>
<tr class="odd">
<td>CPS78_85</td>
<td>N=1084</td>
<td>pooled CS data for two years</td>
</tr>
<tr class="even">
<td>CPS91</td>
<td>N=1084</td>
<td>pooled CS data</td>
</tr>
<tr class="odd">
<td>CRIME1</td>
<td>N=2725</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>CRIME2</td>
<td>N=92</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>CRIME3</td>
<td>N=106</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>CRIME4</td>
<td>N=630</td>
<td>cross-sectional county data</td>
</tr>
<tr class="odd">
<td>DISCRIM</td>
<td>N=410</td>
<td>cross-sectional firm level data</td>
</tr>
<tr class="even">
<td>EARNS</td>
<td>N=41</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>ENGIN</td>
<td>N=403</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>EZANDERS</td>
<td>N=108</td>
<td>time-series individual data</td>
</tr>
<tr class="odd">
<td>EZUNEM</td>
<td>N=198</td>
<td>time-series individual data</td>
</tr>
<tr class="even">
<td>FAIR</td>
<td>N=21</td>
<td>quadrennial timeseries data for 1916-1992</td>
</tr>
<tr class="odd">
<td>FERTIL1</td>
<td>N=1129</td>
<td>cross-sectional family data</td>
</tr>
<tr class="even">
<td>FERTIL2</td>
<td>N=4361</td>
<td>cross-sectional family data</td>
</tr>
<tr class="odd">
<td>FERTIL3</td>
<td>N=72</td>
<td>cross-sectional family data</td>
</tr>
<tr class="even">
<td>FISH</td>
<td>N=616</td>
<td>cross-sectional data on fish sales</td>
</tr>
<tr class="odd">
<td>FRINGE</td>
<td>N=616</td>
<td>cross-sectional family data</td>
</tr>
<tr class="even">
<td>GPA1</td>
<td>N=141</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>GPA2</td>
<td>N=4137</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>GPA2-20</td>
<td>N=827</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>GPA3</td>
<td>N=732</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>GROGGER</td>
<td>N=2725</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>HPRICE1</td>
<td>N=88</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>HPRICE2</td>
<td>N=506</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>HPRICE3</td>
<td>N=321</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>HSEINV</td>
<td>N=42</td>
<td>timeseries data on real housing invest</td>
</tr>
<tr class="odd">
<td>HTV</td>
<td>N=1230</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>INFMRT</td>
<td>N=102</td>
<td>state-level panel data on infant mortality</td>
</tr>
<tr class="odd">
<td>INJURY</td>
<td>N=7150</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>INTDEF</td>
<td>N=49</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>INTQRT</td>
<td>N=124</td>
<td>time-series quarter data on interest rates</td>
</tr>
<tr class="even">
<td>INVEN</td>
<td>N=37</td>
<td>time-series data</td>
</tr>
<tr class="odd">
<td>JTRAIN</td>
<td>N=471</td>
<td>panel individual data on job training</td>
</tr>
<tr class="even">
<td>JTRAIN2</td>
<td>N=445</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>KEANE</td>
<td>N=12723</td>
<td>panel individual data</td>
</tr>
<tr class="even">
<td>KIELMC</td>
<td>N=321</td>
<td>panel individual data</td>
</tr>
<tr class="odd">
<td>LABSUP</td>
<td>N=156</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>LAWSCH85</td>
<td>N=156</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>LOANAPP</td>
<td>N=1989</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>LOWBRTH</td>
<td>N=1989</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>MATHPNL</td>
<td>N=3850</td>
<td>cross-sectional data</td>
</tr>
<tr class="even">
<td>MEAP93</td>
<td>N=408</td>
<td>cross-sectional school attainment test data</td>
</tr>
<tr class="odd">
<td>MEAP01</td>
<td>N=1823</td>
<td>cross-sectional school attainment test data</td>
</tr>
<tr class="even">
<td>MEAP01_40</td>
<td>N=729</td>
<td>cross-sectional school attainment test data</td>
</tr>
<tr class="odd">
<td>MLB1</td>
<td>N=353</td>
<td>cross-sectional major league baseball data</td>
</tr>
<tr class="even">
<td>MROZ</td>
<td>N=753</td>
<td>cross-sectional labor force participation data</td>
</tr>
<tr class="odd">
<td>MURDER</td>
<td>N=153</td>
<td>longitudinal state murder rate data</td>
</tr>
<tr class="even">
<td>NBASAL</td>
<td>N=269</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>NLS80</td>
<td>N=3710</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>NLS81_87</td>
<td>N=3710</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>NORWAY</td>
<td>N=3710</td>
<td>cross-sectional district data</td>
</tr>
<tr class="even">
<td>NYSE</td>
<td>N=691</td>
<td>time-series NYSE stock price and returns data</td>
</tr>
<tr class="odd">
<td>OPENNESS</td>
<td>N=114</td>
<td>cross-sectional country data on openness to trade</td>
</tr>
<tr class="even">
<td>PATENT</td>
<td>N=2260</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="odd">
<td>PENSION</td>
<td>N=226</td>
<td>cross-sectional individual data</td>
</tr>
<tr class="even">
<td>PHILLIPS</td>
<td>N=49</td>
<td>time-series Phillips curve data</td>
</tr>
<tr class="odd">
<td>PNTSPRD</td>
<td>N=553</td>
<td>cross-sectional gambling point spread data</td>
</tr>
<tr class="even">
<td>PRISON</td>
<td>N=714</td>
<td>state-level panel data on incarceration</td>
</tr>
<tr class="odd">
<td>PRMINWGE</td>
<td>N=38</td>
<td>timeseries data on Puerto Rican minimum wage</td>
</tr>
<tr class="even">
<td>Q</td>
<td>N=2068</td>
<td>firm-level panel data</td>
</tr>
<tr class="odd">
<td>RDCHEM</td>
<td>N=32</td>
<td>cross-sectional data on chemical firms’ R&amp;D expenditures</td>
</tr>
<tr class="even">
<td>RDTELEC</td>
<td>N=29</td>
<td>cross-sectional firm data on R&amp;D</td>
</tr>
<tr class="odd">
<td>RECID</td>
<td>N=1445</td>
<td>cross-sectional data on recividism</td>
</tr>
<tr class="even">
<td>RENTAL</td>
<td>N=128</td>
<td>city-level panel data on rental housing</td>
</tr>
<tr class="odd">
<td>RETURN</td>
<td>N=142</td>
<td>cross-sectional data on CEO salaries</td>
</tr>
<tr class="even">
<td>SAVING</td>
<td>N=100</td>
<td>cross-sectional individual data on consumption and saving</td>
</tr>
<tr class="odd">
<td>SLEEP75</td>
<td>N=706</td>
<td>cross-sectional individual data on sleep patterns</td>
</tr>
<tr class="even">
<td>SLP75_81</td>
<td>N=239</td>
<td>panel individual data on sleep patterns</td>
</tr>
<tr class="odd">
<td>SMOKE</td>
<td>N=807</td>
<td>cross-sectional individual data on smoking</td>
</tr>
<tr class="even">
<td>TRAFFIC1</td>
<td>N=51</td>
<td>state level cross-sectional data on traffic deaths</td>
</tr>
<tr class="odd">
<td>TRAFFIC2</td>
<td>N=108</td>
<td>state level timeseries data on traffic accidents</td>
</tr>
<tr class="even">
<td>TWOYEAR</td>
<td>N=6763</td>
<td>individual cross-sectional data</td>
</tr>
<tr class="odd">
<td>VOLAT</td>
<td>N=558</td>
<td>monthly timeseries data on S&amp;P index</td>
</tr>
<tr class="even">
<td>VOTE1</td>
<td>N=173</td>
<td>cross-sectional individual data on Congressional campaign expenditures</td>
</tr>
<tr class="odd">
<td>VOTE2</td>
<td>N=186</td>
<td>panel data on Congressional campaign expenditures</td>
</tr>
<tr class="even">
<td>WAGE1</td>
<td>N=526</td>
<td>cross-sectional data on wages</td>
</tr>
<tr class="odd">
<td>WAGE2</td>
<td>N=935</td>
<td>cross-sectional data on wages</td>
</tr>
<tr class="even">
<td>WAGEPAN</td>
<td>N=4360</td>
<td>individual panel data on wages</td>
</tr>
<tr class="odd">
<td>WAGEPRC</td>
<td>N=286</td>
<td>macro timeseries data on wages and prices</td>
</tr>
<tr class="even">
<td>WINE</td>
<td>N=21</td>
<td>cross-sectional individual data</td>
</tr>
</tbody>
</table>

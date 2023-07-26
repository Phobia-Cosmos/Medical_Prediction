Simulation Result Represent

1. effectsnpsnumsnp25sigmabeta0.1sigmagamma0.1sigmanoise1.0-1repeats1-0.csv

	行为SNP位置编号，识别某一种特殊SNP变异；列为个体ID（下同）。

|   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|
||SNP|id1_0_id2_0|...|id1_99_id2_99|maf|beta|
|0|rs2519016|0|...|1|0.044554455|1.309562592|
|1|rs7524470|0|...|0|0.069306931|0.331796477|
|...|...|...|...|...|...|...|
|9|rs10399878|0|...|0|0.014851485|0.280258916|

2. episnpsnumsnp25sigmabeta0.1sigmagamma0.1sigmanoise1.0-1repeats1-0_fixed.csv

|   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|
||SNP|id1_0_id2_0|...|id1_99_id2_99|maf|beta|
|0|rs1539637|1|...|1|0.316831683|0.17397573|
|...|...|...|...|...|...|...|
|9|rs9729550|1|...|1|0.272277228|-0.303862929|
|interaction_0_1||0|...|0||0.737287851|
|...|...|...|...|...|...|...|
|interaction_8_9||0|...|0||-0.445819966|

3. epitatic_contributionsnumsnp25sigmabeta0.1sigmagamma0.1sigmanoise1.0-1repeats1-0.csv

|   |   |
|---|---|
|SNP|0|
|id1_0_id2_0|0.05242395|
|...|...|
|id1_99_id2_99|0|

4. fitting_summary_repeat_herit_0.csv

|   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|
|OLS Regression Results|||||||
|Dep. Variable:|y|R-squared:|0.398||||
|Model:|OLS|Adj. R-squared:|0.205||||
|Method:|Least Squares|F-statistic:|2.067||||
|Date:|Thu|20 Jul 2023|Prob (F-statistic):|0.00925|||
|Time:|23:48:48|Log-Likelihood:|-213.97||||
|No. Observations:|100|AIC:|477.9||||
|Df Residuals:|75|BIC:|543.1||||
|Df Model:|24||||||
|Covariance Type:|nonrobust||||||
||coef|std err|t|P>\|t\||[0.025|0.975]|
|const|1.0518|0.776|1.355|0.179|-0.494|2.598|
|x1|1.8541|1.033|1.796|0.077|-0.203|3.911|
|...|...|...|...|...|...|...|
|x25|0.6512|1.599|0.407|0.685|-2.534|3.836|
|Omnibus:|7.035|Durbin-Watson:|2.104||||
|Prob(Omnibus):|0.03|Jarque-Bera (JB):|7.32||||
|Skew:|0.445|Prob(JB):|0.0257||||
|Kurtosis:|3.982|Cond. No.|1.19E+16||||
||||||||
|Notes:|||||||
|[1] Standard Errors assume that the covariance matrix of the errors is correctly specified.|||||||
|[2] The smallest eigenvalue is 4.33e-30. This might indicate that there are|||||||
|strong multicollinearity problems or that the design matrix is singular.|||||||

5. phenotype_numeff_10_numepi_10_herit_0.4_epi_m16_0.1.csv

|   |   |
|---|---|
||phenotype|
|id1_0_id2_0|0.44523667|
|...|...|
|id1_99_id2_99|2.33690941|

6. scale_epistatic.txt

	纯数值，无行列标签。表示模拟过程中的特定参数。

7. Numpy数组文件

	.npy结尾文件为np.save（）结果，保存Numpy数组，方便快速读写。
	
	1. environmental_effect_repeat0.npy
	2. epistatic_paired_effect_sizesnumsnp25sigmabeta0.1sigmagamma0.1.npy
	3. unscaled_epistatic_paired_effect_sizesnumsnp25sigmabeta0.1sigmagamma0.1.npy

# Power BI Experiments - new datasets (same experiments as Pragati251000/PEC)

Each experiment has an Excel dataset (`Datasets/`) and a Power BI project (`Projects/ExpN_.../ExpN_....pbip`).

## How to open (Power BI Desktop, recent version)
1. File > Options > Preview features > enable **Power BI Project (.pbip) save option** and **Store semantic model using TMDL format**; restart Desktop.
2. Double-click the `.pbip` file (or File > Open report > Browse).
3. Click **Refresh** (Home ribbon) so data and calculated tables load.
4. **File > Save as** and pick `.pbix` if you need a single file.

The data is embedded in each project (no file path to fix). The Excel files hold exactly the same data
if you want to practise Get Data > Excel yourself (sheet name = table name).

## Experiments
| Exp | Topic | New dataset | Key items |
|---|---|---|---|
| 3 | OLAP: slice, dice, pivot, drill-down | Electronics sales | Slicer, filtered matrix, Year>Quarter>Month drill |
| 4 | 5 statistical measures | Fashion sales + discount | Avg, Median, Min, StdDev, Max measures; histogram; scatter + trend |
| 5 | Predictive analytics | SaaS monthly sales | Key influencers, scatter + trend line |
| 6 | Forecast + what-if | EdTech revenue | Forecast line, Spend Growth% parameter, Predicted_Future_Sales |
| 7 | Churn analysis | Broadband ISP customers | Total/Churned/Churn Rate, donut, 100% stacked by contract |
| 8 | RFM segmentation | Online grocery customers | Segment slicer, avg monetary, recency vs monetary scatter |
| 9 | Market basket | Bakery & cafe orders | Orders_Both_A_and_B, Confidence matrix |
| 10 | Time-series forecast | Grocery daily sales | DateTable relationship, forecast line, slicers |

Exp 2 in the original repo is an empty page, so it is not included.

## Differences from the originals
- Exp 8: segments are a column in the data (RFM quartile scores). The original used Power BI's automatic clustering;
  to try it, right-click the scatter's legend/details field > Automatically find clusters.
- Exp 4: `Sales (bins)` is a calculated column (bins of 1000) instead of a Power BI group.
- Exp 3 drill-down uses Year/Quarter/Month columns instead of the automatic date hierarchy.

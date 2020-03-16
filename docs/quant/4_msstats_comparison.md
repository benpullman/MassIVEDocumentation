
Once you have or know more than two results by MSstats, you can compare the results from MSstats, using **MSstats Comparisons** in MassIVE.quant.


### 1. Workflow Selection

First, go to the main webpage for [MassIVE](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp). Make sure that you are logged in.  Then go to [the MSstats Comparison Workflow](https://massive.ucsd.edu/ProteoSAFe/index.jsp?params=%7B%22workflow%22%3A%20%22MSSTATS_COMPARISONS%22%7D).

Alternatively on the MassIVE homepage, click **Submit your data** in the `Submit Data` section to bring up the workflow input form and select **MSstats Comparisons** from the drop-down button as the `Workflow`.

<center>
![](img/run_msstats_workflow/msstats_workflow_step0.png)
</center>

Once you have selected the workflow, add the title in the `Title` (at least 30 characters).  Please note this is how you will refer to this task on ProteoSAFe as well as when submitting reanalyses.

<center>
![](img/msstats_comparison/msstats_comparison_step0.png)
</center>

### 2. File Inputs

You can compare between/across either up to 5 MSstats results taken from your MSstats workflow(s) and/or in datasets and reanalyses on MassIVE.


#### 2.1 New result(s) generated by MSstats workflow

If you ran the **MSstats workflow** and haven't submitted the results of the job as a reanalysis, you can select the result file(s) from the list of completed jobs for your user.

1. Click '**+**' sign in front of **Select Input Files from MassIVE Workflows Results** option. Then the jobs that you have run will be shown. In case the job you are hoping to compare is not one of the first 5, you can filter these results by title.  
2. Click the `Select` button at the very right of the row for the job you are interesting in adding to the comparison.

<center>
![](img/msstats_comparison/msstats_comparison_select_jobs_step1.png)
</center>

Then, the new pop-up window, `File Selection`, shows all files generated by MSstats that can be used as inputs to compare.

1. Find the CSV file suffixed **differential_abundance_analysis**. For this workflow, only one output file from MSstats can be compared for each job.
2. Select **Result Files** from the drop-down button in the `Select` column.
3. Click the `Add` button in the same cell.

<center>
![](img/msstats_comparison/msstats_comparison_select_jobs_step2.png)
</center>

Finally, click the `Close` button at the bottom-right on the pop-up window. 


#### 2.2 Published result(s) generated by MSstats

If you know which published result(s) by MSstats you would like to compare, here are the steps that you can select the files:

1. Click '**+**' sign in front of **Select Input Files from MassIVE dataset** option. Then, the list of dataset will be shown.
2. Type MSV ID in the empty box in the first row and below the column named 'Dataset', for example, 'MSV000079843'.  Alternatively, use the title box to search for the dataset you are interested in.
3. Click the `Filter` button at the top left of the table. Then, the row with MSV ID in the `Dataset` column or the title you have searched for is shown.
4. Click the `Reanalyses` button at the very right.

<center>
![](img/msstats_comparison/msstats_comparison_select_published_step1.png)
</center>

Then, the `Dataset Reanalysis Selection` pop-up window helps you select the result files. Find the reanalysis that you are interested in comparing. If there are more than 5 reanalyses in the datasets, please use a double arrow (<< or >>) to see more reanalyses. For example, we are interested in comparing three results in the green box below. We should select them one-by-one. Let's start for row 40. Click the `Select` button at the very right in the row for the reanalysis you want.

<center>
![](img/msstats_comparison/msstats_comparison_select_published_step2.png)
</center>

Then, the new pop-up window, `File Selection`, shows all files in this reanalysis. Let's select the result files from MSstats.

1. Find the result file generated by MSstats. For this example, it is _Choi2017_DDA_Skyline_testResult_byMSstats.csv_. 
2. Select **Result Files** from the drop-down button in the `Select` column.
3. Click the `Add` button at the very right.

Next, click the `Close` button at the bottom-right on the pop-up window. 

<center>
![](img/msstats_comparison/msstats_comparison_select_published_step3.png)
</center>

Repeat the same steps for row 38 and 39. Then, you can see three files are selected in total.
<center>
![](img/msstats_comparison/msstats_comparsion_select_done.png)
</center>


### 3. Workflow Submission

Finally, you are ready to submit. Please type your email to get notice of the progress of the submission and click the **Submit** button.

<center>
![](img/submit_quant_reanalyses/workflow_submission_done_iprg.png)
</center>


Then, you will be redirected to a new page, which shows the progress. Please wait. It will take a few minutes. 

<center>
![](img/msstats_comparison/msstats_comparison_running.png)
</center>

After the job is done, the status will say 'DONE' and you will get the notification email.

<center>
![](img/msstats_comparison/msstats_comparison_done.png)
</center>


### 4. Viewing results

After the job is done, you can see the summary of differentially abundant proteins for each analysis.
**Results** row shows the list of results you selected for **MSstats Comparison** workflow.

There are two results views provided. The first, **View Summary Of Differentially Abundant Proteins**, allows you to explore per condition how many proteins are differentially abundant in each result you are comparing.  The second, **View Differential Abundance Analysis**, gives a more in depth look, and allows for the comparson of individual proteins across different results.

#### 4.1 Summary of the Comparison

Click **View Summary Of Differentially Abundant Proteins** in the **Status** row.

<center>
![](img/msstats_comparison/msstats_comparison_done_click.png)
</center>

The table is the summarization for each comparison (for example, C4-C3) across the selected results.

<center>
![](img/msstats_comparison/result_table.png)
</center>

Click the ion at the left of row number, in the first column. Then the Venn Diagram among differentially abundant proteins will appear.

<center>
![](img/msstats_comparison/result_table_venndiagram.png)
</center>

#### 4.2 Protein-level view

Click **View Differential Abundance Analysis** in the **Status** row.

<center>
![](img/msstats_comparison/msstats_comparison_view_differential_analysis.png)
</center>

The table below will appear.  This contains all of the quantifiable proteins from all of the analyses combined, and gives the adjusted p-value and the fold change for each protein in each MSstats job used for comparison.

<center>
![](img/msstats_comparison/msstats_comparison_differential_analysis_table.png)
</center>

We can filter the rows to see all differentially abundant (adjusted p-value < 0.05, issues = 'NA') proteins for a given analysis and see if they are significant in the other analyses.  Applying this filter on the ```Choi2017_DDNA_Skyline_testResult_byMSstats``` as below, we see that there are 29 differentially abundant proteins across the 6 conditions.

<center>
![](img/msstats_comparison/msstats_comparison_filter_comparison_table.png)
</center>

For each protein, we can look at a plot of the fold change for each result and see how they compare by clicking the graph icon on the left of the row.

<center>
![](img/msstats_comparison/msstats_comparison_comparison_plot.png)
</center>

Finally, by clicking on the double arrows on the left side of the table, we can consider the original outputs from MSstats to see the details of each analysis.

<center>
![](img/msstats_comparison/msstats_comparisons_detail_view.png)
</center>
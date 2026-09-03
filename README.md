# CS5324-Machine-Learning-Lab-1---Table-Data-Exploration

You are to perform preprocessing and exploratory analysis of a data set: exploring the statistical summaries of the features, visualizing the attributes, and addressing data quality. Please upload a report (one per team) with all code used, visualizations, and text in a rendered Jupyter notebook. Any visualizations that cannot be embedded in the notebook, please provide screenshots of the output and embed these screenshots in the HTML of the notebook. Only the rendered HTML notebook should be uploaded.

Dataset requirements: Choose a dataset that is mostly ready to be analyzed. That is, it is already in the format of table data. The following requirements should be met:

    The data includes categorical features (it can also include other forms of data, but must have categorical data)
    The data must be 1,000 rows or larger
    The data must contain missing values that you will impute.
    The data is not strictly image or text data (but could have these data)
    The dataset should have some prediction task associated with it (e., labels to learn, classification)

Some sections are required NOT to use an LLM and are marked appropriately. In some of the sections below, you will work with an LLM. In these LLM-assisted sections, you must:

    Treat the LLM as a collaborator, not a source of truth
    When using an LLM, you must provide:
        What type and version of the LLM you are using and any harness used around the LLM (i.e., are you using plug-ins or agentic flows like Claude co-work or OpenAI Codex)
        Clearly mark what came from the LLM using a different font or other visually striking difference so that LLM outputs are obvious.
        Clearly mark what prompt you employed and make this visually distinct from other text in the notebook.

Your grade depends on the quality of your judgment, not just the correctness of the output. You are expected to encounter at least one instance where the LLM produces a flawed or suboptimal result. Identifying and correcting this is part of the assignment.
Grading Rubric

[1.5 points] Business Understanding. In this portion of the rubric, you will be developing a business understanding section. Prompt an LLM to generate a business understanding summary. You should design a prompt that helps you to:

    Describe the purpose of the data set you selected and how it was collected.
    Describe the prediction task for your data.
    Answer why are third parties interested in the result, and what evaluation measure can be used to prove to third parties that your model works.
    Describe what level of performance would be useful and why.

In your notebook, you should provide the prompt you created and provide the output from the LLM. Points will be given for well-designed prompts. Identify at least two inaccuracies, omissions, or generic statements in the LLM response that should be corrected. Provide a refined version in your own words that corrects these problems. 

[1.5 points] Data Loading. Without the assistance of an LLM, load the dataset and appropriately define data types. What data type should be used to represent each data attribute? Justify representation choices (categorical, ordinal, numeric). For datasets with a large number of attributes, only discuss a subset of relevant attributes. Also summarize missing value in each feature.

[1.5 points] Imputation. Design a strategy for imputing missing data with the help of an LLM. Prompt an LLM to propose a data cleaning strategy and specific imputation methods for missing values. Use the LLM to generate code for implementing these methods and run the imputation methods. It is your responsibility to ensure this code if correct.

    In your own words (not with the help of an LLM), clearly indicate which LLM suggestions you accepted, modified, or rejected. Identify at least one limitation, risk, or incorrect assumption in the LLM’s proposed approach.
    You must verify that the imputation does not introduce unintended effects by Comparing distributions before and after imputation and briefly discussing any observed changes.

[2 points] Exploratory Visualization. Visualize basic feature distributions as instructed below. You may use an LLM to assist with code creation for visualizing. Feature distributions are exploratory distribution plots (like boxplots, histograms, kernel density estimation) that better understand the data.

    You can also use data from other sources to bolster visualizations.
    Visualize at least four distributions, at least one should be of categorical data.
    For two of the visuals (without the assistance of an LLM), describe anything meaningful or potentially useful you discover from these visualizations.
    For at least two of the visualizations, prompt an LLM to interpret the visualization and suggest potential insights/conclusions. Identify one useful or valid insight from the LLM and one issue with the interpretation.

[2.5 points] Research Question Visualization. Potentially with the help of an LLM, ask three interesting analytical questions that are relevant to your dataset and explore visuals that help answer these questions. Questions should be critically examined and directly related to your business case. Ask questions that are interesting and critical to the application. Use whichever visualization method is appropriate for your data. Interpret the implications for each visualization.

If using an LLM for reasoning/interpretation of the visuals, critically evaluate the response highlighting one limitation of the LLM analysis. Be specific in your critique of the LLM by identifying specific aspects such as unsupported claims, ignoring confounding variables, or overgeneralizing.

[1 point] Exceptional Work

5000 level students: Provide additional analysis that meaningfully extends your work. LLM use is optional but must be validated if used.

7000 level students: Choose one of the following (only choose one of these options):

    Option A: Train a random forest model to perform prediction on the dataset. This should be done in such a way that it builds from one of your analytical questions. Interpret the results in the context of this analytical question. LLM use is optional but must be validated if used.
    Option B: Train a TabPFN model to perform prediction on the dataset. This should be done in such a way that it builds from one of your analytical questions. Interpret the results in the context of this analytical question. LLM use is optional but must be validated if used.

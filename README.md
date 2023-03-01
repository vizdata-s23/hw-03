# homework-03

For any exercise where you’re writing code, insert a code chunk and make
sure to label the chunk. Use a short and informative label. For any
exercise where you’re creating a plot, make sure to label all axes,
legends, etc. and give it an informative title. For any exercise where
you’re including a description and/or interpretation, use full
sentences. Make a commit at least after finishing each exercise, or
better yet, more frequently. Push your work regularly to GitHub, and make sure 
all checks pass.

1.  **Thank you.** Make a plot that says “Thank you” on it. Get
    creative! You can make it however you like, e.g., annotation, geoms,
    fake data, etc. There will be points assigned to creativity for this
    exercise. So just annotating the plot with the letters would earn
    fewer points than a more creative approach. Also, use as little as
    defaults as possible, in terms of color scales, themes, etc. The
    plots you make will be shared with our guest speakers as part of a
    “thank you” note. If you would like your name shown on the plots
    shared with them, you should add your name somewhere on the plot,
    e.g., the caption. If you don’t want your name shown, just leave it
    out and the plot will be shared anonymously. (There are no points
    attached to adding your name to them, you can choose to share with your 
    name or anonymously.)
    
2.  **A second chance.** Take one of the visualizations from your first project, 
    ideally one you received more feedback on / lost more points on and 
    improve it. First, write one sentence reminding us of your project and a
    a few sentences on why you chose this plot and how you plan to improve it. 
    Some of these improvements might be "fixes" for things that were pointed 
    out as missing or incorrect. Some of them might be things you hoped to do 
    before the project deadline, but didn't get a chance to. And some might 
    be things you wanted to do in your project but your teammates didn't agree 
    so you gave up on at the time. Some notes for completing this assignment:
    
    -   You will need to add your data from your project to the `data/` folder 
    in this assignment. You do not need to also add the data dictionary.
    
    -   You will need to copy over any code needed for cleaning / preparing 
    your data for this plot. You can reuse code from your project but note that 
    we will re-evaluate your code as part of the grading for this exercise. 
    This means we might catch something wrong with it that we didn't catch 
    before, so if you spot any errors make sure to fix them.
    
    -   Don't worry about being critical of your own work. Even if you lost 
    no points on the plot, if you think it can be improved, articulate how / why.
    We will not go back and penalize for any mistakes you might point out that 
    we didn't catch at the time of grading your project. There's no risk to 
    being critical!

3.  **Median housing prices in the US.** The inspiration and the data
    for this exercise comes from
    <https://fred.stlouisfed.org/series/MSPUS>. The two datasets you’ll
    use are median_housing and recessions, both of which are in the data
    folder of your repository.

    -   Load the two datasets using `read_csv()`.

    -   Rename the variables as date and price.

    -   Create the following visualization.

    <img src="images/median-housing-1-1.png" width="90%" />

    -   Identify recessions that happened during the time frame of the
        `median_housing` dataset. Do this by adding a new variable to
        recessions that takes the value TRUE if the recession happened
        during this time frame and FALSE if not.

    -   Now recreate the following visualization. The shaded areas are
        recessions that happened during the time frame of the
        `median_housing` dataset. Hint: The shaded areas are “behind” the
        line.

    <img src="images/median-housing-2-1.png" width="90%" />

    -   Create a subset of the `median_housing` dataset for data from
        2019 and 2020 early. Add two columns: `year` and `quarter`.
        `year` is the year of the `date` and `quarter` takes the values
        Q1, Q2, Q3, or Q4 based on `date`.

    -   Create the following visualization.

    <img src="images/median-housing-3-1.png" width="90%" />

4.  **That’s what our guest said.** We had a guest lecture by Dr. Matthew 
    Kay on Thu, Feb 23. This question as about what you learned in the guest 
    lecture as well as the reading assigned for the lecture:
    
    a. You’ve either attended that guest lecture in person or you should have 
    watched the recording on Panopto by now. Write a one paragraph summary of 
    the guest lecture. Make sure your summary includes at least one thing that 
    you didn’t know before. This can be a tip for better visualization, a 
    tool/package, or a workflow. Your answer can be just text or also 
    include code.
    
    b. Using the `openintro::loans_full_schema` dataset, fit a linear 
    model predicting `interest_rate` from `loan_purpose`. Print out the 
    regression output with `broom::tidy()`. Then, using half-eye plots, 
    plot the confidence intervals around each of the slope coefficients 
    and the intercept. Based on your plot, (1) comment on how the variability 
    of the slope coefficient for various levels of `loan_purpose` varies and (2) 
    describe in one or two sentences how the p-values in the regression output 
    correspond to the widths of the confidence intervals. Hints: (1) Take a look 
    at how many loans per each type of loan purpose. Does that help explain 
    why some curves are very wide while others are much narrower? (2) Which 
    95% confidence intervals include 0 and which don't? How does that correspond 
    to which p-values are less than 0.05 and which are not?

5.  **Du Bois challenge.** Recreate the following visualization by W.E.B. 
    Du Bois on family budgets split by income classes for 150 families in 
    Atlanta, Georgia. This visualization was originally created using ink 
    and watercolors.

    <img src="images/income-expenditures-orig.jpeg" width="90%" />

    Notes for recreation:

    - Use the `data/income.csv` as your starting point.
    
    - You do not need to recreate (1) the plot title, (2) the dollar coin 
    (the circle on top left) and the arched "Annual Income" text above it, 
    (3) the image and tiny text inside the legend box.
    
    - It is also ok if your y-axis isn't a table like the one shown on the 
    plot, but you want to make sure you do have the income ranges styled as 
    closely as possible to the plot.
    
    - To change the background of the plot to match the background of the 
    original visualization, look for an image of a "parchment paper" on a 
    free image site like Pixabay ([https://pixabay.com](https://pixabay.com/)) 
    and place the image file in your `images/` folder and the image in the 
    background of the plot.
    
    - You are welcomed to use the steps outlined in `ae-12` to recreate this, 
    but you do not have to. You can do it all in one step as well. Note that 
    the steps contain good hints though, so if you're struggling, make sure to 
    look there first.

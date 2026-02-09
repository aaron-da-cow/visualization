    > What software did you use to create your data visualization?

I used a Jupyter Notebook running the python environment from class. Specifically, I used the Pandas library to clean the data, and the Seaborn library to generate the heatmap. I used Matplotlib to manipulate the labels and dimensions. 

    > Who is your intended audience? 

The intended audience is urban planners and city officials to understand how and when people use bikes even in the harsh and unaccommodating winters of Toronto. 


    > What information or message are you trying to convey with your visualization? 

A heatmap conveys the distinct demand of ridership during work hours during the weekdays, and the demand of leisure travel during the weekend. This suggests that bike riders who use the service use them for this purpose. 
    
    > What aspects of design did you consider when making your visualization? How did you apply them? With what elements of your plots? 
    
I focused on gestalt principles of continuity. By using a heatmap, the viewer sees the hot spots as continuous blocks of time rather than lines or bars. I reordered the y-axis so that it starts on Monday to reinforce the needs of weekdays in contrast to the weekends in part to match the viewer's standard mental model of a working week.


    > How did you ensure that your data visualizations are reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization? 
    
By using a script rather than manually editing the files, I have ensured reproducibility. By handling file encoding with latin1 in the code, I have ensured that the script is robust. I also used pandas to clean an inconsistency in spaces.

    > How did you ensure that your data visualization is accessible?  

I selected the Viridis colourmap so that it remains distinguishable to most people, including those with common forms of colour blindness. I also ensured that the axes were labeled with 12pt font. 
    
    > Who are the individuals and communities who might be impacted by your visualization?  

This visualization focuses on the average commuter; aggregating the data accross the whole city. This, therefore, could potentially neglect the needs of night time shift workers, or those who live in suburbs and hilly areas where there is comparatively less ridership. If the urban planner makes decisions solely on this map, priority would go to downtown rather than suburban expansion.
    
    > How did you choose which features of your chosen dataset to include or exclude from your visualization? 

I included the start time and day of the week to identify temporal patterns. I excluded the user type (annual vs casual) to showcase the total system usage. I filtered out trips under a minute as they are probably user error (i.e. trying to dock the bike or accidentally creating a new trip).
    
    > What ‘underwater labour’ contributed to your final data visualization product?

The largest "underwater labour" task was file encoding. When I first loaded the file, I got a UnicodeDecodeError, which I solved after investigation by specifically providing the parameter of encoding='latin1'. 
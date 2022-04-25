# Data Visualization Follow-Along
Follow these instructions to get some practice visualizing data!

## Part One: Spreadsheet Graphing
Take a look at some data in a spreadsheet, and see how it can be made into some basic charts.

### Getting Started
The data is available here: https://docs.google.com/spreadsheets/d/1vqKSvuF79aOkbwFT3VR4fE4HLmGmt0f_vNthz3erDFk/edit?usp=sharing

**In order to work with it, it will be necessary to sign into a Google account.** Once signed in, select "Make a copy" from the "File" menu:

![](https://i.imgur.com/wLBUYDA.png)

After that, you can edit the spreadsheet and create charts! Select the "Chart" option from the "Insert" menu to add one:

![](https://i.imgur.com/mGRxspx.png)

### Column Meanings
Here's a rundown of what each column actually means:

- `Private`: Public/private indicator
- `Apps`: Number of applications received
- `Accept`: Number of applicants accepted
- `Enroll`: Number of new students enrolled
- `Top10perc`: New students from top 10% of high school class
- `Top25perc`: New students from top 25% of high school class
- `F.Undergrad`: Number of full-time undergraduates
- `P.Undergrad`: Number of part-time undergraduates
- `Outstate`: Out-of-state tuition
- `Room.Board`: Room and board costs
- `Books`: Estimated book costs
- `Personal`: Estimated personal spending
- `PhD`: Percent of faculty with Ph.D.’s
- `Terminal`: Percent of faculty with terminal degree
- `S.F.Ratio`: Student/faculty ratio
- `perc.alumni`: Percent of alumni who donate
- `Expend`: Instructional expenditure per student
- `Grad.Rate`: Graduation rate

### Private College Pie Chart
Start with a basic chart showing how many of the colleges are private, and how many are public.

1. If there is a title, click it and change it to "Private Colleges"
1. In the "Chart editor" pane that appears on the right, choose "Pie chart" as the Chart type
1. For the Data range, open the selector and choose "A1:S778"
1. For the Label, choose "Private"
1. Check the "Aggregate" box
1. Remove any Value that was added

At the end, it should look something like this:

![](https://i.imgur.com/wlbcLbw.png)

It appears that there are many more private schools than public ones!

### Room & Board vs. Out-of-State Tuition
Next, create a scatter plot comparing Room & Board cost to Out-of-State tuition.

1. If there are titles, change them to the following:
    - Main title: "Room & Board vs. Out-of-State"
    - X-axis label: "Room & Board Cost"
    - Y-axis label: "Out-of-State Student Tuition"
1. In the "Chart editor" pane that appears on the right, choose "Scatter chart" as the Chart type
1. For the Data range, open the selector and choose "A1:S778"
1. For the X-axis, select "Room.Board"
    - Make sure "Aggregate" is _not_ checked
1. For the Series, select "Outstate"
1. Make sure the "Treat labels as text" checkbox at the bottom is _not_ checked

At the end, it should look something like this:

![](https://i.imgur.com/48VUfdk.png)

Based on this, it appears that when the room & board cost is higher, there is also a higher out-of-state tuition.

#### OPTIONAL: Bubble Chart
To continue this line of thinking, change the chart into a Bubble chart, and add "Private" as the color dimension. The settings should be something like this:

![](https://i.imgur.com/mQM2fvb.png)

Looks like private schools have both higher room & board costs _and_ higher out-of-state tuition!

### Applications, Acceptance, and Enrollment
For the next chart, find out how many students applied, were accepted, and enrolled at both private and public colleges.

1. If there are titles, change them to properly match the data columns used
1. In the "Chart editor" pane, choose "Column chart" as the Chart type
1. For the Data range, open the selector and choose "A1:S778"
1. For the X-axis, select "Private"
    - Make sure the "Aggregate" checkbox is checked
1. For the Series, add each of the following:
    - Apps
    - Accept
    - Enroll
1. Set the Series Aggregate Type to "Sum"

It should look something like this:

![](https://i.imgur.com/AyGjUtI.png)

Even though there are many more private colleges, more students are enrolled at public colleges overall!

## Part Two: Custom Programming with Python and `ggplot`
This part of the follow-along activity will take place in Google Colab. Make a copy of [this notebook](https://colab.research.google.com/drive/1bo9vubNJkGDzvNZx9rRP1XII_jz5oF0f#scrollTo=4iFzpN7VGXyc) to begin. All of the instructions are there, along with the code!

## Beyond
After part two, head back to the [main page](StudentDesc.md) to see what else there is to explore!
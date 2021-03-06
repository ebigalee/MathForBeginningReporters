#Math and Data for beginning reporting#

#####Credits#####

This document was started by Matt Waite, professor of practice in the College of Journalism and Mass Communications at the University of Nebraska-Lincoln. 

**Contributors**

    names here

##Summary##

All communicators, regardless of interest, discipline or medium, need to understand numbers to do their jobs effectively. More and more of society is being transformed by data as our lives are increasingly stored in databases. If you can't understand data and the basic math that you'll use regularly on the job, you are at the mercy of people who can.

This module is designed to solve a particular problem: How do you get basic data journalism into a beginning reporting class that many feel is packed as it is? My answer is to combine the basic math for reporters with instructions on how to apply those concepts in a spreadsheet using real data, all aimed at generating real story ideas. This document will show: 

* Basic math concepts and how to calculate them by hand.
* How to apply those basic math concepts to a spreadsheet of data.
* How to turn basic math + a spreadsheet of data into a story idea.

Contained in this repository are the datasets used to illustrate the concepts. They are kept here in .csv format, so you can use Excel or Google Spreadsheets to do the same analysis. The spreadsheet formulas and concepts will work on any of those three software platforms.

##Introduction##

#####Bad at math is a lie#####

Let me guess: There's a not-insignificant part of you that's pretty happy to be in journalism school because the math requirements are pretty minimal. Have you ever said, out loud, "I can't do math, I'm a journalism major!" Have you ever thought "It's okay, I'm bad at math." Have you been bad at math your whole life?

First, you're not alone.

Second, you're living a lie.

That's right. A lie. Bad at math is not a thing. And you are not bad at math. You just think you are. [And it's a destructive lie you tell yourself.](http://www.niemanlab.org/2013/11/matt-waite-how-i-faced-my-fears-and-learned-to-be-good-at-math/)

You, like me, struggled with math at some point when your friends didn't. They kept going, you kept struggling, and suddenly they were good at math and you were not. And here you are today.

Except with journalism today, you can't continue to live the lie. You are surrounded by data. You are surrrounded by numbers. If you continue to believe you're bad at math, you will be easy to fool by people who aren't. You'll be unable to see stories that are sitting there in the numbers. 

In short: you won't be a very good journalist.

The good news? This isn't very hard. The types of math that get you in the door are really quite easy. And you can do some very powerful things.

#####How high school algebra won a Pulitzer Prize#####

If you were at all paying attention in pre-college science classes, you have probably seen this equation:

    d = rt or distance = rate*time
    
In English, that says we can know how far something has travelled if we know how fast it's going and for how long. If we multiply the rate by the time, we'll get the distance.

If you remember just a bit about algebra, you know we can move these things around. If we know two of them, we can figure out the third. So, for instance, if we know the distance and we know the time, we can use algebra to divide the distance by the time to get the rate.

    d/t = r or distance/time = rate 

In 2012, the South Florida Sun Sentinel found a story in this formula.

People were dying on South Florida tollways in terrible car accidents. What made these different from other car fatal car accidents that happen every day in the US? Police officers driving way too fast were causing them. 

But do police regularly speed on tollways or were there just a few random and fatal exceptions? 

Thanks to Florida's public records laws, the Sun Sentinel got records from the toll transponders in police cars in south Florida. The transponders recorded when a car went through a given place. And then it would do it again. And again.

Given that those places are fixed -- they're toll plazas -- and they had the time it took to go from one toll plaza to another, they had the distance and the time.

[It took high school algebra to find how fast police officers were driving. And the results were shocking.](http://www.sun-sentinel.com/news/local/speeding-cops/fl-speeding-cops-20120211,0,3706919.story)

Twenty percent of police officers had exceeded 90 miles per hour on toll roads. In a 13-month period, officers drove between 90 and 110 mph more than 5,000 times. And these were just instances found on toll roads. Not all roads have tolls.

The story was a stunning find, and the newspaper documented case after case of police officers violating the law and escaping punishment. And, in 2013, they won the Pulitzer Prize for Public Service. 

All with simple high school algebra.

##The basics of the basics##

**If you don't know these, you are doomed from the start.**

#####Notation####

One of the most difficult hurdles for beginning students of mathematics to get over is notation. If you miss a day, tune out for a class, or just never get around to asking what something means, you'll be lost. So lets just cover some bases and make sure we all understand some ultra-basic notation. 

You might laugh at these, but someone reading them is looking up Gods on Wikipedia to thank. So do yourself a favor and refresh.


|Symbol|Meaning|Example| 
|------|-------|-------|
|+|addtion|5+2|
|-|subtraction|6-2|
|* |multiplication|7*2|
|/|division|8/2|
|^|exponent|2^3|
|sqrt|square root|sqrt(4)|

	Author notes: More? Delta? Sigma? Coming back to this.


#####Order of operations#####

One of the most important and often overlooked concepts in basic math is the order that you do the calculations. When you have something like `5+5*5^2`, which gets done first? Or, as you'll read in the next section, what comes first when you calculate the average of a thing? The adding up of all the numbers or the division by the number of numbers?

Thankfully, math teachers have provided us an easy to remember memonic that you probably learned in sixth grade and forgot until now. 

**PEMDAS** -- **P**arenthesis, **E**xponents, **M**ultiplication, **D**ivision, **A**ddition, **S**ubtraction

What that means is when you look at a mathematical formula, you do the calculations in the order PEMDAS tells you. Something in parenthesis? Do that first. Is there an exponent? Do that next. Multiplication or division? It's next and so forth.  Knowing PEMDAS will save you from stupid mistakes down the road.

#####Spreadsheets#####

Spreadsheets are one of the most basic and useful tools for data analysis. They are the Swiss Army Knife of data analysis. They're immensely useful. But like a Swiss Army Knife, they're useful for a lot of things, but they're never the best tool for that thing. Statistical analysis? Spreadsheets are great for that, but there are statistics software packages that are better. Graphics and visualizations? You can do amazing work in a spreadsheet, but there are visualization packages that are better. Complex queries? It can be done with a spreadsheet, but a database is better. 

But the simple truth is almost all data analysis, and data analysts, begin or end with a spreadsheet. They're the one tool every data nerd has. 

And they're a great place to start.

But before we can get started, you have to understand some basics. If you've never used a spreadsheet before, you'll learn really quickly that spreadsheets organize data into a grid. That grid is made up of Rows and Columns. Rows run left and right, Columns run up and down. The little squares in the grid? They're called Cells. Each cell stores something. What is that something? It can be a header row, telling you what data is in each column. They can store words, numbers, dates, times, dollar figures and several other types of information.

Spreadsheets are also great calculators. But unlike your calculator you used in the past, this one harnesses your computer. To do that, you have to tell your computer that you're computing something. That starts with an equal sign. If your spreadsheet of choice, try this.

`=2+2`

The formula disappeared and you got 4, right? That's how spreadsheets work. It shows you the results of what you did. You can use any of the symbols from above and your spreadsheet will calculate them all.

##Mean##

#####The basics#####

Here's the thing about mean -- you probably already get it. It's the average. It's a measure of the middle. You've used averages your whole life. They're everywhere. 

But you may not know that average is just one measure of the middle -- what mathematicians call measures of central tendency. The others are the median (more on that later) and mode (which no one except mathematicians ever talks about).

Knowing when to use average and when to use median takes a little bit of thinking. Why? Because averages, by how they are calculated, are sensitive to extremes. What does this mean? Let's use an example. 

Let's pretend for a second that I'm taking a poll of a college class of 5 students on how much everyone makes per year. It's full of students, so the annual salaries are $8,000, $9,500, $7,200, $10,000 and $6,400. That makes the average annual income of these five students $8,220 (we'll talk about how to calculate the average in the next section). In our group of five students, given their incomes, $8,220 is pretty much in the middle. A student might make a little more, or a little less, but $8,220 is in the ballpark.

But I teach at the University of Nebraska. And we love us some football. And surprise! Head Coach Bo Pelini visits class. He makes $2.875 million. Per year. 

The average salary now? $486,016. And 67 cents. Who feels average now?

(This problem gets solved in a later section)

The above example, while a little silly, illustrates the point: Averages are sensitive to extremes. If you have a set of numbers that has no constraints -- there could be really big numbers or really small numbers in the mix -- then a mean probably isn't the number you're looking for. But when the numbers are constrained, or there aren't any extreme values in the set, averages work great. 

#####How to calculate a mean#####

How to calculate a mean is pretty simple: Take your numbers, add them up, and then divide them by the number of numbers you have. Let's take our previous example of the class of five and work through it step by step.

First, we need to add up the salaries in the class.

`8000 + 9500 + 7200 + 10000 + 6400 = 41100`

Then, we divide that 41100 by 5, the number of students in the class. 

`41100 / 5 = 8220`

Calculating the mean of a set of numbers is a very basic and simple way to measure the middle of the group. But be careful with sets of numbers

#####How to calculate a mean in a spreadsheet#####

The great part about spreadsheets is that they remove a lot of the drudgery that doing math by hand involves. Spreadsheets are smart enough to know how to do certain kinds of calculations given a set of numbers, so all you have to do is tell the spreadsheet you want to do that. 

Lets do that with an average. So open your spreadsheet of choice and lets type in the salaries of our mythical class. 

|In Excel|In Google Spreadsheets|
|--------|----------------------|
|![Means step 1 in Excel](images/excelmean1.png "Excel mean 1")|![Means step 1 in Google Spreadsheets](images/googlemean1.png "Google mean 1")|

In a spreadsheet, you *can* do the math yourself. You could, in A7, type `=(8000+9500+7200+10000+6400)/5` which would give you the average. 

But why do that? 

Typing is the devil. It's the devil because it's tedious. It's the devil because it's error prone. If I switch two numbers or type 5 instead of 6, I'm wrong. Once you have data, the less typing you do, the better.

In a spreadsheet, to calculate something with a set of numbers, you'll use something called a function. A function has a name, and takes inputs. If you're getting itchy, relax. Let's use the AVERAGE function in our spreadsheet of choice to illustrate this.

So first, remember that formulas is a spreadsheet start with an equal sign. 

The second thing you need to know is that you have to tell your spreadsheet where all your numbers are. You can do this one of two ways. First, you could name them all individually (A2, A3, A4, A5, A6) but that puts us back into typing-is-the-devil territory. And, what if you have a thousand numbers? That would be awful. So there's a second way -- use a colon. To tell your spreadsheet that you want a range of numbers, you tell it the starting number, colon, ending number. So, in our case, our range will look like A2:A6.

The third is that you call a function -- you tell your spreadsheet you want to use this particular function -- by putting the name of it first, then your inputs in parentheses. Like this: `=FUNCTION(inputs)`

So putting that all together, the format for the AVERAGE function is `=AVERAGE(A2:A6)`

|In Excel|In Google Spreadsheets|
|--------|----------------------|
|![Means screenshot 2 in Excel](images/excelmean2.png "Excel mean 2")|![Means screenshot 2 in Google Spreadsheets](images/googlemean2.png "Google mean 2")|

And, when we hit enter, we get our answer: $8,220.

#####How to turn a mean into a story#####

One of the main uses for an average is to compare how something fares against the middle. Is it above average or below average? And how much?

One thing you might want to do is compare your university's graduation rate compared to other schools like yours. For this example, I've provided a CSV file of schools in the Big 10 athletic conference (which, math alert, has 14 schools in it). If you'd like to get your own athletic conference, this data comes from the US federal Department of Educations [IPEDS](https://nces.ed.gov/ipeds/datacenter/Default.aspx) database. 

Question: What is the average graduation rate among Big 10 schools?

Opening the file in Excel is easy -- go to File > Open and find where you put the file. Open it and it'll come up as a new workbook.

In Google Spreadsheets, it's also easy, but not quite as straightforward. In Google Spreadsheets, open up a new spreadsheet, go to File > Import. There, you'll get a new screen. First, click Choose File and find the data file called colleges.csv in the data folder that came with this tutorial. Click replace spreadsheet (which means the blank sheet you opened up will be replaced with actual data) and then hit import.

|In Excel|In Google Spreadsheets|
|--------|----------------------|
|![Means screenshot 3 in Excel](images/excelmean3.png "Excel mean 3")|![Means screenshot 3 in Google Spreadsheets](images/googlemean3.png "Google mean 3")|
||![Means screenshot 4 in Google Spreadsheets](images/googlemean4.png "Google mean 4")|

    Pro Tip

    See how the data you just imported is cut off by the widths of the columns? Annoying, right? Here's how to fix that. See the rectangle to the left of column A and above row 1? Click it. That selects everything. Now, hover your mouse over the line between column A and B. See how it changed to something else? Double click that line. Boom. Automatically resizes every column to what's needed to show all the data. Much better now.

So you can see now we have five columns of data. A unit ID, the name of the institution, the cost of 30 credit hours -- or one academic year -- for in state students, that same cost for out-of-state students and the graduation rate of what's called the six-year cohort. That six-year cohort is the percent of students who had graduated who started six years before. That's the metric most universities look at to compare each other. 

So, from our last example, we know we can go to row 16 column E and work our AVERAGE magic. 

**Google spreadsheet users: You'll need to add a row to work with. There's a button at the bottom to just add 20 rows. That will work nicely.**

|In Excel|In Google Spreadsheets|
|--------|----------------------|
|![Means screenshot 5 in Excel](images/excelmean5.png "Excel mean 5")|![Means screenshot 5 in Google Spreadsheets](images/googlemean5.png "Google mean 2")|

And when we hit enter, we see that the Big 10 graduates 79.3 percent of students in six years. By eyeballing it, we can see some schools, like Northwestern, graduate nearly all of their students in six years. And, on the opposite end of the spectrum, we see the University of Nebraska-Lincoln, my employer, graduating only 65 percent of students in six years. 

Uh oh. 

So the first question that jumps out at you should be a very simple one: Why? 

Congratulations. You got your first story idea from data. But is eyeballing it the best way to look at this? Nope.

##Minimums, maximums and sorting##

#####The basics#####

#####How to calculate a minimum or maximum#####

#####How to calculate a minimum or maximum in a spreadsheet#####

#####How to turn a minimum or maximum into a story#####

##Median##

#####The basics#####

#####How to calculate a median#####

#####How to calculate a median in a spreadsheet#####

#####How to turn a median into a story#####

##Percentages of a whole##

#####The basics#####

#####How to calculate a percentage#####

#####How to calculate a percentage in a spreadsheet#####

#####How to turn a percentage into a story#####

##Percent change##

#####The basics#####

#####How to calculate a percent change#####

#####How to calculate a percent change in a spreadsheet#####

#####How to turn a percent change into a story#####


##Probability##

#####The basics#####

#####How to calculate a probabiity#####

#####How to calculate probability in a spreadsheet#####

#####How to turn a probability into a story#####

##Odds##

#####The basics#####

#####How to calculate odds#####

#####How to calculate odds in a spreadsheet#####

#####How to turn the odds into a story#####

##Equations of a line##

#####The basics#####

#####How to calculate slope and find the equation of a line#####

#####How to calculate slope and the equation of a line in a spreadsheet#####

#####How to turn the equation of a line into a story#####

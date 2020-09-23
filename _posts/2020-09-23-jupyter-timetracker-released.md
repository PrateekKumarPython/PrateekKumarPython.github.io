---
layout: post
title: "Created My First Python Package Ever : jupyter-timetracker"
categories: misc
---

# Backgroud and Philosophy behind these project

I had always obsessed about saving each and every second of my time in my life. More than just saving, I was more concerned about being able to look at where my time is going throughout the day. The led me to install so many time management app on my mobile, after a lot of trial and error, I found [atimelogger](http://www.atimelogger.com/) the best. It has all the capability what I was looking for. However, later it started to provide only basic features in free version and asking to pay to upgrade to have full features. Also, it has no desktop app. I found helpless in situations, where I am on desktop and away from my mobile. 
That led me to search for more productive and free apps that were both for mobile and desktop. Then i got to know about [toggl](https://toggl.com/) and [timecamp](https://www.timecamp.com/en/). However, these sites also provide very minimal features for free and require to pay for all features.  

As an introvert guy, I want to know deeply about myself ( self-introspection ). So apart from just logging time and having timesheet, I want to know detalied statistics about myself over a long period ( > 3 months ), which none of the time management tools available on internet were providing for free. This made me feel helpless and powerless. I want to make some new habits like reading books and I need a tool that records how much I was being able to read everyday.

Meanwhile, I was learning [pandas](https://pandas.pydata.org/) and [Jupyter Ipywidgets](https://ipywidgets.readthedocs.io/en/latest/). Suddenly, an idea came to my mind, it's better to learn these Python libraries by having a project in my mind. I already knew about [datetime](https://docs.python.org/3/library/datetime.html) in Python. So, I mentally draw a picture of making my own custom timesheet, save in compact pandas dataframe and make a front end User Interface using IPywidgets. It turns out to be a revolutionary idea and I was able to make this complete GUI in the 6 months of coding. It was a very nice and satisfying experience of being independent of any apps and tools and using my own code for my own benefits. I become very happy after making this. Each time i use it, i felt a kind of inner satisfaction that can't be described in words.

After using privately for a year, another idea came about wrapping this code into a open source python package and upload it on PyPI and GitHub so that other experienced programmers may add new features in it. Again, as an introvert and reserved guy, it took me more than a year to open source my code. So, recently I learned about packaging code and host it on PyPI and here is the [result](https://pypi.org/project/jupyter-timetracker/).  

# What is [jupyter-timetracker](https://pypi.org/project/jupyter-timetracker/) ?

`jupyter-timetracker` is a powerful python library to track, manage and analyse your time. The goal of this library to easily track your time spent in various activities and get to know more about yourself in a way that which activities you do most in a day. Also it can keep track of your daily activities for years, decades or so long. If you are too obsessive about utilising every single second of your life, it can keep track of each second of your life. Also, if you are lazy and want to track only 2-3 important activities, then you can do that also by entering those activities that matters to you.

## Main Features
Here are just a few of the things that timelog does vey well :
  - **Ease of use** : To use this library, you **need not require knowledge of any programming language**. Think of it as a software where you just have to click on a few buttons and your work is done. The user interface is very simple, easy to use and self explanatory.
  - **Can record your all activities involving time**, you don't have to worry about having a handwritten timesheet, habit tracker etc. Use this library in your own creative ways.
  - **Provison of Manual Entry** :If you forget to track your activity in real time, but your remember some activities of the past then you can also manuall eneter all of your past activities.
  - **Modifying past data** : You can always edit/insert/delete any of your time entries in the past
  - **Powerful Analysis** : You can analyse how you spent your time for a particular duration on a bar chart as well as in a time matrix form let you know that on which hours of day you do that activity.
  - **Know your History** : After months of time logging, you can always look at a particular date in the past and view all the time entries of it along with the totla duration of your each activity.
  - **Supports atimelogger csv reports** : If you have used *atimelogger* app in mobile for time tracking, you can import all of your *atimelogger* data in csv format in this app. 
  - **Synchronise to external drive** : You can also synchronise your data from your external hard drive or pen drive.  
  - **Backup** : To prevent data loss from external deletion or accidently replacing file, it will keep a back of your data by default on each of your time entry by a different name containing timestamp. You can later manually delete those backups if size become too high
  
In short, You will get a clear picture of how you spend your time in a day, in a week, in a month or in a year. If you want to write an autobiography or memoir in the future , this python library can be of immense help.

## Timesheet
Timesheet is basically the main database which has all records of your entered activities. It has 5 colums, Activity Name, From ( start time ), To ( Stop Time), Notes ( optional), Duration. Duration will automatically be calculated based on your start and stop time. You need only to select your activity from the drop down Menu and enter your start and stop time. Optionally, you can add your remarks/comments in the form of notes. Below is the screenshot of my own timesheet that I have been using since August 2019. Now as you can see my timesheet database has grown up in size having more than 10000 entries and still working fine.

![Timesheet](https://raw.githubusercontent.com/PrateekKumarPython/jupyter-timetracker/master/docs/static/images/Screenshot_2020-09-20_22-43-03.png)

**Note** : If you are working on your desktop, then you don't need to enter even start and stop time, you can go in *timer* tab, select an activity and click on *green* icon. It will take start time from your system's clock. When you finished your activity just click on *red* icon to stop as you can see in the above timesheet.

## Installation
1. Make sure that you have Installed Anaconda Python in your System.
2. run `pip install jupyter-timetracker` from anaconda command prompt or linux terminal
![Timesheet](https://raw.githubusercontent.com/PrateekKumarPython/jupyter-timetracker/master/docs/static/images/Screenshot0.png)


## To Run

1. Open Jupyter Notebook and create a new Python 3 Notebook

2. Run the following Lines  
        `import timetracker`  
        `timetracker.track()`

3. A widget shoud appear for manual entry. Manually enter your first time entry for example you can enter Time spent to install and run this libray)
![Timesheet](https://raw.githubusercontent.com/PrateekKumarPython/jupyter-timetracker/master/docs/static/images/Screenshot1.png)

4. Run the cell again by `Ctrl+Enter`

5. A new widget having multiple tabs should have opened (like shown below ). Now you can enjoy tracking your time.
![Timesheet](https://raw.githubusercontent.com/PrateekKumarPython/jupyter-timetracker/master/docs/static/images/Screenshot2.png)

The first 3 lines tell you the status about whether you have imported past csv report of *atimelogger* app. If you don't use that app, then you can safely ignore these notifications. 

Enjoy tracking your time.   

If you find any bug in this or you want to share your time tracking experience with me.You can always do that by mailing me at prateekongithib@gmail.com


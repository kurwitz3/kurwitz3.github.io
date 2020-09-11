---
layout: post
title:      "My  Mexican Dishes  Cli Project "
date:       2020-09-11 22:53:10 +0000
permalink:  my_mexican_dishes_cli_project
---


So before I started this project, I was feeling pretty confident about everything that we had learned leading up to this point. Then I went to start my project and saw the blank page and thought to myself, "Holy crap. What do I do?" After a few mintues of stressing out, I told myself, "You got this. Now let's get to work." 

So I started out by setting up my enviroment file along with a scraper file and a cli file. I did this because I knew that I was going to need these three no matter what I did because I knew I wanted to scrape a website instead of using an api. So after getting these files set up, I started my search for the website I was going to use to scrape my data from. This process turned out to be a little harder than I thought it was going to be. I searched 15 to 20 websites before I finally found the one that was structured the way I needed it to be. 

After using pry and making sure I was getting my dishes and recipes in an array properly, I decided to go ahead and set up a dishes class. I did this because I knew I was going to need to store this data in an array and use it in my cli class to be able to pass this data to the command line. So I set up my dishes class to initialize with a dish and a recipe. This way I would be able to access them seprately later on when I made my methods for the cli class. 

I also set up a class variable set to an empty array and then added it to my initialize method that way every new instance of dishes would be pushed into the array. Then I set up a class method ".all" that way I could use this array inside my other classes, and it would contain my data that I parsed from the website that I found. So after this, I went back to my scraper class to add in the Dishes.new(recipe,dish) into my scraper method. I used pry to see if the data was being passed into the "dishes.all array," and I kept getting an uninitialized constant error. For the life of me, I couldn't figure what was going on. 

I decided to go ahead and build the cli class and hopefully get things worked out. So I started building my methods for my command line and was getting the same errors. I built an array with made up data just to see if my methods were working properly, and they were. So this was my major road block in this whole project. I couldnt figure out why I was getting these errors. 

After hours of trying different things and searching google, I finally had to set up a one-on-one with my cohort lead, Corrina. She helped me to realize that not only did I forget to make a setter and getter for the data being passed by my array but I also forgot to call my scraper method inside my cli class. So my cli class wasn't even getting the data that I had scraped from the website that I had found. After making these changes, everything worked perfectly. 

I'm excited that we did this project because it helped me to understand more about how we make these separate files and classes work together. I understoood the concept of OO Ruby, but now I feel way more confident in my ability to put it into use. 

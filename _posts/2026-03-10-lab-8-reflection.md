---
layout: post
author: Clodagh
---

In this task, we were expected follow the [tutorial](https://learn.microsoft.com/en-us/aspnet/core/tutorials/razor-pages/razor-pages-start?view=aspnetcore-10.0&tabs=visual-studio-code) for RazorPagesMovies and use this to create a RazorPages website for a different data model.

## Links to Assignment

I decided to produce a model for books (each of which has a Title, Author, Genre, Publishing Date and IBSN number) and the code for my project can be viewed on my Github repository page [here](https://github.com/cnaspec/csci340lab8/tree/main/RazorPagesBooks).

Unfortunately, I am once again having issues with viewing the site on my Github Pages. Whilst it works on my local server and I was able to deploy the site, when I attempt to view it I get a 404 error. In the event I am able to get it working, the site should be able to be viewed at [https://cnaspec.github.io/csci340lab8/](https://cnaspec.github.io/csci340lab8/). (Although from the assignment wording it is unclear if I am supposed to be able to host it or just have it in a repository.)

## Reflections

### What were the easiest parts of the tutorial?

I feel that the first few stages (parts one to three) of the tutorial would have been the easiest if it hadn't been for issues downloading the packages - it was fairly easy to follow what was going on and the size of the project hadn't yet increased to the extent it was difficult to manage. I feel that overall the tutorial was clear and very instructive.

### What parts of the tutorial were confusing?

It was sometimes difficult to locate which file the tutorial wanted you to make changes to as many of the files had very similar names. On a related note, once you make a mistake it can be quite difficult to find and fix the error even if you are testing as you go along - which is why I initially had issue with the search function in Step 1 as I had not made the slight edit to a line that I thought I had. 

### What was difficult to translate when creating your own application in Step 2?

I didn't find it particularly difficult to translate the information from the tutorial because books aren't entirely dissimilar from movies, but I made changes from the start which may have helped. I think it would have been a bad idea to create a Movies database as per the tutorial and then have to adapt it to something else. Since people often have authors' whose writing they prefer, I added an additional search bar so that the database can be searched by book genre, title and author.

One thing that I did find difficult was the validation for the IBSN number as IBSN values are either 10 or 13 digits long. I initially struggled because I had it as a numerical datatype, but it was much easier to find a solution when I changed it to a string and used RegularExpression for validation instead.

### What parallels and differences do you see between the Jekyll framework and the Razor framework?

They both provide structured templates to reduce the heavy lifting required to create a more complex application, and "modulise" sections by grouping files together to help make it easier for people with less familiarity with programming to alter them to suit their purposes. However, the intended user has different goals/purposes for each application and so they diverge in what they are intended to do. They both make use of css files and javascript for core functions, but Jekyll uses yaml as well whilst Razor doesn't seem to. This is possible related to the intended purposes (blog vs. database).

### How confident do you feel making another Razor application?

On a local server, fairly confident. I don't think I had many problems with structuring the Razor application itself. Otherwise not very, as I seem to constantly have issues with Github.



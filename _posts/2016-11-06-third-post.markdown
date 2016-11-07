---
layout: post
title:  "Working With Data"
date:   2016-11-06 
categories:
---
<div style="text-align:center"><img src ="https://66.media.tumblr.com/0041c9bf85bd680c7a8595a21fd58bf0/tumblr_og8p9i4k1v1tpp2lco1_500.gif"/></div>

<br>
For assignment 4, I was able to work a little more with scripting, specifically a script that involves handling data. Also, since we had to work in groups, this assignment gave me some insight on using github and cloud9 as a collaboration tool. 

The repository containing the script we wrote can be found [here][repo], and the script can be found [here][script]. 

[repo]: https://github.com/gma96/braid-assignment-4
[script]: https://github.com/gma96/braid-assignment-4/blob/master/script.sh

The script asks the user five questions using `echo` and saves each answer in a separate variable using `read`. After the user answers all of the questions, the script assigns the user a unique identifier, which is a string that consists of a combination of 6 characters, varying from upper case letters A-Z, lower case letters a-z, and digits 0-9. Next, the script determines the date in which the user answered the questions and assigns the date to a variable. Lastly, all of the answers, the unique ID, and the date are appended to a csv file using `echo` and `>>`. Each time the script is executed, the new data gets copied to a new line in the csv file while keeping all data from previous executions in the file as well. 

While completing this assignment, my group and I first attempted to each create the script on our own since there were different methods that could be used to successfuly complete the task, and each person has their own preferred strategy of figuring things out. After a little while of independent brainstorming, we eventually put our ideas together and created a working script. 

Overall, we didn't run into too many issues while completing this assignment. The question and answer portion was easy because it involved concepts that we went over and practiced in class. We weren't completely sure how to add the unique ID and date or how to append the data to a csv file, but after some google searching, we were able to successfully complete these tasks. Also, a common issue we ran into was that someone would try to push to github and would receive an error, but this was generally fixed if we pulled before pushing and could be avoided with good communication skills. 


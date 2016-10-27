---
layout: post
title:  "A First Look at Scripting"
date:   2016-10-26 
categories:
---

For assignment 3, I was able to work with scripting for the first time. The script I wrote and worked with involves using pandoc to convert a markdown file to different formats, including html, docx, odt, and pdf. The markdown file I used was the reflection post from the second assignment (the first post on this website) but with a couple of added changes to fit the requirements of assignment 3. I changed some of the pictures, added a table, and included smart quotes to the text of the file. 

In order to convert the markdown file into different formats, a software called [Pandoc][pandoc] has to be used. First, the user has to input the name of the file that they want converted. After this has been done, the syntax of converting into different formats is generally the same, no matter what format the file was being converted into. This general syntax is shown below.

{% highlight ruby %}
pandoc -o FILENAME.{new format} --smart FILENAME.{original format}
{% endhighlight %}

For example, if you wanted to convert a **markdown** file named **writing** into a **docx** file, the command would be as follows: 

{% highlight ruby %}
pandoc -o WRITING.docx --smart WRITING.md
{% endhighlight %}

The **-o** flag creates a new output file with the new format and the **--smart** flag converts all punctuation in the new document into smart punctuation. 

A list of all the files used for assignment 3 with links is provided below. 

- Script
    - gma96-convert-docs.sh --- [ [link][script] ]
- Files
    - SampleWriting.md ---[ [link][md] ]
    - SampleWriting.html ---[ [link][html] ]
    - SampleWriting.docx ---[ [link][docx] ]
    - SampleWriting.odt --- [ [link][odt] ]
    - SampleWriting.pdf --- [ [link][pdf] ]

Overall, assignment 3 wasnn't too difficult to complete. Scripting kind of reminded me of programming, which I have a some experience with from other classes, so that familiarity probably contributed to why I was able to complete this assignment with minimal errors. Also, since the syntax for converting files was generally the same no matter what the file types were, it made the script fairly easy to write because there was a lot of repitition. The only issue I had was converting normal punctuation into smart punctuation because I had no idea what smart punctuation was, but after some google searching and some further explanation in class, I was easily able to figure out how to implement smart punctuation into the different files. Although this assignment involved a fairly simple script, I know there is a lot more that can be done with scripting, and maybe in the future I will look a little further into writing scripts and the different more complicated things that can be done with them. 

<!--- LINKS -->
[pandoc]: http://pandoc.org/
[script]: https://github.com/inls161/assignment-3-gma96/blob/master/gma96-convert-docs.sh
[md]: https://github.com/inls161/assignment-3-gma96/blob/master/SampleWriting.md
[html]: https://github.com/inls161/assignment-3-gma96/blob/master/SampleWriting.html
[docx]: https://github.com/inls161/assignment-3-gma96/blob/master/SampleWriting.docx
[odt]: https://github.com/inls161/assignment-3-gma96/blob/master/SampleWriting.odt
[pdf]: https://github.com/inls161/assignment-3-gma96/blob/master/SampleWriting.pdf
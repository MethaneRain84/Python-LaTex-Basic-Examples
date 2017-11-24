# Python-LaTex-Basic-Examples
### With all the new updates and a new laptop I needed to do a couple of steps to be able to convert my jupyter .ipynb notebooks to either pdf or tex files (they work on the same process). 

### First off I needed to install homebrew installer: (command line)
### $/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

### Next we need Pandocs: 
### $brew install pandoc

### Then MacTex to convert to LaTex:
### I went to http://tug.org/mactex/

#### So the latest problem I have noticed with my weather notebooks was that when I tried to convert the .ipynb notebooks to either LaTex or pdf one of my noetbooks was just not working when others were converting nicely.

#### A basic intro: I was using jupyter notebooks through Anaconda and using nbconvert after downlowding the pandoc and MacTex libraries (I'm using Mac OSx).

#### The notebook converted the beginning but only saved a pdf upto a certain point. I was totally lost because I had an almost identical noetnbook that converted no problem. So I saved the notebook to a .tex file and opened it in the TexShop app. Running the code (typset button), it would not bring up a wkrking copy of the pdf. It did indicate an error for me and a place to locate it. Another shitty problem was the error line in question was identical to a line elsewhere in the code so I wasn't even looking at the correct code. Long story short I was able to sift through the LaTex code and actually locate the code block that was causing the problems.

#### The final resolution was that in my specific notebook I had some Raw NBConvert cells. Now that I write this the error totally makes sense. Regardless of hindsight, I have narrowed down my specific problem!!

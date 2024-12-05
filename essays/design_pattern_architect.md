---
layout: essay
type: essay
title: "Design Pattern Architect"
# All dates must be YYYY-MM-DD format!
date: 2024-12-04
published: true
labels:
  - Design Patterns
  - Problem Solving
  - Software Development
---

<img width="300px" class="rounded float-start pe-4" src="../img/man-are-working-as-architecture-construction-company_81761-404.png"> 

## Having an Architect

Imagine being tasked with building a house. Growing up as a daughter of a carpenter, I've watched and helped with the building of around 10 houses. The foundation must be level and sturdy, the plumbing and water ways functional and efficient, and the layout optimized for accessibility. Without guidance, there might be a leaky roof or creaky floors. This is where being and achitect and having a blueprint comes in handy: proven templates for solving common design problems. In the realm of software development, design patterns are the blueprints.

Design patterns provide structured solutions to recurring issues in software design. These are not lines of code to be copied and pasted, but rather conceptual frameworks that developers can use to adapt to their needs. Like the idea of a house floor plan, this allows for software to be flexible, scalable, and easy to maintain. 

## Being the Architect

In one of my classes a year ago, I was tasked with creating a simple, centralized logging system that all parts of the application could access. I chose to implement the Singleton pattern where one instance of the logger exists across the application. 

```
class Logger:
  _instance = None

  def new(cls,*args,**kwargs):
    if not cls._instance:
      cls._instance=super(Logger,cls).new(cls,*args,**kwargs)
    return cls._instance

  def log(self,message):
    print(f"[LOG]: {message}")

logger1 = Logger()
logger2 = Logger()

print(logger1 is logger2) #should output True
```

While the heading of his question could be better, it does convey what he’s trying to figure out. Usually something as brief as “python date of previous month” is what other users would enter in as search terms on Google, making it easily found. Another good thing about the question is that it’s not just a question. The asker shows what he or she has done and that he or she has put in some effort to answer the question. And while it may not be as important as the question itself, the asker shows courtesy, which does increase the chance of getting an answer.

```
A: datetime and the datetime.timedelta classes are your friend.

1. find today
2. use that to find the first day of this month.
3. use timedelta to backup a single day, to the last day of the previous month.
4. print the YYYYMM string you're looking for.

Like this:

 >>> import datetime
 >>> today = datetime.date.today()
 >>> first = datetime.date(day=1, month=today.month, year=today.year)
 >>> lastMonth = first - datetime.timedelta(days=1)
 >>> print lastMonth.strftime("%Y%m")
 201202
 >>>

```
 
The asker received six possible answers, and he or she was successful in inciting discussion from multiple users. The answers themselves were clear and were devoid of the rumored sarcasm and hostility of “hackers.” Since I myself have referenced this page and found it useful, I can confidently say that it is a good question.

## Conclusion

When we rely on others’ generosity and expertise to provide answers to our questions, it should hold that the question we ask should be one that leads to efficient and effective help that not only benefits us, but also the people we ask and others who might ask the same question in the future. Thus, if you have a question… make it a smart one! Asking questions may not always get you the best answer, but asking them in a way that will make others want to answer them will increase the success of finding a good solution and make it a positive experience on all sides.

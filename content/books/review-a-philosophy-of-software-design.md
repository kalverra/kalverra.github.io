---
title: "Review: A Philosophy of Software Design"
date: 2023-05-07
draft: false
categories: ["books"]
tags: ["software design", "review"]
description: A review/summary of the book A Philosophy of Software Design.
summary: A review/summary of the book A Philosophy of Software Design.
---

[A Philosophy of Software Design by John Ousterhout](https://www.goodreads.com/en/book/show/39996759) is a wide ranging, highly opinionated look at general software design practices and how to best implement them. It vacillates from big-picture musings on "The Nature of Complexity", down to seemingly miniscule squabbles around "Choosing Names" for variables and methods.

## The Author

[John Ousterhout](https://web.stanford.edu/~ouster/cgi-bin/home.php) is a computer scientist who got his PhD from Carnegie Mellon, did some cool research work, bounced around the industry a bit, and has settled back into academia as a faculty member at Stanford where he regularly teaches courses on software design. He claims teaching this course is what gave him most of his inspiration and material in writing the book. He also thanks a group of people for their help in the book, including [Rob Pike](https://en.wikipedia.org/wiki/Rob_Pike) and [James Koppel](https://www.jameskoppel.com/).

## The Book

Broken down into highly structured and compact chapters, Ousterhout touches on what he considers the most crucial considerations for writing modern software. He starts out by ultimately declaring complexity to be an enemy of the state of software, and anytime you find yourself writing complex code, you need to take a good look at what has led you down this demonic path.

> The most fundamental problem in computer science is problem decomposition: how to take a complex problem and divide it up into pieces that can be solved independently [...] we must find ways to make software simpler. Complexity will still increase over time, in spite of our best efforts, but simpler designs allow us to build larger and more powerful systems before complexity becomes overwhelming.

This problem remains prevalent no matter how much sheer willpower we have thrown at it as an industry. It seems that CS is often the *practice* of independent problem solving, rather than its antagonist. Framing this as a "problem" strikes me as odd in the same way if someone told me that 'math would be perfect if it weren't for all these pesky equations'. I'm getting bogged down in semantics here, the ultimate idea is that intertwined systems lead to complexity, and complexity ultimately leads to bugs, frustration, and screaming at my computer like a lunatic when it keeps printing `a` despite me *clearly* telling it to print `b`. Ousterhout spends the rest of the book detailing what he means by complexity, then delving into the strategies to avoid it. Each chapter details one of these strategies, providing a handy summary at the end of each one, and some red flags to watch for when you can likely implement a specific strategy to remove complexity from your design.

> Every rule has its exceptions, and every principle has its limits. If you take any design idea to its extreme, you will probably end up in a bad place. Beautiful designs reflect a balance between competing ideas and approaches.

The book is staunchly opinionated on design approaches, what types of problems to focus on, and how to fix them. But it consistently warns that taking any solution to the extreme will ultimately lead you back into the clutches of complexity. And what exactly is complexity?

> Complexity is anything related to the structure of a software system that makes it hard to understand and modify the system. Complexity can take many forms. For example, it might be hard to understand how a piece of code works; it might take a lot of effort to implement a small improvement, or it might not be clear which parts of the system must be modified to make the improvement
> 
> The first symptom of complexity is that a seemingly simple change requires code modifications in many different places.
>
> The second symptom of complexity is cognitive load, which refers to how much a developer needs to know in order to complete a task.
>
> The third symptom of complexity is that it is not obvious which pieces of code must be modified to complete a task, or what information a developer must have to carry out the task successfully.
>
> Of the three manifestations of complexity, unknown unknowns are the worst. An unknown unknown means that there is something you need to know, but there is no way for you to find out what it is, or even whether there is an issue.

Complexity itself is defined rather amorphously; it's largely left to "you know it when you see it". Which is fine for me. I've rarely found myself disagreeing with someone about whether some code is complex or not. Conflict usually begins when we start asking pesky questions like "how do we make it simpler?". This question is what Ousterhout spends the majority of the book answering.

I won't detail all of his suggestions here (take a look at the Table of Contents for a good idea), but I found his focus on comments and naming (5 of the 22 chapters) intriguing, mostly because I've found myself to be more focused on this aspect than nearly all of my colleagues, and often took that focus as a sign of me being somehow inferior as a programmer; that I couldn't magically divine what the code is doing showed that I was somehow deficient. It turns out that Ousterhout agrees with me that this is something to focus heavily on, and can really help everyone. Some of his advice includes **starting your method by writing the comment** then work on the implementation, taking care to update the comments as you make changes to the original design. This can be annoying &mdash; especially as you make lots of changes in need of documenting &mdash; but forces you to at least write *something*, where most people never bother going that far.

My only real criticism of the book is the same I have for all programming books: its reliance on toy problems. Toy problems are a necessity for this stuff. You can't just say "my example is Kubernetes, go read it", I need digestible problems to learn your lessons from. For the concrete problems and solutions Ousterhout focuses on, this use of toy problems makes even more sense, but so often I find that simplifying the issue often trivializes the solution. So applying some of the toy code advice to a situation where I actually am working on code as large and complex as Kubernetes becomes tricky.

You can see this in another light though, as Ousterhout continually mentions that the complexity we most often encounter is rarely a symptom of overall design, but rather is added in small increments over the years, until you find yourself staring at a 50 layer `if-else` garbage pile. Just like no one looks like Arnold Schwarzenegger after a couple days in the gym, and Schwarzenegger doesn't gain 50 pounds of fat after eating a bag of chips, these large transitions usually take time. It's those little decisions, like choosing to comment your code, spend a little more investment on a simpler design, focusing on more-frequent use cases on that one method, those little acts of care add up to reduce overall complexity as long as you consistently adhere to their underlying philosophy.

## The Takeaways

The book is excellent. I found myself silently nodding to myself as I read over written forms of lessons I had long ago internalized in my experience of writing software. I wish I had read it sooner, and I think that if you're a college senior embarking on your career &mdash; or have been working for a few years &mdash; this book is ideal. Here's a scattering of key quotes and takeaways I felt to be poignant.

> it’s worth taking a little extra time to find a simple design for each new class; rather than implementing the first idea that comes to mind, try a couple of alternative designs and pick the cleanest one. Try to imagine a few ways in which the system might need to be changed in the future and make sure that will be easy with your design.

I find this can sometimes paralyze me with decision paralysis though. Best to not be taken to the extreme.

> interfaces should be designed to make the common case as simple as possible

An opinionated book recommends you use an opinionated design. Though sometimes it's tricky to predict just how exactly people will use your code.

> Information leakage is one of the most important red flags in software design. One of the best skills you can learn as a software designer is a high level of sensitivity to information leakage. If you encounter information leakage between classes, ask yourself “How can I reorganize these classes so that this particular piece of knowledge only affects a single class?”

> I have found over and over that specialization leads to complexity; I now think that over-specialization may be the single greatest cause of complexity in software. Conversely, code that is more general-purpose is simpler, cleaner, and easier to understand.

> I have noticed that the design-it-twice principle is sometimes hard for really smart people to embrace. When they are growing up, smart people discover that their first quick idea about any problem is sufficient for a good grade; there is no need to consider a second or third possibility. This tends to result in bad work habits. However, as these people get older, they get promoted into environments with harder and harder problems. Eventually, everyone reaches a point where your first ideas are no longer good enough; if you want to get really great results, you have to consider a second possibility, or perhaps a third, no matter how smart you are. The design of large software systems falls in this category: no-one is good enough to get it right with their first try.

> If you want to maintain a clean design for a system, you must take a strategic approach when modifying existing code. Ideally, when you have finished with each change, the system will have the structure it would have had if you had designed it from the start with that change in mind.

I love this idea, but it's hard to focus on when this change is blocking 5 different teams that need it now.

> Don’t change existing conventions. Resist the urge to “improve” on existing conventions. Having a “better idea” is not a sufficient excuse to introduce inconsistencies. Your new idea may indeed be better, but the value of consistency over inconsistency is almost always greater than the value of one approach over another.

Consistency == Readability

> Programmers’ intuitions about performance are unreliable. This is true even for experienced developers. If you start making changes based on intuition, you’ll waste time on things that don’t actually improve performance, and you’ll probably make the system more complicated in the process.

Design it, then measure it to find out where you fucked up.

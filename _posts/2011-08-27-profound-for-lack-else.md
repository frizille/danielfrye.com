---
id: 87
title: Something profound (for lack of anything else)
date: 2011-08-27T22:48:20+00:00
author: Daniel
layout: post
guid: http://danielfrye.com/?p=87
permalink: /2011/08/27/profound-for-lack-else/
categories:
  - Ramblings
tags:
  - life
  - memories
  - philosophy
---
I&#8217;ve been sitting here for a bit, listening to some music with this feeling I need to write&#8230; something. No idea what, I just want to write. Something profound, meaningful, I don&#8217;t know&#8230; something. So as I was sitting here I saw a picture of a bunny rabbit (yes, I got sidetracked on the writing thing and hit [the lolcats site](http://icanhascheezburger.com/)) and was reminded of the [Fibonacci sequence](http://en.wikipedia.org/wiki/Fibonacci_number). And when I think of Fibonacci, I think of my first programming class in Pascal.

**_So with that intro&#8230; I present Programming in Pascal 101._**

In high school, I took a class in Pascal, the only computer class offered other than Introduction to Keyboarding. Blah. If you can’t figure out how to use a keyboard in sixteen weeks, you frankly have no right existing on this earth. End of story. When school started up in the fall of my senior year, those of us who looked, noticed a class labeled “Programming” on the last line, of the last page, of our school computer class list. All of the geeks quickly signed up (I was obviously one such individual). This class became the focal point in my high school day. To sit down at a computer and create something that I had complete and total control to do was awe inspiring at the age of 17. The only limit of my ability to create was my own imagination.

I remember the very first program we had to write. It was a simple “Hello World” program that asked for our name, age, and weight then printed all the information back to the screen. Except I had this idea. I don’t know where it even came from, I just all of a sudden knew. If I added a boundary for the name, then did an “If&#8230;then” statement I could customize the output screen. Revolutionary. I was proud of myself and after making the necessary changes to my program I copied the source code over to the floppy disk and scooted my chair over to my friend Brent’s desk.

“Take a peak at this”, I said to him.  
“Why?”  
“Just do it. It’s cool.”  
“Ok, fine.”

So he put this disk in, brought up the source code, compiled it, and then hit the Run command. It popped up the name, age, and weight prompts. He put in all his information like normal and after he hit the return key to get the print out, he got the message “I’m sorry you’re a dork” plus the normal name, age, and weight that he had entered. I just smiled; that cocky half grin I sport occasionally.

“Ok, that was stupid.”  
“Yeah, but it was funny.”  
“No, it was stupid.”  
“Ok, fine, just do it again. And don’t enter in Brent.”  
“I’m gonna enter in Stupid, just for you”.  
“Fine”.

My smile steadily grew as he worked his way through the prompts. When the print out came back, he saw a new message, “Stupid is the best person in the world”. His puzzled look as he worked his way back through the prompts again was priceless. Again he put in Stupid for the name, and again he was told “Stupid is the best person in the world”. As we started getting more creative improving the logic, we attracted the attention of our side of the room. They crowded around his screen watching him put in the prompts and trying different names, ages, and weights &#8211; all with different logic. Everyone was in awe. Finally, after several requests to do so, we showed them what we had done and the syntax for an “If…then” statement in Pascal. Immediately, everyone jumped back to their desks, in an effort to expand on what we had done. It was the biggest sense of pride I had ever felt in high school. Mrs. Brown, our teacher, talked to me sometime later that week, asking how I knew about the “If…then” statements since we hadn’t covered those yet. I told her I didn’t read ahead in the book and wasn’t sure where I had picked it up from. I just knew there was this thing called an “If…then” statement that could do some cool things. I guess she understood, as she left it at that. Thinking back, I&#8217;m pretty sure I picked it up from my IBM Basic 3.0 programming manual, circa 1982, that ironically is behind me on my office bookshelf as I&#8217;m writing this, I still have it after all these years _(by the way, mom, in the event I get hit by a bus or something there is a micro-SD card in there with my will and stuff on it)_.

As the school semester began to draw to a close several weeks later, Mrs. Brown pulled me aside from everyone else. I had been done with all the required programs for a week and spent all my class time using the compiler to build some program that did whatever I could think of or helping her grade the other students programs. I, of course, was feeling pretty cocky. I was done for the most part, in fact, I was pretty much just hanging out for the rest of the semester. I had already done all the assigned programs as well as the final program which was designed to be a crucible of sorts. At the end of the quarter, rather than do a final, we had a massive programming assignment, one that would take several weeks to finish and was designed to be as complex as possible. Regardless, we all had pretty much gotten an A in the course. It wasn’t like the class was hard or anything. We did the programs as needed and turned them in. If someone was having problems understanding a concept, it was drilled into them by the rest of us, and with most of the (ok, all of the) high school level computer intellect in one room there wasn&#8217;t much we couldn&#8217;t cooperatively solve. All for one, and one for all. Pretty simple concept.

“Daniel, I have a different program for you.”  
“Uh. Ok, I guess.”  
“Good, it’s on this disk. Just open the files on there and read through it. If you have any questions, come find me and I’ll help you out.”  
“Ok.”

So I walked back to my desk, put in the disk, and opened up the file she had typed all the instructions in. I was enthralled. I had to write a program to print the Fibonacci numbers. 0, 1, 1, 2, 3, 5, 8, 13, 21, etc, up to anything greater then 100.

A little background on Fibonacci. He developed this theory of numbers to count the reproduction cycle of a family of rabbits. You start with one rabbit, then he reproduces to get another rabbit so now you have two rabbits. I was always unclear on this. It seems to me it’s hard to reproduce with only one rabbit, but I’m not a rabbit so I wouldn’t know _(Editorial note: So I looked up Fibonacci when I was gathering links for this article and it was a pair of rabbits, not just a rabbit. It makes sense now&#8230; I&#8217;m still not a rabbit)_.

Well, the two rabbits reproduce to get three rabbits. You probably see the pattern now. The first slot gets added to the second slot to get the third number. The second slot gets added to the third slot to get the fourth number. Three plus four gets you the fifth slot. And on down the line, until you hit one hundred. Well, I got the pattern, but for the life of me I couldn’t figure out how the hell to get the computer to take the damn numbers and then reuse them in the next calculation. I tried every kind of loop out there. If, for, “do … while”, “repeat…until”. Nothing worked. I was stumped. I went and asked Mrs. Brown about it. She told me, yes I was on the right track, but no, she wasn’t going to help me. The “see me for help” speech was only applicable for the correct pattern in the numbers. The coding part was up to me. So for weeks I tried to figure out the right loop. I built the menu system and the screen formats and all the other input / output procedures. But I could never ever get the numbers to add right. I could do the first numbers or the last numbers but could not get the whole thing to run.

Finally school ended for the semester and the class was over. My program still didn’t work. I still got my ‘A’ in the class and I mentioned to Mrs. Brown that I was disappointed in not being able to figure it out.

She said to me, “Daniel, you weren’t supposed to figure it out.”

My glazed blank expression stared back at her.

“You’ll understand someday and it will all make sense. But if you really want to figure out the program, try using a nested loop. And you did well, you didn’t give up.”

Two years later, when I was taking CS1502 “Application Programming in Pascal” during my freshman year at Georgia Tech, I got assigned the same problem. Word for word. She must have got her problem from the same text book they used at Tech for second semester CS majors. Needless to say, that was the easiest program I ever did there. But more importantly I learned two very valuable lessons from the Fibonacci numbers.

**One:** Don’t think you know it all because when it comes down to it, you don’t.  
**Two:** Don’t ever give up.

So that&#8217;s my message for the day. It isn&#8217;t as profound as some of my other posts, but sometimes we just need to hear the basics one more time.

Daniel
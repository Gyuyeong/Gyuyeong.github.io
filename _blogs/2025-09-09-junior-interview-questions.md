---
layout: single
title: "Frequently Asked Junior Software Engineer Interview Questions"
date: 2025-09-09
---
Before I begin, thank you for all the companies that saw my resume and decided give me a chance to prove myself in the interview.

In the year 2025, I had interviews from 6 different companies as a junior software engineer. While all the interviews were unique, some questions were commonly asked and I want to share some of them. Here we go.

# 1. Process vs Thread
All the interviewers asked me this at least once. Some companies asked me this multiple times during different phases of the process. I think the reason they ask you this question specifically is because this is probably the one thing CS graduates will know if they took their classes seriously. It also makes sense to ask CS related questions since it is obvious that juniors will not have that many in-depth working experience. The following is a table that I have in my head to explain the difference between them:

||Process|Thread|
|:---|:---|:---|
|What?|An independent program|A small unit that can execute code|
|In terms of memory|A process has a separate virtual memory space. It has its own stack, heap, and program counter.|All threads share one heap and global region (that of the caller). Each thread maintains separate stack and program counter.|
|Context Switching|Must switch everything, heavy|Only switch stack and program counter part, which is much faster than switching everything.|
|Usage|When running different programs. For example, when we run a game, it can have one process render visuals on the screen, and another process receive keyboard inputs.|When there is a single function that processes a large amount of data, you separate the data into smaller chunks and each thread deals with each of them. In short, multiple threads do the same thing on different chunks.|
|How to use them?|C: fork()|C: pthread, Openmp|

## 1-1. Locks
Some interviewers asked about locks as a followup question, which is very reasonable since multithreaded programming requires locks to safely process globally shared resources. They also asked what deadlocks are, so having a firm understanding of OS concepts and doing some practical assignments in system programming really helped out.

# 2. Projects
While I cannot recall everything questions that were asked to me, here are some of them:
- What was the project about?
- Why did you participate or start the project?
- What was your role?
- What did you do?
- What did you use? (tech stacks, methodology, etc.)
- Tell me about some frustrating experience during that period of time and how you overcame them.
- Did you eventually make it work? If so, why? and vice versa.
- Who was in your team? How did you collaborate?
- Tell me about some events that happened with your teammate(s) that was challenging.
Some companies alloted nearly 2 hours for this section, and I honestly felt kind of squeezed out. At first, I explain to them what this project is all about, what my role was and my contributions. Afterwards, it was always one of the following (in my case):
- Questions regarding the tools you've used in the project. They really wanted to see whether you did some research about the things you've used during the project. For example, if you used a certain database, they ask you some unique traits of that particular database. In my case, it was Hana DB (since I was working at SAP as an intern), and they immediately asked some traits of Hana DB. I honestly felt embarrassed to not be able to recall on site that Hana DB was an in-memory database.
- Some CS related questions. I mostly used Python for projects and they immediately asked me what object-oriented programming was. When I talked about the things I did with the database, they asked me about basic concepts of DB, such as what rows and columns mean, what is a primary key and a foreign key, what is an index and how are they implemented, and etc.
- Motivations behind the project. The interviewers really wanted to know this. I might be wrong, but I think this was important to them because they wanted to see who I really am. Some people can start a project because everyone else does it. Some people may start a project with a clear intention.
Overall, I spent most of the time trying to organize and recall what I did during every projects I have done to be as confident as possible in front of the interviewers and I think that really helped out.

# 3. Why This Company?
Since there are so many companies out there, it is no surprise that they will ask you this question. Some companies asked me this question in all the interview phases. These are the things that I did that really helped me out:
- Find what the CEO says in social media. Most companies had their own LinkedIn account and blogs. In there, I looked through what the CEO said, since that is what that company's goal is going to be. Afterwards, I thought about how **I** can be in line with those words. Looking back, the more I was able to relate myself to the CEO, the further I was able to proceed in the interview process.
- Read the job post over and over again. The job post clearly has all the information in regards to what I should bring to them. As I read through many job posts, I kind of realized that every company wants something different. Some companies wanted you to be good at certain tech stack, while others wanted you to be good with your CS basics as a junior. My goal was to emphasize how fit I am according to their job description and that really paid off.

# 4. Explain Anything You Are Confident With
They ask you to choose anything that you are very familiar with and elaborate as much as possible. I think they ask you this because they want to know how much you can dive deep into a certain topic or problem. Before an interview, you should pick something technical that you can explain as much as possible.

# 5. Culture-Fit Question
They wanted to know whether you would be fit for the company. Since everything is essentially teamwork, these are some of the questions that I have encountered:
- How would you persuade others?
- If A and B cannot agree on certain things, what would you do?
- If you find out you cannot finish your work on time no matter what, what will you do?
I think nobody will have an exactly same take on these types of questions, but it is worth thinking about them before you go in.

Overall, it was a harsh experience. I was asked many questions in a long period of time and it exhausted my brain and energy. However, in the end, it was a great learning experience in that I was able to know what people in the industry wanted from the candidates. I am very thankful that I have been successfully hired in one of the companies and I thank everyone that led me throughout my lifetime.
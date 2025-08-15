# First-Bounty


## Introduction

> [!Note]
> The goal of this guide is to take someone from zero knowledge in bug bounties and web application security to earning their first bounty (monetary reward).


A lot of people ask me how to get started in bug bounties. Most of them are lost and overwhelmed by the endless list of resources out there.

I think there are two main problems with most of those resources:

- They forget that the reader is a beginner who just wants a clear starting point  
- They believe that adding more tools, links, and buzzwords makes their guide more valuable

I want to address those issues.

One thing to keep in mind is that everyone thinks differently. People have different learning styles and approaches, so you might come across other roadmaps or advice that suggest a different path. That’s totally normal.

What you're going to read below is based on my ([@Behi_Sec](https://x.com/Behi_Sec)) personal experience of over 4 years as a part-time bug hunter.

When I started, I had to learn everything by trial and error. I wasted weeks going in the wrong direction.

This repo is my way of helping you skip the guesswork and build a strong foundation. Once you've got the basics down, leveling up will be way easier.




## 🌐 1. Web Fundamentals

What separates someone making $250K a year in bug bounties from someone who can’t even find a valid bug is **knowledge**. 
The more you know, the better you’ll perform.

If you’re going to hack web apps, it really helps to understand how modern web applications are built and how they work.

For this first phase, I’m not going to hand you direct resources.

Why? Because this approach will help you build long-term, high-value skills:

- Problem-solving on your own  
- The ability to explore and learn new skills  
- Patience

The only hint I’ll give you is this: search on Google or ask ChatGPT.



**Path for Learning Web Fundamentals:**

1. **HTML & CSS Basics**  
   - Understand how web pages are structured and styled.

2. **JavaScript Fundamentals**  
   JavaScript is the programming language of the web. Learn the basics like variables, functions, and events, it’s key for finding bugs such as XSS.
   - The more JavaScript you learn, the more opportunities you’ll have. It will definitely pay off in the long run. 
   - For example, [this hunter](https://x.com/samm0uda) only hunts client-side bugs, yet has earned over $3M in bug bounties. 


3. **React.js Core Concepts**  
   React is a JavaScript framework for building dynamic UIs. Learning its basics will help you understand how data flows in modern apps, identify client-side vulnerabilities, and test component behavior effectively.
   - Understand components, props, state, and how data flows in a React app.

4. **Next.js Fundamentals**  
   Next.js is a React-based framework for full-stack apps that combines frontend and backend capabilities in one project.
   It supports features like server-side rendering, API routes, and file-based routing, making it very useful for understanding how modern web apps work.
   
   Focus on understanding routing, server components, and file-based architecture.  
   Make sure you learn these three areas well:  

    - **Authentication systems:** How cookies, JWT, and OAuth work
    - **Databases:** How to store, query, and manage data using SQL  
    - **APIs:** How to request, retrieve, and send data to APIs. Use tools like [Postman](https://www.postman.com/) and learn HTTP basics


## 🐞 2. Vulnerabilities

After learning how web apps are built and how they work, breaking into them will be much easier.

In this section, we'll focus on learning the bug types you're most likely to run into in bug bounty programs.

To learn a bug type well, we'll follow this process:

1. Study the basics of the vulnerability  
2. Practice what you’ve learned to fully cement your understanding of the basics.
3. Read real bug bounty writeups to understand:
   - How others are finding this type of bug  
   - Where it's most likely to exist  
   - How it's exploited  
   - What the real-world impact looks like 

> [!Note]  
> Most of the challenges and CTFs you’ll solve will be much easier than finding the same kind of bug on a real target. That’s because modern web apps have more protections in place, and many other bug hunters may have already tested the same areas.

> [!Tip]  
> In many writeups, you’ll come across chains of multiple vulnerabilities. If you see a bug you haven’t studied yet, don’t worry, you’ll get to it later. You can always pause, learn that bug from the list, then come back to the writeup. The order here isn’t strict.

**Here’s your guide:**


- [Before We Get Started](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Before%20We%20Get%20Started.md)
- [Injection Bugs](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Injection%20Bugs.md)
- [Server-Side Logic Bugs](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Server-Side%20Logic%20Bugs.md)
- [Client-Side Bugs](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Client-Side%20Bugs.md)
- [Authentication Bugs](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Authentication%20Bugs.md)
- [Authorization Bugs](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Authorization%20Bugs.md)
- [Infrastructure-Misconfiguration Bugs](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Infrastructure-Misconfiguration%20Bugs.md)
- [Beyond Vulnerabilities](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Beyond%20Vulnerabilities.md)



## 🚀 3. Getting Started with Real Hacking

After learning the web fundamentals, common vulnerabilities, and understanding the rules, it’s time to put all of that into action.

The goal here is to start hunting in a real-world environment so you can apply what you’ve learned and work toward earning your first bounty.

- Sign up on [HackerOne](https://hackerone.com/).
- Pick a target from the [directory](https://hackerone.com/directory/programs).  
>[!Tip]
> The more reports a program has resolved, the higher your chances of finding a bug as a beginner.
- Start hunting using our [testing methodology](https://github.com/BehiSecc/First-Bounty/blob/main/Vulnerabilities/Beyond%20Vulnerabilities.md#testing-methodology)
- Stay focused on your target for at least 6–8 weeks.

After those 6–8 weeks, you should have a solid shot at getting your first bounty.

> [!Note]
>  Once you get your first bounty, DM me on X ([@Behi_Sec](https://x.com/Behi_Sec)), I should have the next steps ready for you by then.



## 🧰 4. Supporting Skills  
No matter where you are in your journey, dedicate time to learn and explore new areas.
As a beginner, there are a few extra skills worth picking up early that will pay off later.

### Networking  
Networking is the foundation of how devices and systems communicate over the internet. Understanding it helps you make sense of how data moves between clients, servers, and other systems. 
For now, focus on the basics like IP addressing, DNS, and how devices connect and communicate.

Resources:  
- [Introduction to Networking – Zero to Mastery](https://zerotomastery.io/blog/introduction-to-networking/)  
- [Networking Basics PDF](https://www.ece.uvic.ca/~itraore/elec567-13/notes/dist-03-4.pdf)  

### Linux Basics  
Linux is the operating system that powers most servers and many security tools. It’s important because many real-world exploitation steps, from running scripts to analyzing logs, are easier and faster in a Linux environment.
You don’t need to go deep for now, only learn basic commands, file navigation, and permissions.  

Resources:  
- [Linux Journey](https://linuxjourney.com/)  
- [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/)  

### Python or Go  
Python and Go are great for automating tasks and building hacking tools.
Knowing one will help you process data faster, build custom tools, and automate repetitive tasks.

Resources:  
- [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/)  / [Learn Python](https://www.learnpython.org/)
- [Go by Example](https://gobyexample.com/)  



## 💡 FAQ

### How long does learning all this take?  
It depends on how much time you put in and your prior experience. I believe that starting from zero and following this roadmap consistently, it’s possible to get a first bounty within 6–8 months.

---

### Is bug bounty worth it?  
Yes, if you enjoy learning, problem-solving, and persistence.

No, if you’re looking for quick money or an easy path.

---

### Is bug bounty easy?  
No. The basics are simple to understand, but finding impactful bugs takes patience, skill, and creativity. 
If you’re looking for "easy", bug bounty isn’t for you, but it’s exactly the challenge that makes it so rewarding.

---

### I’m good at CTFs and challenges but I can’t find bugs. What should I do?  
CTFs test problem-solving in controlled environments. Real bug bounty targets are messy, unpredictable, and don’t give you hints. Start applying your skills to real applications, stay focused, and dig deeper. Eventually, you’ll land your first valid bug.

---

### I keep quitting programs/targets. What should I do?  
Commit to one target for at least 6–8 weeks. Quitting early means you never reach the deeper bugs. Treat each target like a long-term puzzle instead of a quick hit.

---

### The bugs in writeups seem so easy, but my targets feel secure. Why?  
You’re seeing the final, polished story. The hunter probably spent days or weeks exploring before finding that “easy” bug. Security isn’t absolute but finding the gap takes persistence and the right angle.

---

### There are a lot of resources out there. where should I start?  
Start with the roadmap in this repo. Follow it step by step to avoid overwhelm.

---

### Should I wait to start hunting until I've learned every bug category? 
No. You’ll never truly “finish” learning all bug categories; even experienced hunters are still learning. 
As soon as you learn a bug type, you can start applying it to real targets. Even if you don’t find anything, you’ll get familiar with the process and gain experience.

---

### How can I see what others are doing?  
Join bug bounty communities on X, Reddit, and Discord. Follow active hunters, read their posts and writeups, and engage in discussions.

Here are a few communities worth checking out:  
- [r/bugbounty](https://www.reddit.com/r/bugbounty/)  
- [Bug Bounty Write-Ups](https://x.com/i/communities/1489229152280530960)

---

### What tools do you use?  
My main tool is Burp Suite, but I also use:  
- [ffuf](https://github.com/ffuf/ffuf)  
- [nuclei](https://github.com/projectdiscovery/nuclei)  
- [waybackurls](https://github.com/tomnomnom/waybackurls)  
- [LinkFinder](https://github.com/GerbenJavado/LinkFinder)  
- [Arjun](https://github.com/s0md3v/Arjun)  
- [cloud_enum](https://github.com/initstring/cloud_enum)  




## ⚠️ Beginner Mistakes to Avoid

As a beginner, you won’t know everything — and that’s normal.  
The goal here is to avoid mistakes that waste time and cause frustration, so you can focus on the right things and keep improving in the long term.

- **Don’t work 24/7**  
  This field can be addictive. If you overwork, you’ll burn out quickly. Take breaks and pace yourself.  
  I don't recommend working on weekends or more than 8 hours per day.

- **Don’t install Kali Linux (just because it’s “for hacking”)**  
  Kali is just a Linux distro with a lot of pre-installed tools. It’s cool, but unnecessary. I recommend using a stable distro like Ubuntu and installing only the tools you actually need.

- **Don’t get obsessed with tools**  
  There are countless tools out there. Don’t collect them just for the sake of it. Stick to the ones that work for you.

- **Don’t compare yourself to others**  
  Everyone’s journey is different. Focus on your own progress. You can learn and master this field with enough time and practice.

- **When you see someone’s bounty, don’t get emotional**  
  Use it as motivation, not a reason to feel discouraged. Keep improving your skills and you’ll land high bounties.

- **Have a vision**  
  After a while, you might lose motivation or excitement. Having a clear long-term goal will help you stay focused.  
  Don’t just do it for the sake of money, you’re in a field that can have a significant positive impact on millions of users.

- **Think and search before asking questions**  
  Often, the answer is already out there. Searching first will make you a better learner and help you avoid looking like a noob.

- **Stick to what works for you**  
  Don’t constantly jump between different approaches or bug types. Give your strategy time to produce results.

- **Don’t take things personally**  
  Unfortunately, there are toxic people in this field. If someone responds poorly to your beginner questions, move on and focus on those who help.

- **Don’t spam others**  
  Respect people’s time and space. Constantly DMing or emailing others will just make them ignore your questions.

- **Don’t stop learning**  
  Bug bounty is constantly evolving, keep learning and exploring.

- **Don’t expect too much from your first few reports**  
  Early on, most reports will be marked as “Not Applicable” or “Duplicate.” That’s part of the process.  
  Learn from your reports and hit harder next time.

- **Believe in yourself**  
  Confidence and persistence are just as important as technical skill. This field takes a huge amount of time to learn, but it’s not a sci-fi skill only a few people can master. If others could do it, so can you( just make sure you have a strong reason to start and that you understand the hardships before jumping in).



## 🤝 Contribution

If you have suggestions, improvements, or new resources to add:

1. Fork this repo
2. Make your changes
3. Submit a Pull Request

You can also open an **Issue** 🐛 if you spot something that needs fixing.

## 📬 Contact

If you want to contact me, you can reach me on [X](https://x.com/Behi_Sec).

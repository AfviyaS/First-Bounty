But bug bounty hunting is more than just knowing how XSS or IDOR works.

Before you start testing real targets, you should be familiar with other core concepts that make you a well-rounded hunter. These skills will help you find more bugs, avoid mistakes, and stand out from beginners who only know the basics.

In this section, we’ll cover:


- [Recon basics](#recon-basics)
- [Testing methodology](#testing-methodology)  
- [Responsible Disclosure and Ethics](#responsible-disclosure-and-ethics)
- [Understanding Scopes and Rules](#understanding-scopes-and-rules)
- [Bug Report Writing](#bug-report-writing)
- [Mindset for Bug Hunting](#mindset-for-bug-hunting)


## Recon basics

Recon is the process of gathering information about your target before testing.

Here are some great resources on this topic:
- [Bug Bounty Recon Guide – YesWeHack](https://www.yeswehack.com/learn-bug-bounty/recon-series-recap-reconnaissance-footprinting)
- [Recon for Bug Bounty: 8 Essential Tools – Intigriti Blog](https://www.intigriti.com/researchers/blog/hacking-tools/recon-for-bug-bounty-8-essential-tools-for-performing-effective-reconnaissance)
- [The Bug Hunter's Methodology v4.0](https://www.youtube.com/watch?v=p4JgIu1mceI)



## Testing methodology


Many beginners test randomly, clicking around and hoping to stumble upon a bug. That approach might work once in a while, but it’s inconsistent and wastes time.

A testing methodology is simply a plan for how you’ll approach a target. It keeps you organized, reduces missed areas, and helps you reproduce results.

This is a simple example I recommend for beginners:

1. **Map the Application**
   - Use the application like a regular user would.
   - Understand all available features.
   - List endpoints, parameters, and forms.


2. **Test Feature by Feature**
   - Choose one functionality and test it for potential bug types, for example, on a file upload feature, check for unrestricted file types, path traversal, etc.

3. **Use a Checklist**
   - Have a simple list of bugs to check for. [This repo](https://github.com/Az0x7/vulnerability-Checklist?tab=readme-ov-file) is a good starting point.
   - Update your checklist as you learn more.

4. **Take Notes**
   - Document what you tested, what worked, interesting behaviors, etc
   - Use [Obsidian](https://obsidian.md/) or [Notion](https://www.notion.com/)



## Responsible Disclosure and Ethics

Bug bounty hunting only works when there’s trust between hunters and organizations. That trust comes from following the rules and acting responsibly.

Keep these principles in mind:

1. **Only test targets you have permission for.**  
   - Only test targets listed as in-scope.
   - Never test random websites, it’s illegal and can have serious consequences.

2. **Report, don’t exploit.**  
   - Your goal is to prove the bug exists, not to cause damage.  
   - Avoid actions that could harm data, users, or systems.

3. **Follow disclosure rules.**  
   - Some programs allow public writeups after a fix, others require permanent confidentiality.  Always respect the program’s disclosure policy.

4. **Be professional.**  
   - Provide clear, respectful communication.  
   - Avoid frustration or hostility, even if your report gets marked as duplicate or N/A.


## Understanding Scopes and Rules

Before you test anything, you need to know exactly what you’re allowed to hack. That’s what the scope and rules define.

Program guidelines tell you which targets you can test, what types of vulnerabilities are in-scope, and what testing methods are allowed. Many rules are common across bug bounty programs, but some programs also have unique requirements.

Here’s what you should know about scope and rules:

1. **Scope Basics**
   - **In-scope** means you have permission to test those targets.  
   - **Out-of-scope** means you must avoid them completely.  
   - Scope can include domains, subdomains, IP ranges, mobile apps, APIs, and more.  

2. **Reading the Scope Carefully**
   - Look for target lists, wildcards, and exclusions.  
   - Pay attention to notes that specify testing environments or restrictions.  
   - Some programs limit the types of vulnerabilities they accept.  

3. **Rules to Follow**
   - No denial-of-service attacks.  
   - No spamming or phishing users.  
   - Avoid automated scanning that can overwhelm systems.  
   - Don’t access or modify real customer data.  





## Bug Report Writing

Finding a bug is only half the job. If your report is unclear or incomplete, the program’s security team might reject it, misjudge its impact, or ask you to redo the work.

A good bug report should be clear, concise, and reproducible.

Here’s what every good bug report should include:

1. **Title**
   - Keep it short but descriptive.  
   - Example: "IDOR in /api/user allows access to other users’ information."

2. **Description**
   - Clearly explain what the bug is and why it matters.  
   - Include the vulnerability type, the affected endpoint or feature, and the potential impact.

3. **Steps to Reproduce**
   - Write step-by-step instructions so anyone can replicate the issue.  
   - Keep each step clear and in order.  
   - Include sample payloads or modified requests where needed.

4. **Impact**
   - Explain what an attacker could do if this bug were exploited.  
   - Connect it to real-world consequences like data theft, account takeover, or service disruption.

>[!Note] 
>I created a GPT called [ReportWriter](https://chatgpt.com/g/g-67adbeb78b588191aeadae88489173d9-report-writer) to make this task easier. Use [ReportWriter](https://chatgpt.com/g/g-67adbeb78b588191aeadae88489173d9-report-writer) to help write clear and structured reports.



## Mindset for Bug Hunting

Bug bounty hunting is a long game. You won’t find critical bugs every day, and you will face rejections, duplicates, and dry spells. Your mindset will often decide whether you improve or quit.

The following tips can help you stay motivated and improve over time:

1. **Be Patient**
   - High-quality bugs take time to find. Don’t expect instant rewards.  
   - Treat each test session as practice, even if you find nothing.

2. **Stay Curious**
   - There’s always something to learn if you’re curious enough.  
   - Explore parts of an application that others might ignore.

3. **Think Like a Developer**
   - Understand how features are built and how the application is meant to work.  
   - Consider what small checks or validations a developer might have missed.


4. **Learn from Every Report**
   - Read other hunters’ writeups to see different approaches. I highly recommend reading every disclosed report on the [Shopify](https://hackerone.com/shopify) and [GitLab](https://hackerone.com/gitlab) programs.
   - Analyze your own rejections or duplicates to improve next time.

5. **Be Consistent**
   - Regular hunting builds skills faster than rare marathon sessions.  
   - Even short, focused practice sessions matter.

6. **Protect Your Mental Health**
   - Your health is far more important than bug bounties or money.  
   - [This video](https://www.youtube.com/watch?v=raH7tRy8M7g) offers helpful advice on maintaining your mental health.

7. **You’ll only find what you’re looking for**  
   - If you want to find high-severity bugs, you have to actively hunt for them.  
     If you spend all your time testing low-hanging fruit like open redirects or DKIM issues, don’t expect to stumble upon an IDOR or SSRF. Focus your efforts where you want results.

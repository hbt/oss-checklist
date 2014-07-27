---
layout: post
title:  "Open Source Software checklist"
---

<img src="https://raw.githubusercontent.com/hbtlabs/oss-checklist/master/doc/icons/Misc-Settings-icon.png" width="20" title="TODO: add flowchart with graphiz"/>

problem identification / definition
- https://www.google.ca/search?channel=fs&q=problem+definition+for+project&revid=1953962045&bav=on.2,or.r_cp.r_qf.&bvm=pv.xjs.s.en.PAf6cFvc9yg.O&ech=1&psi=qOrUU4v2H6eD8QHJ24CoAQ.1406462633221.3&ei=qOrUU4v2H6eD8QHJ24CoAQ&emsg=NCSR&noj=1
- http://www.sciencebuddies.org/engineering-design-process/engineering-design-problem-statement.shtml
- http://www.sciencebuddies.org/engineering-design-process/engineering-design-problem-statement.shtml#checklist
- https://www.google.ca/search?client=ubuntu&channel=fs&q=problem+definition&ie=utf-8&oe=utf-8&gfe_rd=cr&ei=hP3IU83rG8KC8QfDxIG4CQ#channel=fs&q=problem+definition+in+research&revid=1953962045
- http://www.studygs.net/problem/problemsolvingv1.htm
- http://ctb.ku.edu/en/table-of-contents/analyze/analyze-community-problems-and-solutions/define-analyze-problem/main
- http://www.wikihow.com/Define-a-Problem


Research
research the problem and how other people experiencing it have to say about it . differnet from searching for solutions. Goal here is to make sure you are addressing the right problem.
  case: think big/abstract - e.g  phpmyadmin mysql browser with keyboard shortcuts vs vimium

- learn the vocabulary of the problem (reading articles etc.) to learn the right keywords to make better searches
  case: evaluate OSS
  
-come up with a list of basic product requirements.   

research existing solution to that problem + evaluate themn
  case: backup

consider using different products and mashing them together to get what you want
  case: backup
  

Post research analysis
possibilities:
- you found the perfect product
- you found multiple products and you have to mash them up
- you found existing solution(s) but some key requirements are not addressed. (fork, contribute, develop)
- you found no solutions (worst)


In the case of existing solutions:
- if closed source, consider developing the feature separately and get it to communicate with the closed source product
- if open source, consider the effort required to integrate your feature in the project (e.g history of pull requests, is it worth contributing?). 
Otherwise, treat it as closed source and develop the feature separately. It is not adivsed to fork and maintain a custom fork unless you can really isolate your changes


## Stage 0 - Before starting an OSS project

- questions to ask before starting a project
    - does your idea apply to yourself or can others use it?
    - has somebody already had your idea or similar one?
    - choose collaboration instead if any of this is true: "Will the new project be duplicating work done by another project? Will the new project be competing for developers with an existing project? Can the goals of the new project be accomplished by adding functionality to an existing project?"


- ###Research 
  - *Define* the problem and break it down
  - *Search the problem* and see how people are already solving it
    - Tools
      - google
  - *Search the solutions* for existing projects
    - Tools
      - github
      - codeplex
      - freshmeat
      - <img src="https://raw.githubusercontent.com/hbtlabs/oss-checklist/master/doc/icons/Misc-Settings-icon.png" width="20" title="TODO: document others + add links"/> etc.
    - Enhancements needed in this area
      - <img src="https://raw.githubusercontent.com/hbtlabs/oss-checklist/master/doc/icons/Misc-Settings-icon.png" width="20" title="TODO: suggest"/> X
  - *evaluate* open source solutions
    - reputation (quality: performance & reliability)
    - activity
    - interoperability (ability to mashup systems)
    - support (community / commercial)
    - last stable version
    - documentation
    - maintenance costs (install, configure, update/upgrade etc.)
    - project management / contributors (howto contribute, development processes etc.)
    - license
    - *Tools*
      - assessment methodologies 
      - ossmeter
      - <img src="https://raw.githubusercontent.com/hbtlabs/oss-checklist/master/doc/icons/Misc-Settings-icon.png" width="20" title="TODO: add other OSS software evaluators"/> etc.
  - *mashup up* multiple systems to solve the problem instead of looking for one perfect solution
    - Tools
      - mashableapi
      - open protocols (plain text, json etc.) 
      - API
      - <img src="https://raw.githubusercontent.com/hbtlabs/oss-checklist/master/doc/icons/Misc-Settings-icon.png" width="20" title="TODO: document "/> etc.
      
## Stage 1 - Starting

- define *purpose*
  - Short, general, ambitious and clear statement related to what it does
  - think big and small - focus on immediate needs but have ambition i.e how others could use it?
- define *roadmap*
  - a set of milestones towards completing a vision
- define *features* 
  - the minimum required to solve the problem and achieve the first milestone
- *name* the project
  - gives an idea of what the project does
  - easy to remember
  - is not the same as some other project's name
  - is available as a domain .com, .net or .org
- short description
  - quick description to decide in less than 30sec if they want to learn more or not. Concrete, limited, short.  Can be be more than one sentence
- licensing    

## Stage 2 - Development
- Solve the right amount of the problem first -- Solving too much of the problem relegates the OSS development community to the role of testers. Solving too little before going OSS reduces "plausible promise" and doesn't provide a strong enough component framework to efficiently coordinate work.
- Importance of modularity / componentization in order to deal with integration of patches from multiple sources later on
- Methods
  - Martin Fowler / agile / esr hack
    - minimum effort path to get result
    - write automated test to check result against spec
    - refactor
- *open source from day one*
- be open from day one
    - open sourcing later means reviewing the code / history for personal data and such
    - difficult because you will always favor decisions that make it incompatible for the future 
- *explain your role*  - open source the code does not necessarily mean opening your schedule. Clear things up.
  - how serious are you about the project? 
  - can people contact you? 
  - if they log issues, will you address them?
  - 
- *everything in the open, everything in one place* - avoid hiding important information e.g requirements in private GDocs
- *document*
  - features list
  - requirements / dependencies
  - install instructions
  - configuration 
  
- explain your branches
  
- release early, release often  
- changelog
what has been changed, fixed, or added to the program

- *release scripts*
  - packaging binaries
    - binaries in download section
      - provide checksums
   - uses appropriate package manager
  - deployment scripts
    - travis
- test    
- Don't be afraid to throw away code, if you don't feel good about it
- Simple Design & minimum-effort path (simplest thing that works but not the dumbest thing)
- Perfection (in design) is achieved not when there is nothing more to add, but rather when there is nothing more to take away 
- update roadmap
- update progress (development status) -- progress of features if project is very new
      - developement status should answer two questions:
            - where does the project stand in relation to its stated goals?
            - how fast is it making progress?
            - how active is the project?
                - is stuff going on? are there people getting things done?
           e.g launchpad.net
    should reflect reality -- don't hype, don't acquire a reputation for buggy software that failed to deliver

## Stage 3 - Marketing
- spread the word
  - freshmeat
  - Q&A sites
  - forums 
  - users of related/alternative technologies 
- demos / screenshots/ videos / example output
    - web-based = demo site
    - GUIs = screenshots + maybe videos (with subtitles / narrator (less than 4m))
    - console, try ttyrecord
- extra stuff (not necessary for a start)
    - news page
    - project history page
    - related links
    - site-search
    - donations
    - blog 
    - ***make a list***
- mention alternatives / comparisons to other solutions
- mention how the software can be integrated / used

## Stage 4 - Contributors

- avoid private discussions and rudeness
- clarify expectations
    - what can people expect from you? will you respond to bugs and address them?

- - website = user section and developer section
    - "get involved" = other type of volunteers (support, triage, donations, UI designers, marketing etc.) https://wiki.documentfoundation.org/Get_Involved https://wiki.documentfoundation.org/Marketing
    - dev wiki = excellent example https://wiki.documentfoundation.org/Development

- metrics
    - operational health: s the project's ongoing ability to incorporate new code contributions and new developers, and to be responsive to incoming bug reports
    - Survivability is the project's ability to exist independently of any individual participant or sponsor—think of it as the likelihood that the project would continue even if all of its founding members were to move on to other things
documentation 
    - developer guide (to explain the API, naming conventions, tookit issues etc.)
    - user guide (comprehensive guide for users on how to operate the software)
    - requirements / design document 
        - list of modules/systems + interactions / diagrams
        - what modules should do (inputs, outputs)
    - all 3 documents above must be on source control

- open your code, not your time -- decisions on what the project is and your role in it
- patches
    - review & accept as quickly as humanly possible
- emails 
    - reply quickly
- create a welcoming atmosphere

- make things easy 
    - easy to install, modify, find the project, find documentation, try etc.
- developer 
    - guidelines
        - how to interact with other developers
        - how to report bugs / submit patches
        - how development is done / decisiosn made 

    - developer documentation
        - difference from guidelines is ". Developer guidelines tell programmers how to get along with each other; developer documentation tells them how to get along with the code itself."
        - grown not written
        - focus on user documentation because users with an incentive + knowledge will dig into the code

- documentation
    - how to quickly set up the software
    - overview of how it works
    - guides to doing common tasks
    - should be all in one page because people want to search for specific words

- guidelines to writing documentation 
    - limit the scope
    - tell the reader how much knowledge they are expected to have e.g know rvm, ruby, + apt-get
    - tell the reader how to verify that the install was correct
    - startup documentation is more important than usage documentation
    - one tutorial on how to do a common task
    - highlight areas where documnetation is incomplete

- maintaining a FAQ
    - good FAQs are grown not written. They are based on experience gathered and previous questions asked and patterns
    - FAQs are also a good indication of major improvements waiting to be made in the application because that many people should not be asking the same question over and over if the answer was not obvious
    - monitor stackoverflow tags related to your project


- faq 
  - faqs are grown based on patterns of questions
- issue tracker  
- delegate everything you can
- Be open to the point of promiscuity
- listen to users and build contributors
- procedures: "to capture the best known way to accomplish routine tasks"
- *make it easy*
  - small tasks identified in the code and linked to the issue tracker
  - up-to-date HOWTO guides on how to develop locally
  - clear instructions to log issues, send pull requests etc. 
- *Communication channels*  
  - google groups
  - issue tracker
  - IRC 
  - website
  - email
- awareness 
  - Awareness encompasses knowing who else is working on the project, what they are doing, which artifacts they are or were manipulating,
   and how their work may impact other work
- *Forks* 
  - analyze the forks 
    - are people forking to contribute OR are they forking to configure?
- *Issues* -  bugs/features/changes/discussions 
  - how responsive are you?
  - check for patterns in bugs
  - listen to suggestions / ideas in discussions
  - check how people are using the software
- facilitate evaluation of your project by providing metrics  
      - if project is mature
        - recent activity, recent releases, issues, analytics
        - is it maintained?
        - how often it puts out new releases?
        - how responsive it is likely to be to bug reports?
        - history of past releases / change log
        - future releases (roadmap)
        - *** a panel that aggregates data on the status of the project to show developmenet stauts and progress ***
           - timeline of recent releases
           - recent activity in bug tracker
           - mailing lists / forum activity / google groups

  
  
## Stage 5 - Commercialization

- business models
- making changes and contributing
    - using your employees to make the changes you want
    - offering bounties (pledge/sponsor system)


## Later
- successor / survivability

-------------------------------------------------


Notes:
http://www.catb.org/~esr/writings/cathedral-bazaar/homesteading/ar01s13.html
the role of reputation in measuring contributions and evaluating projects


Notes: 


http://opensource.com/business/13/8/oss-patterns-and-practices
Stages:
- build users
- build community
- build contributors
- build commercial community

So, driving open source project success is an exercise in building onramps for communities of users, developers, and contributors, and eventually commercial contributors to enable an project ecosystem.

Marketing:
    - attract a lot of users 
        - easy install, configure, usage, 
    - attract developers
        - easy download, test, develop, configure, fix, patch
    - attrack contributors
        - easy howto contribute, guides, communication, pipeline, bug reports, 
        
        
- have blank / work areas -- where you can clearly see what needs contributions / work       
        

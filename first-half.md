# Chef Conf Talk

## I. Back-story
  A. Relativity has been a long-term client
  
    1. Why they hired us.
    
    2. I was excited to on-board.
    
    3. I was hired to bring testing.

## II. When I got there...

  A. Jira backlog took precendence
  
  B. Then started adding Test Kitchen and InSpec tests to cookbooks
  
    1. Not everyone knew how to run it locally
    
    2. Develop was still broken all the time
    
    3. Had to train
    
### III. Pull Request Builds
  A. Had to enforce Test Kitchen since we couldn't trust is people would use it
      
      1. Getting feedback back to the reviewers is critical. We had all this automation hooked up, builds automatically kicking
      off for each commit. But without easy feedback, we still had red build. 
  
  B. Because the backlog was top priority, had to work it in on the side
  
  C. Had to work across teams to figure out BitBucket / Jenkins integration
  
    1. Nick and Ray
    
    2. DevOps basics
    
### IV. Moving to larger scale

  A. My team was proving ground
  
  B. Nick took the basis and flew with it. 
  
  Annie to show the Jenkinsfile/rakefile

### V. Managing at the Project level
  
  Annie had this repo, or a small set of repos that had this awesome workflow developed.
  
  A. Take Annie's workflow and centralize it. Using Jenkins "Shared Libraries" it makes it really easy to consume. Instead of copying & pasting all of the rake libs & Jenkinsfiles into each repository, we copy & paste a 5-line block. A simple "hook" into our workflow. 
  
  B. It does not have to be super complex, especially at first. It's about taking what makes sense and making it easy to use. 
  
  Possibly show some metrics? Figure out how to show/measure our success. 
  
  TO DO: Show Side-by-Side comparison with the "CookbookCI" helper. 
  
### VI. Buy-in for this Direction

  A. When we needed to shut down commits to a shared code base, it was easy to go in and change the workflow from a central place to temporarily disable any additional code from introduced. 
  
  B. When we got a new Chef server, we had to start uploading our cookbooks to it. With Jenkins "Shared Libraries" it was as simple as modifying one place. 
  

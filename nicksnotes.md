# Chef Conf Talk

Shared jenkins libarary is an evolution to the rake lib/tasks maintained in every repo. Ability to manage code at a higher level than just repositories. 

Chef cookbooks are a perfect candidate for managing at a higher level. All should:

  * Run foodcritic/rubocop
  * Run RSPEC
  * Run Test-Kitchn
  * Package & Upload to Chef
  
 Managing code at the "project" level reduces the snow-flakiness of repository code managament. 
 
 Managing code at the "project" level lowers barriers of entry allowing for easier value contribution from outside team members.
 
 
 
 
 # TO DO
 
 * I think we need a small Jenkins server hooked up to GitHub. Probably do a small docker container locally

 * Figure out what we are going to demo (if anything?)

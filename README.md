#Git Hooks

##Intro
Below are a scripts that you should be including for all your git repositories for Delivery Agent. To install, in your local repository, copy the hook into the .git/hooks/ directory


###Required
post-message-hook

post-message-hook will generate our commit message template in the following format, if you commit without using -m, it will open your editor with an auto-generated format.


	commit ee69bc661b910691e8f4ab1821203432ad89128a - commit
	Author: Albert Wu <awu@deliveryagent.com> - author
	Date:   Fri Jun 13 11:54:44 2014 -0700 - time

	[branch you are on]
	Test commit - your desired message

	Modified Files
	M  test.java

If you use git commit -m "Message goes here", it will still keep the formatting we destire,

	commit ee69bc661b910691e8f4ab1821203432ad89128a - commit
	Author: Albert Wu <awu@deliveryagent.com> - author
	Date:   Fri Jun 13 11:54:44 2014 -0700 - time

	[branch you are on]
	Message goes here

	Modified Files
	M  test.java
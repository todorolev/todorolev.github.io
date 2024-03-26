---
layout: post
title:  "Comparison between GitHub Copilot and Tabnine in IntelliJ IDEA"
date:   2024-03-26
categories: tool
---
I've been experimenting with AI tools integrated into my IDE to test their effectiveness in accelerating my coding process and improving efficiency.
I did some research on which tool would fit well into the work process of a software developer who writes a lot of code. I ended up with GitHub Copilot and Tabnine on the table, both of which looked equally good from what I read in various articles. 
So I installed both the Copilot and Tabnine plugins in IntelliJ and I switch on/off one or the other every day to see which works better for me. Below is the result from this excercise in the form of a scoring game. 

### Suggestions for improvements in code *(Copilot 1:0 Tabnine)*
*One point to Copilot.*

	String username = playerRequest.getUsername();
	
Copilot correctly recognized the aim of introducing the new variable ```username``` - to replace it’s value in several places, and even did one correct replacemet. 
<br />
<br />
Tabnine just pointed 3 “code issues”, all of them exactly the same - that there was an unused variable declaration.

### Suggestions for code completion *(Copilot 2:0 Tabnine)*
*This is another one for Copilot.*
<br />
<br />
Copilot’s suggestions are more accurate, complete and more likely to be accepted. 
<br />
Example - I started typing:
	
	.depo

Copilot:
	
	.deposits( user.getDeposits().stream().map( DepositResource::of ).toList() )

Tabnine:

	.deposits( user.getDeposits().stream().map( DepositResource::of )

***Note:*** *This extends beyond just code completion during the implementation of business logic. Copilot provides superior completion suggestions across the board, including during the creation of unit tests and javadoc.*

### Ease of use *(Copilot 2:1 Tabnine)*
*One for Tabnine.*
<br />
<br />
Copilot functions are harder to use. Most the context menu options lead to opening the Copilot Chat, which seems to be working for just a few people, the rest are in a "waiting list". So for the normal user most functions go to a dead-end.

Tabnine has an intuitive interface and all functions  seem to be working fine, including the chat.

***Note:*** *I actually stayed in the waiting list for just few days, then I was allowed to the chat, which made Copilot easier to use. Still Tabnine remains more straightforward and intuitive.*  

### Pricing *(Copilot 3:2 Tabnine)*
*One point for each.*
<br />
<br />
Copilot’s individual plan costs 10$/month.
Tabnine’s Pro plan costs 15$/month paid monthly and 12$/month paid annually. However, Tabnine has free basic version.

### Recap
Copilot and Tabnine bear a lot of similarities in the ways they help improve the efficiency of writing code. Personally, I favor GitHub Copilot due to its higher accuracy; often, with minimal adjustments, I achieve satisfactory code. For an experienced developer, overall, both tools excel, especially in writing test and javadoc.
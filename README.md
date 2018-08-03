# scoring_webapp
Applying a scoring system in our website

# Create scoring condition
Create a new condition named Any page condition which has the condition of type: Page path, with
operator: contains param: /

The above condition means that we want this condition is satisfied if page path contains / which 
is true for every page of website hence condition is satisfied if any page of our website is 
accessed.

# Scoring system
Create a Score named Basic scoring and in the column with Start scoring if select condition of 
Any page condition and in the column for Set a score if select the same condition of Any page 
condition and set the score of value 1

# Create modal
Create a new modal named Subscription modal and select checkbox of show only once and paste code 
for subscription form from subscripion_form.html

# Setting trigger
We want to show the subscription form to the users if we total score for website is three so for 
that we can add trigger to the Basic scoring modal and select scoring in and set score to 3, this 
means that we want the form to be shown if score equals 3.

# Pro scoring condition
Users will be displayed a discount card once the pro score reaches 10. We set another condition 
named Offer page condition and set its operator: contains and param: offer. The Offer Page 
contain string "/offer" in its URL address, so the condition above will be fullfiled after 
visitng the Offer Page. 

# Create Pro score
Make a new score named Pro scoring and to Start counting if add a trigger named and set offer page
condition as trigger.To the set score if add Any page condition as a trigger and save and publish 
changes.

# Discount modal
Create a new modal and add the discount_modal_card.html and save the modal, set the trigger to scoring if Pro scoring reaches 10 scores and save and publish changes. 
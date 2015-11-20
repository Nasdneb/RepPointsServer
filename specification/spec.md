Fair Collaboration

components specification

describe central bank account
	- should accumulate all income
	- should pay user revenue according to reputation points

describe user
	- should have reputation points
	- should have reliability percentage
	- should have a list of tasks
	- should have a list of publicly available resources
	- should have a list of reoccurring tasks
	- should have a list of reoccurring resource transfers
	- should have a list of reoccurring reputation points transfers

describe reputation points
	- should be equal to all users at the beginning
	- should be gained from an accomplished task
	- should be possible to give to other user
	- should be recalculated to avoid inflation
	- should be able to be regularly assigned to a reoccurring task
	- should be multiplied when a user joins or leaves the organization

describe task
	- should be possible to create by an user
	- should be assigned a title
	- should be assigned a description
	- should be assigned expected reputation points
	- should be assigned necessary resources
	- should be assigned an estimated time for accomplishment
	- should accept reputation points for backing
	- should need total amount of expected reputation points to be backed successfully
	- should distribute backed reputation points to all users equally once backed successfully
	- should transfer the assigned points to the task creator once finished
	- should be logged
	- should accept comments
	- should be able to create as reoccurring task
	- should show it's results to the backers, once accomplished

describe reliability
	- should be voted on by users once a task is accomplished

describe resources
	- should be assigned to a task if necessary
	- should be transferred from user to user
	- should be able to be regularly transferred to a reoccurring task

interface specification

As a user
When I go to the task board
Then I see the tasks in user columns

As a user
When I go to the task board
I can vote on tasks

As a user
When I vote for a task
I can reclaim my voted points

As a user
When I go to the task board
I can create a new task

As a user
When I go to the distribution view
I can see the distribution of reputation points and the total income

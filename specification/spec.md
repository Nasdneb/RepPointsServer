Fair Collaboration

components specification

describe reputation points
	should be equal to all users at the beginning
	should be gained from an approved activity
	should be possible to give to other user
	should be recalculated to avoid inflation

describe voting points
	should be mirroring the reputation points
	should be locked on an activity before it gets accepted
	should be given back after the activity is accepted

describe activities
	should be possible to create by an user
	should expire after x days if not accepted through voting
	should be assigned reputation points
	should be checked by users who voted to flag as accomplished
	should accept voting points
	should need half of the total reputation points to be successfully voted
	should transfer the assigned points to the activity participants
	should be logged

describe points redistribution
	should happen after the payments
	should remove the peaks and smoothen the points distribution

interface specification

As a user
When I go to the activity board
Then I see the activities in user columns

As a user
When I go to the activity board
I can vote on activities

As a user
When I go to the activity board
I can create a new task

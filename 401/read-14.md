# Event Driven Architecture


### What’s the difference between a FIFO and a standard queue?
- They are rather similar but FIFO also provideds some checks and balances to ensure there is no duplicates.
### How can the server be assured a message was properly received?
- By sending confirmation messages like the acknowledge step in a syn/ack system
### What classic design pattern is best represented by event driven programming?
- Observer. THis is where a system maintains a list of dependancies(observers)
### How do you test an event driven system?
- by testing it for end to end function. Additionaly you would instantiate some compnent(unit) testing to comfirm smaller parts of the applicatin are functioning.


# Terms

### FIFO Queue
  - Its a queue system where the actions send it are completed in the order they are recieved
### Pub/Sub
  - This is the event components for systems like socket.io, Publishing it tx'ing data. Sub'ing is 'listening' for the before mentioned "publishes"

### Which 3 things had you heard about previously and now have better clarity on?
- loved the CC PR explanation
- SNS - do others care about your data
- SQS - do events pertain to you
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- sns vs. sqs, but more enterpise examples
- I'd like to learn more about the validation step in making a transaction
- 
### What are you most excited about trying to implement or see how it works?
- is lambda a must know for dealing with these systems
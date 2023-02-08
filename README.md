# streaming-04-multiple-consumers

> Use RabbitMQ to distribute tasks to multiple workers

One process will create task messages. Multiple worker processes will share the work. 


## Before You Begin

1. Fork this starter repo into your GitHub. Done
1. Clone your repo down to your machine. Done
1. View / Command Palette - then Python: Select Interpreter Done
1. Select your conda environment. Done

## Read

1. Read the [RabbitMQ Tutorial - Work Queues](https://www.rabbitmq.com/tutorials/tutorial-two-python.html) Done
1. Read the code and comments in this repo. Done

## RabbitMQ Admin 

RabbitMQ comes with an admin panel. When you run the task emitter, reply y to open it. 

(Python makes it easy to open a web page - see the code to learn how.)

## Execute the Producer

1. Run emitter_of_tasks.py (say y to monitor RabbitMQ queues) Done

Explore the RabbitMQ website.

## Execute a Consumer / Worker

1. Run listening_worker.py    Done

Will it terminate on its own? How do you know?  No. I had to manually press Control + C to terminal it

## Ready for Work

1. Use your emitter_of_tasks to produce more task messages. Done

## Start Another Listening Worker 

1. Use your listening_worker.py script to launch a second worker.  Done

Follow the tutorial. Done
Add multiple tasks (e.g. First message, Second message, etc.)
How are tasks distributed? Alternated messages being sent to terminals. Not sure if it was equally received by each consumers in version 1, and 2. But for version 3, each consumer will receive the next message when the previous one was done.

Monitor the windows with at least two workers. Done
Which worker gets which tasks? As above,Not sure if it was equally received by each consumers in version 1, and 2. But for version 3, each consumer will receive the next message when the previous one was done.


## Reference

- [RabbitMQ Tutorial - Work Queues](https://www.rabbitmq.com/tutorials/tutorial-two-python.html)


## Screenshot

See a running example with at least 3 concurrent process windows here:

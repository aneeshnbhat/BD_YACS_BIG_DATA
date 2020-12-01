# BD_YACS_BIG_DATA
This project is about scheduling different tasks on multiple machines. A job is made of one or more tasks.This scheduling framework receives job requests and launches the tasks in the jobs on the machines in the cluster.As and when a task finishes exectution, the scheduling framework is informed, and the resources are freed. The framework can threreafter assign these freed resources to other tasks.
First run worker.py ( this must be run as many times as the numbers of workers in config.json)
syntax: python worker.py port_num worker_id
Then run master.py
syntax: python master.py config.json name_of_scheduler(RR,LL,RANDOM)
Then run request.py
syntax: python request.py number_of_jobs
Once all of the jobs have completed exectution
Then run analysis.py

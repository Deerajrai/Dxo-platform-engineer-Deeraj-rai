DXO Platform Engineer – Technical Assignment

Hi, I’m Deeraj Rai. This repository contains the work I did for the DXO Platform Engineer technical round.

I’ve tried to keep everything as close to a real-world setup as possible. The goal was to show how I approach problems, build infrastructure, automate processes, and keep things running reliably.

What This Project Is About
The assignment asked me to:
	•	Set up two Linux servers (I used Ubuntu)
	•	Install web servers on both and make sure they serve a simple HTML page
	•	Create a PostgreSQL database with a table that holds one line of random content
	•	Pull that data and show it dynamically on the web page
	•	Add a Load Balancer to route traffic to both servers evenly
	•	Make sure the web servers are resilient – meaning they restart automatically if they crash

All of this had to be done using Infrastructure as Code and automation.

How I Did It :-
I used Terraform to set up the infrastructure – that includes the servers, the database, networking, and the Load Balancer.

Then I used Ansible to handle configuration – installing the web server, enabling it to start on boot, setting up the database, and getting the HTML page to show both “Hello World” and the content from the database.

For the self-healing part, I added a small script and system service to restart the web server automatically if it stops.

About the Branches

I’ve kept two branches:-
	•	main – this has the final, clean version of the code that I would actually use in production
	•	recover-infra (dev) – this was my working branch where I tried things out, made mistakes, fixed them, and slowly built towards the final solution

I left the dev branch here so you can see how I worked through the task step by step. I didn’t want to just show the perfect end result — I wanted you to see how I think and build.

Why I Think This Shows I’m a Good Fit 
This task covers the kind of work I do regularly. Writing infrastructure code, automating configuration, handling failures, and making systems that are stable and repeatable — these are all things I’m comfortable with.

What I tried to show here is:
	•	I know how to structure a project properly
	•	I can break down a requirement and implement each part in a clean and automated way
	•	I think about reliability and real-world operations
	•	I’m used to working in a team setup with branches, testing, and clean handoffs
I didn’t try to overcomplicate anything — just kept it simple, readable, and focused on getting the job done right.

During Reviewing This
Start with the main branch — that’s where the final version is. You’ll find:
	•	Terraform code under the infra/ folder
	•	Ansible automation under the main/roles-web/tasks/main.yml / folder
	•	Self-healing scripts and instructions included
	•	A sample SQL file and template for the dynamic HTML content
If you want to see how I built up to this, feel free to check out the dev branch.

Thanks for taking the time to go through my work. I enjoyed working on this task because it closely matches what I enjoy doing — solving problems with clear, reliable automation and infrastructure design.

Thanks and regards,
Deeraj Rai

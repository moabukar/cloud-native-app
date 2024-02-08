#  K8s Experts Tech Test

This task has been assigned to you to get to know you better as a DevOps Engineer before the technical interview. <br>
Besides its basic requirements, consider this task as open-ended. It's meant to show that you know your way around Terraform and that you conceptually understand the architecture of cloud infrastructure, but it is also your opportunity to show off your skills and to let us know what you can bring to the team beyond that to make it better.

## Assignment 

The present assignment has to be commited to this very same repository. Feel free to alter its structure as you see fit to accomodate your vision of the solution. <br>

In this scenario you are provided with a simple html file that represents a client's web application. <br>
We want you to use **Terraform** to deploy this application using a webserver of your choice. The website has to show some value that is fetched from the backend side and loaded **dynamically** in it (e.g.: the webserver's ip, the container ID, the port used, some secret stored in the cluster, some random file in a storage resource, a value from a DB... anything you want!). How you will generate and serve this dynamic value is up to you, but keep in mind that you won't be judged on your skills as web developer, so just make it simple and functional. <br>
The webserver you choose has to be deployed in some cloud **container orchestration** system, preferably in AWS (for example Fargate or EKS), and publicly accessible for us at the time of the interview.

Add a **short technical document** with an architectural diagram of the infrastructure you deployed and explain briefly the reasons for your design choices. <br> 
You don't need to keep this README file, you can delete the contents of it to use it for your documentation if you want. <br>
Please include a rough measurement of how long it took you to complete each part of the task.

That's it!


## Bonus points

These are barely suggestions and not required at all, but if you want to brag a bit and show us the true extent of your capabilities, here are some ideas of things that would make us raise our eyebrows and smile:

- Make the code modular and reusable.
- Show us you know your way around CI/CD tools: Add pipelines to automate things like app deployment, image building, code linting, etc. <br>
  If you will, consider not only what'd make your life easier but also pipelines the devs will need when making changes to the website.
- Include a CDN service.
- Include any SRE tools you like (e.g.: monitoring, logging, alerting, etc [^1]). Present your ideal toolset that would make you feel confindent that you'd know instantly if the app goes down and that you'd have all the info you need to troubleshoot it easily.
- Make code that would support scaling, resiliency, high availability, backups, etc, if that were to be needed.[^1]
- Include a (short) technical document explaining what things you'd make differently if this were a 3-tier microservices app instead of just a POC.

You are expected to dedicate a few hours of your afternoon for the  basic challenge, so don't feel pressured to make **all** (or any!) of these bonus points. If you do know how to do these things but don't have the time to actually do the code for them, you can just explain in a technical document how you'd do it and we can discuss it further in the technical interview.


[^1]: Use a sandbox or demo AWS account. Make sure to delete resources once you are finished and set budgets for your AWS account. Keep screenshots of working app in a directory called `images` in this repo

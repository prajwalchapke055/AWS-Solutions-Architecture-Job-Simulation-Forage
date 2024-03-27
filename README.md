# AWS-Solutions-Architecture-Job-Simulation-Forage
Design a scalable hosting architecture for your client who is experiencing significant growth as a Solutions Architect at AWS.

## Task 1: Designing a simple, scalable, hosting architecture

**Draft your email to Lilly**
Okay let's get started on the email to Lilly. In the email, you will need to show an architecture diagram and explain: 
  what each part of the architecture is,
  why it was chosen, and
  how the costs are calculated and how they may vary month-to-month - remember you don’t need to give concrete numbers, just an overview!

Your team has come together and decided on the architecture approach. Outlined below is all the information you need to draft your email - you can also refer back to Step 2 to learn about AWS services. 

**Read the information and write your response in the text box below. Your response should be approx. 600-700 words.**

We'll show you an example answer on the next step, but we encourage you to give it a go first! 

### First - Your team considers the brief:

When deciding on the right AWS solution, your team considers these points:

The company is a startup. We are lucky because we can provide more of a greenfield approach, and they are more likely to be able to make changes to their application stack. Compared to an enterprise, where change can take a long time, and they may end up only being able to migrate part of their system at a time.
Again, being a startup, it is probably easy to migrate their data into AWS.
They have a single server and already experience downtime, so they are probably OK with some downtime during migration and setup.
Being a mixed API and web app they will need to host some static content as well.

### Second - You decide on the solution: 

In this case, we will recommend a solution based on Elastic Beanstalk based on these requirements:
  The customer has a Python application that Elastic Beanstalk has support for.
  The customer will need to scale, and this is one of the fundamental features of Elastic Beanstalk.
  They want to remove downtime when deploying and Elastic Beanstalk’s Blue/Green deployment can assist with this.
  The AWS Elastic Beanstalk documentation provides some more information if you want to learn about it! 

### Third - Specify the services: 

The services we will use are listed below: 
  Route 53
  Elastic Load Balancing
  Elastic Beanstalk with Autoscaling EC2 Group
  RDS
  S3
  CodePipeline
An additional availability zone for redundancy is proposed but is not necessary.

### Fourth - Evaluate!

Importantly, the team recognizes that Elastic Beanstalk is not the only product that we could recommend for this customer! AWS is an open platform and encourages creativity when building solutions. We need to be aware of the pros and cons of each solution and how they will best fit each customer.

Other options like Lambda or Fargate can be more complex to set up. Lightsail and EC2 can be easy but they don’t provide that automatic scaling; the customer can end up paying more because they are running virtual machines that are often not at capacity. However, each of these services also has its own advantages, and depending on the application that’s being built we can provide different recommendations and discuss the options more in-depth with the customer before coming up with the final design.

Here is the architecture diagram that your team creates for Lilly : 
![Architecture Diagram](https://github.com/prajwalchapke055/AWS-Solutions-Architecture-Job-Simulation-Forage/assets/122814333/37501aba-012a-452f-a04e-7623ce5a84c6)

## CHECK OUT THE SIMULATION HERE : [Job Simulation Link](https://www.theforage.com/simulations/aws-apac/solutions-architecture-ts4o)

## CERTIFICATE OF COMPLETION : 
![AWS APAC Solutions Architecture Completion Certificate_page-0001](https://github.com/prajwalchapke055/AWS-Solutions-Architecture-Job-Simulation-Forage/assets/122814333/767fd46f-1c39-4e55-820b-b58497c46b5e)



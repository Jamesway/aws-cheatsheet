# AWS GUI Cheatsheet
# VPC
Most things on AWS create their own VPC, but its a good idea to make your own from the start so you can isolate your instances from the rest of AWS and secure them.

## We'll be using a few networking things that are under VPC
(Without the Wizard)
1) Create a VPC...
- the wizard won't let you create a vpc without an elastic ip. if you go that route, get an elastic ip first

2) Subnets
Add a public and private Subnets

3) Internet Gateway to public Subnets

4) Nat gateway to Private Subnets

5) Add routing table
add an route for the world into the internet gateway
add the subnets to the routing table


6) create security groups for web, db, ssh ... whatever you need

7)

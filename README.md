# Service Patterns

An experiment in displaying service patterns a linking assets, content, etc.

## The CAPTCHA Pattern

### Example of a CAPTCHA 
![Example of CAPTCHA](/images/captchasample.png)

### What is it? 
A CAPTCHA (a backronym  for "Completely Automated Public Turing test to tell Computers and Humans Apart") is a type of challenge-response test to determine whether or not a user is human. CAPTCHA’s are used to protect digital services from spam robots.  

The most common CAPTCHA requires that the user type the letters of a distorted image, sometimes with the addition of an obscured sequence of letters or digits that appears on the screen. To make a CAPTCHA accessible an audio layer should be included. 

> Check: is this pattern for you? 
> Put in CAPTCHA when your service requires anonymous users, i.e., not logged in, to submit (personal or non-personal) information.  Especially highly valued and frequently used services are at a higher risk of spam attacks.  

> Warning: Due to advances in computer vision technologies, common CAPTCHA solutions can be broken if the attacker is determined enough.  Complimentary security controls should be used in conjunction with CAPTCHA if the digital service is a very high value target.

### Why use this design pattern? 
1.	This pattern has passed STRA (Security Threat and Risk Assessment). Most government services require to fill in personal information. Most CAPTCHA services delivered by third parties contain Terms of Use that do not fit with the security guidelines in place (ie. Google’s ReCAPTCHA). 
1.	This pattern meets the Government standards for accessibility. 
1.	This pattern has been proven in high risk production deployments. 

### How does a ‘good’ CAPTCHA behave? 
A good CAPTCHA is nuanced in its design.  Its a fine balance of  not being too easy so robots can break them easily but not too hard so people find it difficult.  Consideration for a good CAPTCHA: 
-	Is not too long 
-	Should contain a clear image (if an image is used)
-	Has a task that is not too onerous 
-	Does not use upper and lower casing, just upper or lower casing 
-	Contains no common letters that appear the same (ie. I and l, o and 0) 
-	Is made accessible with an audio layer

### Where to use this design pattern? 
From a flow perspective, the best place to put a CAPTCHA is right before the user submits their (personal or non-personal) information at the end of a workflow/transaction.  

### I want to use this pattern 
This reference documentation shows you the design pattern for CAPTCHA:

-	Service Component: [MyGovBC-CAPTCHA-Service](https://github.com/bcgov/MyGovBC-CAPTCHA-Service) 
-	User Interface Component [MyGovBC-CAPTCHA-Widget](https://github.com/bcgov/MyGovBC-CAPTCHA-Widget)
-	Demo (link coming) 

### Discuss this pattern 
[Raise an issue in GitHub to discuss](https://github.com/bcgov/service-patterns-temp/issues)

 





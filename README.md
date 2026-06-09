# AWSporject-1sttierArchitecture
AWS

<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Website Delivery with CloudFront

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-cloudfront)

**Author:** Oluwaseni Oguntonade  
**Email:** seniade490@gmail.com

---

## Website Delivery with CloudFront

![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_1dddddwe)

---

## Introducing Today's Project!

In this project, I will demonstrate how to setup a S3 bucket using AWS console... I'm doing this project to learn cloudfront and web develoment in AWS...

### Tools and concepts

Services I used were cloudfront and S3 bucket... Key concepts I learnt include content delivery network (CDN), Origns, OAC's and Policy...

### Project reflection

This project took me approximately 6 hours... The most challenging part was I could not run my cloud.net from my browser... It was most rewarding to know how AWS actually works, I work as an IT administrator, I think I am confident with the skillset upgrade...

I chose to do this project today because AWS is the most essential part of cloud infrastucture... Something that would make learning with NextWork even better is always learning with the community...

---

## Set Up S3 and Website Files

I started the project by creating an S3 bucket to store all my files... I can't use CloudFront for this task because cloudfront does not work as a storage capacity but as a distributed edge by region within a network...

The three files that make up my website are index.html, which is my main executable file... style.css , which is my css file used to render styles to the project... and script.js, which is used to provide dynamic and responsive page rendering and layout ...

I validated that my website files work by first downloading them by saving the link files and by opening it with the browser, I also launched it through the browser to see the user interactive content...

![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_qgo7wcd3)

---

## Exploring Amazon CloudFront

Amazon CloudFront is a content delivery network, which means it speeds up the distribution of your static and dynamic web content such as .html, .css, .js and image files ... Businesses and developers use CloudFront because CloudFront caches website content in multiple servers around the world. When a user requests content that you're serving with CloudFront, the request is routed to the edge location that provides the lowest latency (time delay), so content is delivered with the best possible performance.

To use Amazon CloudFront, you set up distributions, which are set of instructions that tell how to deliver your content... I set up a distribution for security standards and how my website should be cached ... The origin is nextwork-three-tier-name-123985823271193.s3.eu-north-1.amazonaws.com...

My CloudFront distribution's default root object is nextwork-three-tier-name-123985823271193

 ... This means I can access all my work files from the internet through cloudfront... Setting up my distribution in cloudfront nextwork-three-tier-name-123985823271193 to use all edge locations.



![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_qgo7wcdt)

---

## Handling Access Issues

When I tried visiting my distributed website, I ran into an access denied error because of access and permissions to pick and run real time on the files wiithin the specified and configured S3 buckets.

My distribution's origin access settings were public... This caused the access denied error because setting the origin access to public doesn't automatically update the permissions of the objects in your S3 bucket - for security, the objects are private by default. You'll still need to go to your S3 bucket and set all your objects to public for everyone to access them.
So, even if origin access is public, CloudFront can't access your website's content until your objects' access settings are also set to public.

To resolve the error, I set up origin access control (OAC). OAC is an origin access control (OAC). An OAC lets you keep your S3 bucket and objects not publicly accessible, while still making sure they can be accessed through CloudFront.

OAC also gives you granular control over how CloudFront accesses the content. ...

![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_egrhntyu)

---

## Updating S3 Permissions

Once I set up my OAC, I still needed to update my bucket policy because The OAC's role is that it makes sure only CloudFront can access the files stored in the S3 bucket. For this restricted access to be effective, the S3 bucket's policy still needs to explicitly grant the OAC permission to the bucket's contents.

Creating an OAC automatically gives me a policy I could copy, which grants permissions to cloudfronts to access any document from within the S3 bucket without making the S3 bucket public to everyone...

![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_eg98ntyu)

---

## S3 vs CloudFront for Hosting

---

## S3 vs CloudFront Load Times

---

---



<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Website Delivery with CloudFront

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-networks-cloudfront)

**Author:** Oluwaseni Oguntonade  
**Email:** seniade490@gmail.com

---

## Website Delivery with CloudFront

![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_1dddddwe)

---

## Introducing Today's Project!

In this project, I will demonstrate how to setup a S3 bucket using AWS console... I'm doing this project to learn cloudfront and web develoment in AWS...

### Tools and concepts

Services I used were cloudfront and S3 bucket... Key concepts I learnt include content delivery network (CDN), Origns, OAC's and Policy...

### Project reflection

This project took me approximately 6 hours... The most challenging part was I could not run my cloud.net from my browser... It was most rewarding to know how AWS actually works, I work as an IT administrator, I think I am confident with the skillset upgrade...

I chose to do this project today because AWS is the most essential part of cloud infrastucture... Something that would make learning with NextWork even better is always learning with the community...

---

## Set Up S3 and Website Files

I started the project by creating an S3 bucket to store all my files... I can't use CloudFront for this task because cloudfront does not work as a storage capacity but as a distributed edge by region within a network...

The three files that make up my website are index.html, which is my main executable file... style.css , which is my css file used to render styles to the project... and script.js, which is used to provide dynamic and responsive page rendering and layout ...

I validated that my website files work by first downloading them by saving the link files and by opening it with the browser, I also launched it through the browser to see the user interactive content...

![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_qgo7wcd3)

---

## Exploring Amazon CloudFront

Amazon CloudFront is a content delivery network, which means it speeds up the distribution of your static and dynamic web content such as .html, .css, .js and image files ... Businesses and developers use CloudFront because CloudFront caches website content in multiple servers around the world. When a user requests content that you're serving with CloudFront, the request is routed to the edge location that provides the lowest latency (time delay), so content is delivered with the best possible performance.

To use Amazon CloudFront, you set up distributions, which are set of instructions that tell how to deliver your content... I set up a distribution for security standards and how my website should be cached ... The origin is nextwork-three-tier-name-123985823271193.s3.eu-north-1.amazonaws.com...

My CloudFront distribution's default root object is nextwork-three-tier-name-123985823271193

 ... This means I can access all my work files from the internet through cloudfront... Setting up my distribution in cloudfront nextwork-three-tier-name-123985823271193 to use all edge locations.



![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_qgo7wcdt)

---

## Handling Access Issues

When I tried visiting my distributed website, I ran into an access denied error because of access and permissions to pick and run real time on the files wiithin the specified and configured S3 buckets.

My distribution's origin access settings were public... This caused the access denied error because setting the origin access to public doesn't automatically update the permissions of the objects in your S3 bucket - for security, the objects are private by default. You'll still need to go to your S3 bucket and set all your objects to public for everyone to access them.
So, even if origin access is public, CloudFront can't access your website's content until your objects' access settings are also set to public.

To resolve the error, I set up origin access control (OAC). OAC is an origin access control (OAC). An OAC lets you keep your S3 bucket and objects not publicly accessible, while still making sure they can be accessed through CloudFront.

OAC also gives you granular control over how CloudFront accesses the content. ...

![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_egrhntyu)

---

## Updating S3 Permissions

Once I set up my OAC, I still needed to update my bucket policy because The OAC's role is that it makes sure only CloudFront can access the files stored in the S3 bucket. For this restricted access to be effective, the S3 bucket's policy still needs to explicitly grant the OAC permission to the bucket's contents.

Creating an OAC automatically gives me a policy I could copy, which grants permissions to cloudfronts to access any document from within the S3 bucket without making the S3 bucket public to everyone...

![Image](http://learn.nextwork.org/easygoing_beige_jolly_ostrich/uploads/aws-networks-cloudfront_eg98ntyu)

---

## S3 vs CloudFront for Hosting

---

## S3 vs CloudFront Load Times

---

---

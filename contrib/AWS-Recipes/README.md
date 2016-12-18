From Ken-Tune, https://github.com/ken-tune/MarkLogic-AWS-Recipes

Please find attached some hopefully useful assets

•	A parameterized cloud formation template for setting up a VPC (Virtual Private Cloud) consisting of three external and three internal subnets across three different AZs with all necessary ACLs, NATing, Security Groups and ‘jump boxes’ to access internal resources

•	A parameterized cloud formation template allowing setup of a three zone MarkLogic cluster in a VPC such as the one above ( though not limited to that )

•	A document discussing the templates, what they do and how to use them

The MarkLogic setup template as well as dealing with VPCs includes a couple of small additions to the standard template including automated setup of an SNS topic for diagnostic messages and creation of an IAM role for the MarkLogic instances tailored to their specific requirements (hat tip to Tom Ternquist for adding these to an earlier mail), reducing the ‘pre-requisites’ to just two (SSH key pair and AWS account).

I have posted these as the first part of a GitHub project - https://github.com/ken-tune/MarkLogic-AWS-Recipes (example-1 directory). There are a few other recipes I would like to create building on the work above, and will hopefully find the time to add them to this one.

I hope that this will be found useful as there has been quite a lot of discussion of this topic. As is usually the case, I have built on the work of others and appreciate particularly that of David Lee.

Ken


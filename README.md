# Lab 3
[Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repo and clone it to your machine to get started!

## Team Members
- Diego Garcia
- team member 2

## Lab Question Answers

Answer for Question 1: Why are RESTful APIs scalable?

RESTful APIs are scalable because they optimize client-server interactions through statelessness, which reduces server load by eliminating the need for it to retain past client request information, and well-managed caching which can partially or completely eliminate some client-server interactions. These features support scalability and prevent communication bottlenecks that can negatively impact performance.

Answer for Question 2:According to the definition of “resources” provided in the AWS article above, what are the resources the mail server is providing to clients?

The resources that the mail server is providing to clients would be information related to email, such as email messages, contacts, and folders. The mail server is the machine that provides these resources to clients, and the API helps to ensure that the resources are shared securely, with control and authentication in place to determine which clients get access to specific internal resources.

Answer for Question 3: What is one common REST Method not used in our mail server? How could we extend our mail server to use this method?

A common REST method not used in the mail server is the POST method. To extend the mail server to use the POST method, we could append the 'data' obtained from the GET request to an endpoint that accepts POST requests through a json-encoded payload. This is a convenient method provided by Flask's request object that parses the json payload and return it as a python dictionary.Then, the server could access data sent by a client and is able to create a new entry in the 'mail' database.

Answer for Question 4: Why are API keys used for many RESTful APIs? What purpose do they
serve? Make sure to cite any online resources you use to answer this question!

API keys are used to identify the calling client and provide access to the resources associated with the key. They are used for many RESTful APIs because it allows the server to control the level of access granted to each lcient, which is useful for limiting the amount of data that is returned in response to a request. It is a great form of access control.


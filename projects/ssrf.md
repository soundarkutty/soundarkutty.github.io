What is SSRF?

SSRF stands for server-side request forgery. It is one of the most popular web security vulnerabilities exploited by hackers and security researchers.

It is a security vulnerability where an attacker can abuse the available functionalities in a server-side application to access internal server files, resources leading to potentially sensitive information disclosure.
How does it work?

In modern-day applications, it is common to find functionalities that communicate with internal servers, access resources, etc.

If any functionality is vulnerable to SSRF attacks then an attacker can manipulate the address of the requested resource and get access to it easily.
What causes SSRF?

To access resources in a machine, we always need to specify a unique address. It can be an HTTP URL or simply a file path. The outcome is based upon our input we give as the address.

There are instances where an application trusts the server itself for requesting, modifying resources and in that case, if there is a request having the address of the needed resource, an attacker can modify it to make the application access resources other than what is needed in the context of that user session.

The same can be done if the application has trust built over any external backend server i.e. any server that is not the one where the application is hosted at.

Let’s understand it better through some visuals: There are functionalities where the application is supposed to be communicating with a server and access resources.

 Types of SSRF

Non-Blind SSRF: This is a type of SSRF where an application fetches the requested resource and directly presents it on the front end. The whole output is clearly visible to the user/attacker.

Blind SSRF: This is an interesting and very common type of SSRF where the HTTP request for requesting resources is made by the server but the output isn’t visible on the frontend. In simple words, the resource is requested by the server but not displayed to the user/attacker. There are certain ways of exploiting this type of SSRF vulnerabilities and we will cover them further in this blog.

Semi-blind SSRF: In this type of SSRF, a resource is requested but the complete output isn’t visible to the user but instead it can be file metadata, parts of the file, complete file path in the form of stack trace errors, and more.

This is called semi blind because the data is partially available, unlike blind SSRF where nothing is visible on the frontend. To exploit semi-blind SSRF, similar ways of exploiting blind SSRFs can be used.

Exploitation

We will now cover the exploitation of the different types of SSRF cases explained above. Keep in mind that there can be unique methods of exploiting SSRF because the behavior of the application matters a lot while exploiting and validating security issues so a straightforward method may not always work.


# Web-Crawler
A Web Crawler is a piece of software that automatically gathers and traverses documents on the web.
This project is designed to crawl on a class website called fakebook to engage in a capture the flag activity.

High-level Approach:
    First, the project established a web socket to connect to the network. Then it sends a GET request to the website and retrieve relevant information from the retrieved data (cookies, data, etc).
    Project also redesigned a HTML Parser to read the crsf token from the retrieved data.
    Then the project sends a POST request to login into fakebook. Once the code is logged in, we start crawling.
    This process is mainly keeping track of links that are in queue and those that has been visited while also looking for the flag inside the links.

Challenges:
    I had troubles at first trying to figure out how to start since I didnot know about the cookies and token or parser, etc.
    I resolves this by reading through some HTML documents and follow some instructions on communicating with HTML.
    I also needed to spend some time inspecting the elements of fakebook to figure out the 'set-cookie' tags or cookies tags.

Testings:
    I mostly run the code in the Khoury Linux virtual machine and I try to run it a lot of time to try to estimate the time needed to fully get all 5 flags
    Another is simply submit the project onto Gradescope and see for results.

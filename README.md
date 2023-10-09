# b9122_homework2
Author information: Qiantong Li, Columbia Business School, Master of Science in Accounting and Fundamental Analysis, ql2471

Description of the code files
Q1-1: I use two methods to write web crawlers.
(1) bs4 method: Firstly, I install lxml and import bs4 and requests, and then unction to check if a given page is a press release. During the process, I pay attention to keep track of visited URLs and make queue initialized with the start URL. After that, I extract links to enqueue and Properly join the base URL with the href. However, although this method is related more to class, it takes more time to run on my computer.
(2) scrapy method: Firstly, I install and import scrapy, and then define the spider class, and counter for the number of press releases found containing the word "crisis". After that, I extract all links and recursively scrape them. I also configure settings and run the spider. These codes run more smoothly on my computer and take less time.

Q1-2: bs4 and requests
After importing requests and bs4, I set up caching and perform a search with the same URL. During the process, I send a GET request using search keywords, and initialize a queue based on search results, and add the first max_pages pages to the queue.

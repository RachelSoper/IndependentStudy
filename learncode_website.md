import markdown 

md = markdown.Markdown([
    "markdown.extensions.wikilinks(base_url=, end_url=.html)",
    "markdown.extensions.tables",
    "markdown.extensions.fenced_code"]
)

text = """

![]("http://futurefocusfoundation.us/wp-content/uploads/2016/07/coding.jpg")


# Interactive Websites That Teach Users How To Code


## 10 Most Popular Websites
*   [Codecademy](https://www.codecademy.com/)
*   [Code Avengers](https://www.codeavengers.com/)
*   [Code School](https://www.codeschool.com/)
*   [Treehouse](https://teamtreehouse.com)
*   [Udacity](https://www.udacity.com/)
*   [CodeHS](https://codehs.com/)
*   [Khan Academy](https://www.khanacademy.org/computing/computer-programming)
*   [SQLZOO](http://sqlzoo.net/)


## Website Comparison

### Codecademy
*  Courses: HTML, CSS, JavaScript, jQuery, PHP, Ruby, Python, API
*  Fature: Code Interpreter, Progress Saver, Project, Forum			
*  Price: Free 										
*  Difficulty: Easy – Intermediate
	
### Code Avengers	
*  Courses: HTML5, CSS3, JavaScript
*  Fature: Code Interpreter, Progress Saver, Project, Note			
*  Price: Free 										
*  Difficulty: Easy
	
### Code School	
* Courses: HTML5, CSS, CSS3, jQuery, Ruby, Ruby on Rails, iOS
* Fature: Code Interpreter, Screencast, Progress Saver, Project, Forum			
* Price: Free, $25/month							
* Difficulty: Intermediate - Hard

### Treehouse     
* Courses: HTML, CSS, CSS3, JavaScript, jQuery, Ruby, Ruby on Rails, iOS, Android, UX, Database
* Fature: Code Interpreter, Screencast, Progress Saver, Project, Forum				
* Price: ree, $25/month, $49/month	 										
* Difficulty: Easy – Hard	
	
### Udacity
* Courses: Web Development, HTML5, Python, Java, Computer Science, Algorithm, AI
* Fature: Code Interpreter, Screencast, Progress Saver, Forum									
* Price: Free 										
* Difficulty: Intermediate – Extremely Hard
	
### CodeHS        	
* Courses: Problem Solving, JavaScript, Animation, Game Programming
* Fature: Code Interpreter, Screencast, Progress Saver					
* Price: Free, $25/month, $75/month									
* Difficulty: Easy – Intermediate
	
### Khan Academy
* Courses: Programming Basics, Canvas Drawing, Animation, User Interaction
* Fature: Code Interpreter, Screencast, Progress Saver, Project, Discussion			
* Price: Free 										
* Difficulty: Easy – Intermediate
	
### SQLZOO
*  Courses: SQL	
*  Fature: Code Interpreter		
*  Price: Free 										
*  Difficulty: Easy – Hard

"""

html = md.convert(text)
print(html)

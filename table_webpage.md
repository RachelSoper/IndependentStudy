import markdown 

md = markdown.Markdown([
    "markdown.extensions.wikilinks(base_url=, end_url=.html)",
    "markdown.extensions.tables",
    "markdown.extensions.fenced_code"]
)

text = """

![](http://www.cbronline.com/wp-content/uploads/2017/03/programming-languages.jpg)

# Using Python Markdown to Create a Webpage


Programming Language | Creator |
--- | --- |
Java | James Gosling |
C | Dennis Ritchie |
C++ | Bjarne Stroustrup |
Python | Guido Van Rossum |
PHP | Rasmus Lerdforf | 
Perl | Larry Wall |
JavaScript | Brendn Eich |
Ruby | Yukihiro Matsumoto |

"""
html = md.convert(text)
print(html)

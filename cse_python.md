
import markdown 

md = markdown.Markdown([
    "markdown.extensions.wikilinks(base_url=, end_url=.html)",
    "markdown.extensions.tables",
    "markdown.extensions.fenced_code"]
)

text = """
![]("http://highdesertdaily.com/wp-content/uploads/2011/12/csusb4.jpg")

##__Welcome To__##

#School of Computer Science and Engineering#

The School of Computer Science and Engineering educates students in the disciplines of computing theory and machinery, and teaches them to apply their knowledge in a socially responsible way. 
The School educates  students in the intellectual basis of the field, including issues of computability, information theory, and engineering, as well as the technology.  Our graduates can design and 
implement the technology of computing and data communications	with a deep understanding of the bases upon which these technologies rest.  In addition to preparing professional workers for 
industry, we educate those students who wish to pursue an advanced degree or career in academic or industrial research. Students may study for the BS or MS in Computer Science, the BS in 
Computer Engineering, the BS in Bioinformatics, or the BA in Computer Systems.

The Bachelor of Science in Computer Science and the Bachelor of Science in Computer Engineering programs are both accredited by [Extermal Link]( http://www.abet.org/wp*signup.php?new=abet.org "ABET").

##Degree Pograms##
* [Bachelor of Science in Computer Science]( https://cns.csusb.edu/cse/bs-computer-science )
* [Bachelor of Science in Computer Engineering]( https://cns.csusb.edu/cse/bs-computer-engineering )
* [Bachelor of Science in Bioinformatics]( https://cns.csusb.edu/cse/bs-bioinformatics )
* [Bachelor of Arts in Computer Systems]( https://cns.csusb.edu/cse/ba-computer-systems )
* [Minor in Computer Science]( https://cns.csusb.edu/cse/minor-computer-science )
* [Certificate in Computer Systems and Programming]( https://cns.csusb.edu/cse/certificate-computer-systems-and-programming )
* [Master of Science in Computer Science]( https://cns.csusb.edu/cse/ms-computer-science )

##Department Information##
####Faculty and Staff####
* [Full-Time Faculty](https://cns.csusb.edu/cse/faculty-staff)
* [Emertius Faculty](https://cns.csusb.edu/cse/faculty-staff)
* [Part-Time Faculty](https://cns.csusb.edu/cse/faculty-staff)
* [Staff](https://cns.csusb.edu/cse/faculty-staff)

####Other Information####
* [Industry Advisory Board]( https://cns.csusb.edu/cse/industry-advisory-board )
* [Faculty Office Hours]( https://cns.csusb.edu/sites/default/files/cse-office-hours.pdf )
*  [Contact Us]( https://cns.csusb.edu/cse/contact ) 
* Contact Information
	Phone: (909) 537-5326
	Fax: (909) 537-7004
	Location: Jack Brown Hall, Room 307



##Student Resources##
* [Forms]( https://cns.csusb.edu/cse/forms) 
* [Course Schedule]( https://cns.csusb.edu/cse/courses )
* [Student Organizations]( https://cns.csusb.edu/cse/student-organizations ) 
"""

html = md.convert(text)
print(html)

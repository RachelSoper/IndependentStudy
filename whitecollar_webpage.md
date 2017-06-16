
import markdown 

md = markdown.Markdown([
    "markdown.extensions.wikilinks(base_url=, end_url=.html)",
    "markdown.extensions.tables",
    "markdown.extensions.fenced_code"]
)

text = """

![](https://upload.wikimedia.org/wikipedia/commons/0/06/White_Collar_2009_logo.svg)

#### USA Network Tv Series
#####  2009 - 2014

[White Collar Webite](http://www.usanetwork.com/whitecollar)


WHITE COLLAR focuses on the unlikely partnership between the very intelligent and charming con-artist Neal Caffrey (Matt Bomer) and the hard-working and earnest FBI agent Peter Burke (Tim DeKay, “The New Adventures of Old Christine”).  In exchange for his freedom, and on the condition that he wear an ankle bracelet at all times, Caffrey provides his expertise in thievery to help Burke and agents Clinton Jones (Sharif Atkins,) and Diana Berrigan (Marsha Thomason) catch other elusive white collar criminals. 



## Season 1  
![](https://img.yescdn.ru/2016/07/05/poster/ae95ba86f31b83d1509bcb0ab507736e-white-collar-season-1-1467737925.jpg) 
Neal Caffrey is a criminal mastermind who is serving a four-year prison sentence. He earns a conditional release into FBI custody and forges a relationship with FBI Special Agent who put him in jail, Peter Burke. Using his vast knowledge of criminal activity, Neal assists Peter in solving a series of white collar crimes while also searching for his girlfriend who has disappeared.


## Season 2
![](https://vignette1.wikia.nocookie.net/whitecollar/images/2/2b/WhiteCollarS2-5.jpg/revision/latest?cb=20101221235706) 
Season 2 begins as Peter Burke is investigated by the FBI for his role in the alleged escape attempt by Neal and the disappearance of Fowler. Neal is dealing with the death of his girlfriend Kate, while back in prison due to the temporary suspension of his release into FBI (Peter's) custody.


## Season 3
![](https://vignette2.wikia.nocookie.net/whitecollar/images/5/5c/S3poster.jpg/revision/latest?cb=20110507123152) 

## Season 4
![](https://vignette1.wikia.nocookie.net/whitecollar/images/2/26/S4Poster2.jpg/revision/latest?cb=20120613165115) 

## Season 5
![](https://vignette1.wikia.nocookie.net/whitecollar/images/a/a6/S5Poster.jpg/revision/latest?cb=20131003212440) 
Season 5 picks up after the shocking arrest of FBI agent Peter Burke on murder charges. Neal Caffrey must make a deal with the devil to help clear his name.

## Season 6
![](https://vignette1.wikia.nocookie.net/whitecollar/images/0/0f/S6-Promo.jpg/revision/latest?cb=20140912184645) 
The thrilling final season picks up on last season’s cliffhanger, when Caffrey has disappeared, sans ankle bracelet. Personal transitions and returning enemies complicate things when Caffrey and Agent Burke are pitted against the most sought-after network of criminals in the world, the Pink Panthers. With the help of Mozzie (Garson) and FBI agents, Barrigan and Jones, they will attempt to infiltrate and bring down the infamous criminal ring. Guest stars for the final bow include Ross McCall, Gavin Lee, Bridget Regan, Toby Leonard Moore, Paloma Guzman, Michael Potts, Isaach de Bankole and Diahann Carroll.

"""
html = md.convert(text)
print(html)

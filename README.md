<div align="center">

## Form to submit a URL to search engines


</div>

### Description

Create a form that will submit a URL to the search engines. Submision to 24 search engines is supported.

The code includes both a form and a response file. Both may be customized.

This first form should be placed in any .asp file.

The 2nd file must be save as "submit.asp" in the cgi-bin directory.

http://www.submitside.com/script/submit/aspsubmit.html
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Found on the World Wide Web](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/found-on-the-world-wide-web.md)
**Level**          |Intermediate
**User Rating**    |4.2 (21 globes from 5 users)
**Compatibility**  |ASP \(Active Server Pages\)
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__4-9.md)
**World**          |[ASP / VbScript](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/asp-vbscript.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/found-on-the-world-wide-web-form-to-submit-a-url-to-search-engines__4-50/archive/master.zip)





### Source Code

```
Copy this form to your page
<FORM METHOD=POST ACTION="/cgi-bin/Submit.asp">
<table border=1 cellpadding=5 bgcolor="#EEEEEE">
<tr><td align=center>
<table>
<tr><td>Your name:</td><td><INPUT name="name" maxlength=256 size=35 type=text></td></tr><tr><td>E-mail:</td><td><INPUT name="email" maxlength=256 size=35 type=text></td></tr><tr><td>Page Title:</td><td><INPUT name="title" maxlength=256 size=35 type=text></td></tr><tr><td>URL:</td><td><INPUT name="url" maxlength=256  size=35 type=text value="http://"></td></tr><tr><td>Description:</td><td><INPUT name="description" maxlength=256 size=35 type=text></td></tr>
</table>
<input type=submit value="Submit"><BR>
<A HREF="http://www.submitside.com/included"><font size=2 color=blue>Search engines included in the submission area</font></A>
</td></tr></table>
</FORM>
The content in this table must be save as "submit.asp" in the cgi-bin directory
<html><head><title>Submission area</title></head>
<body bgcolor="#FFFFFF">
<center>
<BR>
<table border=1 width=480>
<tr><td align=center>
<font size=4>Automatic submission to 10 search engines</font><BR>
<font size=2>
<A HREF="http://altavista.digital.com">Altavista</A>
<A HREF="http://www.excite.com">Excite</A>
<A HREF="http://www.infoseek.com">InfoSeek</A>
<A HREF="http://www.lycos.com">Lycos</A>
<A HREF="http://www.whatuseek.com">What-U-Seek</A> <BR>
<A HREF="http://www.hotbot.com">HotBot</A>
<A HREF="http://webcrawler.com">WebCrawler</A>
<A HREF="http://netfind.aol.com">AOL NetFind</A>
<A HREF="http://www.goto.com/">GoTo.com</A>
<A HREF="http://www.northernlight.com">Northern Light</A></font>
<form method="POST" action="http://www.free-banners.com/cgi-bin/fb/submit/reg.cgi" target="new">
<!-- Free-Banners : http://www.free-banners.com/ -->
<input type=hidden name="engine2" value="2">
<input type=hidden name="engine5" value="5">
<input type=hidden name="engine9" value="9">
<input type=hidden name="engine4" value="4">
<input type=hidden name="engine7" value="7">
<input type=hidden name="engine0" value="0">
<input type=hidden name="engine1" value="1">
<input type=hidden name="engine3" value="3">
<input type=hidden name="engine6" value="6">
<input type=hidden name="engine8" value="8">
<input type=hidden name="title" value="<% =REQUEST.FORM("title") %>">
<input type=hidden value="<% =REQUEST.FORM("url") %>" name="url">
<input type=hidden value="<% =REQUEST.FORM("name") %>" name="name">
<input type=hidden value="<% =REQUEST.FORM("email") %>" name="email">
<input type="hidden" name="service" value="Url Submission">
<input type="submit" value=" Submit"><br>
<font size=2>Service provided by
<a href="http://www.free-banners.com" target="newa">Free Banners</a></font>
</form>
</td></tr></table>
<table border=1 width=480>
<tr><td align=center>
<FORM METHOD=GET ACTION="http://www.anzwers.com.au/cgi-bin/print_addurl.pl" target=new2>
<A HREF="http://www.anzwers.com.au">Anzwers</A><br>
<INPUT TYPE=hidden VALUE="<% =REQUEST.FORM("url") %>" name="url">
<INPUT TYPE=hidden VALUE="<% =REQUEST.FORM("email") %>" name="email">
<INPUT TYPE=submit VALUE="Submit">
</form>
</td><td align=center>
<FORM METHOD=POST ACTION="http://magellan.mckinley.com/cgi/add_url.cgi"
ENCTYPE=multipart/form-data target=new3>
<A HREF="http://magellan.mckinley.com">Magellan</A><br>
<INPUT TYPE=hidden NAME="url" VALUE="<% =REQUEST.FORM("url") %>">
<INPUT TYPE=hidden NAME="email" VALUE="<% =REQUEST.FORM("email") %>">
<INPUT TYPE=SUBMIT VALUE="Submit">
</FORM>
</td><td align=center>
<FORM ACTION=http://www.planetsearch.com/ METHOD=GET target=new5>
<A HREF="http://www.planetsearch.com/">PlanetSearch</A><br>
<INPUT TYPE=hidden NAME=a VALUE=20>
<INPUT TYPE=hidden NAME=flags VALUE=3>
<INPUT TYPE=hidden NAME=count VALUE=10>
<INPUT TYPE=hidden NAME=olda VALUE=0>
<INPUT TYPE=hidden NAME=url VALUE="<% =REQUEST.FORM("URL") %>">
<INPUT TYPE=submit value="Submit">
</FORM>
</td><td align=center>
<form action="http://www.infomak.com/add_url.sh" method=GET target=new6>
<A href="http://www.infomak.com">Infomak</A><br>
<input type=hidden name="url" value="<% =REQUEST.FORM("URL") %>">
<input type=hidden name="Page" value="url">
<input type=submit value="Submit">
</FORM>
</td></tr>
</table>
<table border=1 width=480 cols2>
<tr><td align=center>
<form action="http://findlink.com/searchit/bulk-addurl.cgi" method="GET" target=new7>
<input type=hidden name="recipient" value="<% =REQUEST.FORM("EMAIL") %>">
<input type=hidden name="linkaddr" value="<% =REQUEST.FORM("URL") %>">
<select name="category">
<OPTION VALUE="">Select Category
<OPTION VALUE="catx3dx=Arts">Arts
<OPTION VALUE="catx3dx=Automotive">Automotive
<OPTION VALUE="catx3dx=Business">Business
<OPTION VALUE="catx3dx=Chat">Chat
<OPTION VALUE="catx3dx=Computers">Computers
<OPTION VALUE="catx3dx=Education">Education
<OPTION VALUE="catx3dx=Employment">Employment
<OPTION VALUE="catx3dx=Entertainment">Entertainment
<OPTION VALUE="catx3dx=Finance">Finance
<OPTION VALUE="catx3dx=Games">Games
<OPTION VALUE="catx3dx=Gardening">Gardening
<OPTION VALUE="catx3dx=Health">Health
<OPTION VALUE="catx3dx=Internet">Internet
<OPTION VALUE="catx3dx=Kids">Kids
<OPTION VALUE="catx3dx=Life">Life
<OPTION VALUE="catx3dx=Music">Music
<OPTION VALUE="catx3dx=News">News
<OPTION VALUE="catx3dx=Personal_Pages">Personal_Pages
<OPTION VALUE="catx3dx=Realestate">Realestate
<OPTION VALUE="catx3dx=Recreation">Recreation
<OPTION VALUE="catx3dx=Reference">Reference
<OPTION VALUE="catx3dx=Science">Science
<OPTION VALUE="catx3dx=Services">Services
<OPTION VALUE="catx3dx=Shopping">Shopping
<OPTION VALUE="catx3dx=Software">Software
<OPTION VALUE="catx3dx=Sports">Sports
<OPTION VALUE="catx3dx=Travel">Travel</select><BR>
<input type=hidden name="sitename" value="<% =REQUEST.FORM("TITLE") %>">
<input type=hidden name="description" value="<% =REQUEST.FORM("description") %>">
<input type="submit" value="Submit">
<input type=hidden name=submitter value="submitside.com">
<input type=hidden name=submitterhttp value="http://submitside.com">
<a href="http://www.findlink.com/">FindLink</a>
</form>
</td><td align=center>
<form action="http://questfinder.com/search/bulk-addurl.cgi" method="GET" target=new9>
<input type=hidden name="recipient" value="<% =REQUEST.FORM("EMAIL") %>">
<input type=hidden name="linkaddr" value="<% =REQUEST.FORM("URL") %>">
<select name="category">
<OPTION VALUE="">Select Category<OPTION VALUE="catx3dx=Adults_Only">Adults_Only<OPTION VALUE="catx3dx=Advertising">Advertising<OPTION VALUE="catx3dx=Animals">Animals<OPTION VALUE="catx3dx=Arts">Arts<OPTION VALUE="catx3dx=Auctions">Auctions<OPTION VALUE="catx3dx=Business">Business<OPTION VALUE="catx3dx=Chat">Chat<OPTION VALUE="catx3dx=Classifieds">Classifieds<OPTION VALUE="catx3dx=Communications">Communications<OPTION VALUE="catx3dx=Community">Community<OPTION VALUE="catx3dx=Computers">Computers
<OPTION VALUE="catx3dx=Consumer">Consumer<OPTION VALUE="catx3dx=Education">Education
<OPTION VALUE="catx3dx=Employment">Employment<OPTION VALUE="catx3dx=Entertainment">Entertainment<OPTION VALUE="catx3dx=Events">Events
<OPTION VALUE="catx3dx=Ezines">Ezines<OPTION VALUE="catx3dx=Finance">Finance
<OPTION VALUE="catx3dx=Freebies">Freebies<OPTION VALUE="catx3dx=Games">Games<OPTION VALUE="catx3dx=Government">Government<OPTION VALUE="catx3dx=Health">Health<OPTION VALUE="catx3dx=Hobbies">Hobbies<OPTION VALUE="catx3dx=Home">Home<OPTION VALUE="catx3dx=Internet">Internet<OPTION VALUE="catx3dx=Kids">Kids<OPTION VALUE="catx3dx=Legal">Legal<OPTION VALUE="catx3dx=Life">Life<OPTION VALUE="catx3dx=MLM">MLM<OPTION VALUE="catx3dx=Manufacturing">Manufacturing<OPTION VALUE="catx3dx=Medical">Medical<OPTION VALUE="catx3dx=Music">Music<OPTION VALUE="catx3dx=News">News<OPTION VALUE="catx3dx=Personal_Pages">Personal_Pages<OPTION VALUE="catx3dx=Pets">Pets<OPTION VALUE="catx3dx=Products">Products<OPTION VALUE="catx3dx=Publishing">Publishing<OPTION VALUE="catx3dx=Real_Estate">Real_Estate
<OPTION VALUE="catx3dx=Recreation">Recreation<OPTION VALUE="catx3dx=Reference">Reference
<OPTION VALUE="catx3dx=Religion">Religion<OPTION VALUE="catx3dx=Science">Science<OPTION VALUE="catx3dx=Services">Services<OPTION VALUE="catx3dx=Shopping">Shopping<OPTION VALUE="catx3dx=Software">Software<OPTION VALUE="catx3dx=Sports">Sports<OPTION VALUE="catx3dx=Technology">Technology<OPTION VALUE="catx3dx=Transportation">Transportation
<OPTION VALUE="catx3dx=Travel">Travel<OPTION VALUE="catx3dx=Wholesale">Wholesale</select><BR>
<input type=hidden name="sitename" value="<% =REQUEST.FORM("TITLE") %>">
<input type=hidden name="description" value="<% =REQUEST.FORM("description") %>">
<input type="submit" value="Submit">
<input type=hidden name=submitter value="submitside.com">
<input type=hidden name=submitterhttp value="http://submitside.com">
<A HREF="http://www.questfinder.com">QuestFinder</A>
</form>
</tr><tr>
<td colspan=2 align=center>
<BR>
<form action="http://www.webgremlin.com/cgi-bin/links/add.cgi" method="POST" target=new8>
<input type=hidden name="Title" value="<% =REQUEST.FORM("TITLE") %>">
<input type=hidden name="URL" value="<% =REQUEST.FORM("URL") %>">
<SELECT NAME="Category" SIZE=1><OPTION>Select Category<OPTION>Art_and_Graphics<OPTION>Astrology<OPTION>Auctions
<OPTION>Autos_and_More<OPTION>Beauty_and_Fashion<OPTION>Books<OPTION>Business_Opportunities
<OPTION>Careers_and_Jobs<OPTION>Classifieds_Ads<OPTION>Computers<OPTION>Computers/Hardware
<OPTION>Computers/Software<OPTION>Education<OPTION>Electronics<OPTION>Entertainment
<OPTION>Family_Friendly<OPTION>Finance<OPTION>Food_and_Wine<OPTION>Free_Stuff
<OPTION>Gambling<OPTION>Games<OPTION>Games/Computer<OPTION>Games/Nintendo
<OPTION>Games/Playstation<OPTION>Games/Sega<OPTION>Gay<OPTION>General_Interest
<OPTION>Health_and_Fitness<OPTION>Internet_Related<OPTION>Internet_Related/Internet_Tools
<OPTION>Internet_Related/Service_Providers<OPTION>Internet_Related/Website_Design
<OPTION>Internet_Related/Website_Hosting<OPTION>Legal<OPTION>Magazines
<OPTION>Movies_and_Cinema<OPTION>Music<OPTION>NC_17<OPTION>Office
<OPTION>Real_Estate<OPTION>Retail_Sites<OPTION>Romance<OPTION>Romance/Flowers
<OPTION>Romance/Personals<OPTION>Sports<OPTION>Toys<OPTION>Travel<OPTION>Video
<OPTION>Webmasters<OPTION>Webmasters/Adult_Webmasters</SELECT><BR>
<input type=hidden name="Description" value="<% =REQUEST.FORM("description") %>">
<input type=hidden name="Contact Name" value="<% =REQUEST.FORM("name") %>">
<input type=hidden name="Contact Email" value="<% =REQUEST.FORM("EMAIL") %>">
<input type="hidden" name="Rating" Value="0">
<input type="hidden" name="Votes" value="0">
<input type="SUBMIT" value="Submit">
 <a href=" http://www.webgremlin.com ">WebGremlin</a>
</form>
</td></tr></table>
<table><tr>
<td nowrap>
<form action="http://www.websitegarage.com/bin/go" METHOD="POST" target=new11>
<font color="FF0000" face=arial><B><I>Tune Up Your Web Site Free:</I></B></font><br>
<input type="text" name="url" size="20" maxlength="100" value="<% =REQUEST.FORM("url") %>">
<input type="hidden" name="istate" value="start">
<input type="hidden" name="util" value="page_summary">
<input type="hidden" name="banner" value="reff267022e">
<input type="submit" value="Go!">
</form></td></tr></table>
<table border=1 width=480>
<tr><td align=center>
<form method=post action="http://www.submitside.com/cgi-bin/i/add.asp" target=new20>
<SELECT NAME="w">
<option>Select_Category<option>Advertising<option>Agriculture
<option>Animals_Ecology<option>Architecture<option>Arts
<option>Astrology<option>Auctions<option>Beauty_and_Fashion
<option>Books_Magazines<option>Business<option>Careers_and_Jobs
<option>Cars_Motorcycles<option>Chat<option>Computers_Hardware
<option>Computers_Software<option>Computer_Games
<option>Entertainment<option>Events<option>Fiction
<option>Food_Beverage<option>Freebies<option>Gardening
<option>General_Interest<option>Health_Fitness<option>Hobbies
<option>Home<option>Humor<option>Internet<option>Internet_Design
<option>Internet_Freebies<option>Internet_Hosting
<option>Internet_Tools<option>Kids<option>Maps
<option>Miscellaneous<option>Movies<option>Music
<option>News<option>Personal_Pages<option>Photography
<option>Romance_Flowers<option>Romance_Personals
<option>Science<option>Shopping<option>Sports
<option>Technology<option>Travel
</SELECT>
<input type=hidden name=title value="<% =REQUEST.FORM("TITLE") %>">
<input type=hidden name=url value="<% =REQUEST.FORM("url") %>">
<input type=hidden name=description value="<% =REQUEST.FORM("description") %>"><BR>
<input type=submit value="Submit">
<A HREF="http://www.submitside.com/links">Huge Link Page</A>
</form>
</td></tr><tr><td align=center>
<form NAME="aa" action="http://rex.skyline.net/add/add.cgi" method=POST target=new13>
<input type=hidden name=thispage value=2>
<input type=hidden name=cat value="">
<input type=hidden name=catnum value="">
<input type=hidden name=navigate value="">
<input type=hidden name=confirm value="">
<input type=hidden name=urlfail value="">
<input type=hidden name=refer value="http://submitside.com">
<input type=hidden name=url value="<% =REQUEST.FORM("URL") %>">
<input type=hidden name=yourname value="<% =REQUEST.FORM("NAME") %>">
<input type=hidden name=email value="<% =REQUEST.FORM("EMAIL") %>">
<input type=hidden name=name value="<% =REQUEST.FORM("TITLE") %>">
Keywords separated by spaces (select up to 5; 60 characters)<BR>
<input type=text name=keys size=75 maxlength=60 onChange="document.bb.Keywords.value=document.aa.keys.value;document.dd.key.value= document.aa.keys.value "><BR>
<input type=hidden name=desc value="<% =REQUEST.FORM("description") %>">
<input type=submit value="Submit">
<A HREF="http://rex.skyline.net/">Rex</A>
</form>
</td></tr><tr><td align=center>
<FORM NAME="bb" ACTION="http://www.scrubtheweb.com/cgi-bin/addurl.cgi" METHOD="GET" target=new14>
<INPUT TYPE=HIDDEN NAME="action" VALUE="Add Listing">
<INPUT TYPE=hidden NAME="Title" value="<% =REQUEST.FORM("TITLE") %>">
<INPUT TYPE=hidden NAME="Email" value="<% =REQUEST.FORM("EMAIL") %>">
<INPUT TYPE=hidden NAME="URL" value="<% =REQUEST.FORM("URL") %>">
Category: <SELECT NAME="cat">
<OPTION VALUE="Advertising">Advertising
<OPTION VALUE="Arts">Arts
<OPTION VALUE="Books">Books & Magazines
<OPTION VALUE="Business">Business Services
<OPTION VALUE="Cars">Cars & Motorcycles
<OPTION VALUE="Children">Children
<OPTION VALUE="Collectibles">Collectibles
<OPTION VALUE="Computer">Computer & Peripherals
<OPTION VALUE="Dating">Dating
<OPTION VALUE="Education">Education
<OPTION VALUE="Electronics">Electronics
<OPTION VALUE="Employment">Employment
<OPTION VALUE="Entertainment">Entertainment
<OPTION VALUE="Fashion">Fashion
<OPTION VALUE="Finance">Financial
<OPTION VALUE="Flowers">Flowers
<OPTION VALUE="Food">Food & Beverage
<OPTION VALUE="Gifts">Gifts
<OPTION VALUE="Health">Health
<OPTION VALUE="Malls">Internet Malls
<OPTION VALUE="Internet">Internet Services
<OPTION VALUE="Legal">Legal
<OPTION VALUE="Misc" SELECTED>Miscellaneous
<OPTION VALUE="Money">Money Opportunities
<OPTION VALUE="Music">Music, Musical Instruments
<OPTION VALUE="Newsletters">Newsletters
<OPTION VALUE="Pets">Pets
<OPTION VALUE="Realestate">Real Estate
<OPTION VALUE="Software">Software
<OPTION VALUE="Sports">Sports
<OPTION VALUE="Travel">Travel
</SELECT><BR>
<input type=hidden NAME="Description" value="<% =REQUEST.FORM("description") %>">
Keywords separated by spaces (select up to 15; 150 characters)<BR>
<INPUT TYPE=TEXT SIZE=75 NAME="Keywords" MAXLENGTH=150 onChange="document.cc.linkwords.value=document.bb.Keywords.value; document.dd.key.value=document.cc.linkwords.value"><BR>
<INPUT TYPE=SUBMIT VALUE="Submit">
<A HREF="http://www.scrubtheweb.com">ScrubTheWeb</A>
</form>
</td></tr><tr><td align=center>
<form NAME="dd" action="http://www.moshix2.net/scripts/aliseadd.dll" method="POST" target=new15>
<input type="hidden" name="Dir" value="d:\inetpub\wwwroot\moshix2\ALISE\addtemp">
<input type="hidden" name="Alise" value="/add3.htm">
<input type="hidden" name="ok" value="/alise/ok.htm">
<input type="hidden" name="url" value="<% =REQUEST.FORM("URL") %>">
<input type="hidden" name="title" value="<% =REQUEST.FORM("TITLE") %>">
<input type="hidden" name="comment" value="<% =REQUEST.FORM("description") %>">
Keywords (separated by spaces):<BR>
<input type=text size=75 name="key"><br>
<input type=hidden name="name" value="<% =REQUEST.FORM("NAME") %>">
<input type=hidden name="email" value="<% =REQUEST.FORM("EMAIL") %>">
<input type="hidden" name="END" value="END">
<input type="submit" value="Submit">
<A HREF="http://www.moshix2.net">MOSHIx2</A>
</form>
</td></tr><tr><td align=center>
<FORM METHOD="POST" ACTION="http://www.aaa.com.au/dir2/sendsub.cgi" target=new16>
<input type=hidden name="to" value="aaa2@fl.net.au">
<input type=hidden name="subject" value="Matilda Listing">
<input type=hidden name="redirect" value="http://www.aaa.com.au/thankyou.shtml">
<INPUT Type=hidden NAME="realname" value="<% =REQUEST.FORM("name") %>">
<INPUT Type=hidden NAME="from" value="<% =REQUEST.FORM("email") %>">
<INPUT Type=hidden NAME="url" value="<% =REQUEST.FORM("title") %>">
<INPUT TYPE=hidden NAME="urlname" value="<% =REQUEST.FORM("url") %>">
<select name="selection">
<option selected>Select One Category</option>
<option value="Animals_and_Ecology"> Animals & Ecology
<option value="Animals_and_Ecology.Mammals"> -&gt; Mammals
<option value="Animals_and_Ecology.Reptiles"> -&gt; Reptiles
<option value="Animals_and_Ecology.Birds"> -&gt; Birds
<option value="Animals_and_Ecology.Environment"> -&gt; Environment
<option value="Arts_and_Humanities"> Arts & Humanities
<option value="Arts_and_Humanities.Architecture"> -&gt; Architecture
<option value="Arts_and_Humanities.Books"> -&gt; Books
<option value="Arts_and_Humanities.Good_Causes"> -&gt; Good Causes
<option value="Arts_and_Humanities.Literature"> -&gt; Literature
<option value="Arts_and_Humanities.Photography"> -&gt; Photography
<option value="Arts_and_Humanities.Poetry"> -&gt; Poetry
<option value="Audio"> Audio
<option value="Audio.Artists"> -&gt; Artists
<option value="Audio.Chat"> -&gt; Chat
<option value="Audio.MP3"> -&gt; MP3
<option value="Audio.Music"> -&gt; Music
<option value="Business_and_Economy"> Business & Economy
<option value="Business_and_Economy.Agriculture"> -&gt; Agriculture
<option value="Business_and_Economy.Companies"> -&gt; Companies
<option value="Business_and_Economy.Insurance"> -&gt; Insurance
<option value="Business_and_Economy.Employment"> -&gt; Employment
<option value="Business_and_Economy.Finance"> -&gt; Finance
<option value="Business_and_Economy.Real_Rstate"> -&gt; Real Estate
<option value="Computers_and_Internet"> Computers & Internet
<option value="Computers_and_Internet.Countries"> -&gt; Countries
<option value="Computers_and_Internet.Programming Languages"> -&gt; Programming Languages
<option value="Computers_and_Internet.Internet"> -&gt; Internet
<option value="Computers_and_Internet.Multimedia"> -&gt; Multimedia
<option value="Computers_and_Internet.Software"> -&gt; Software & Hardware
<option value="Computers_and_Internet.Homepages"> -&gt; Personal Homepages
<option value="Computers_and_Internet.WWW"> -&gt; WWW
<option value="Education"> Education
<option value="Education.College_Entrance"> -&gt; College Entrance
<option value="Education.K12"> -&gt; K12
<option value="Education.Kids"> -&gt; Kids
<option value="Education.Universities"> -&gt; Universities
<option value="Free_Stuff-Entertainment"> Free Stuff, Entertainment
<option value="Free_Stuff-Entertainment.Games"> -&gt; Games
<option value="Free_Stuff-Entertainment.Movies"> -&gt; Movies
<option value="Free_Stuff-Entertainment.Humor"> -&gt; Humor
<option value="Free_Stuff-Entertainment.Competitions"> -&gt; Competitions
<option value="Food_and_Cuisine"> Food & Cuisine
<option value="Food_and_Cuisine.Nutrition"> -&gt; Nutrition
<option value="Food_and_Cuisine.Recipes"> -&gt; Recipes
<option value="Food_and_Cuisine.Restaurants"> -&gt; Restaurants
<option value="Food_and_Cuisine.Types"> -&gt; Types
<option value="Food_and_Cuisine.Cultures"> -&gt; Cultures
<option value="Food_and_Cuisine.Drinks"> -&gt; Drinks
<option value="Government"> Government
<option value="Government.Law"> -&gt; Law
<option value="Government.Military"> -&gt; Military
<option value="Government.Politics"> -&gt; Politics
<option value="Government.Taxes"> -&gt; Taxes
<option value="Health"> Health
<option value="Health.Diseases"> -&gt; Diseases
<option value="Health.Drugs"> -&gt; Drug
<option value="Health.Fitness"> -&gt; Fitness
<option value="Health.Medicine"> -&gt; Medicine
<option value="History"> History
<option value="History.Archeology"> -&gt; Archeology
<option value="History.Genealogy"> -&gt; Genealogy
<option value="History.Exploration"> -&gt; Exploration
<option value="History.Computers"> -&gt; Computers
<option value="History.People"> -&gt; People
<option value="History.Museums"> -&gt; Museums
<option value="Lifestyle"> Lifestyle
<option value="Lifestyle.Auto"> -&gt; Auto
<option value="Lifestyle.Home"> -&gt; Home
<option value="Lifestyle.Gardening"> -&gt; Gardening
<option value="Lifestyle.Pets"> -&gt; Pets
<option value="Lifestyle.Kids"> -&gt; Kids
<option value="Lifestyle.Travel"> -&gt; Travel
<option value="News_and_Media"> News & Media
<option value="News_and_Media.Current_Events"> -&gt; Current Events
<option value="News_and_Media.Magazines"> -&gt; Magazines
<option value="News_and_Media.Newspapers"> -&gt; Newspapers
<option value="News_and_Media.TV"> -&gt; TV
<option value="News_and_Media.Radio"> -&gt; Radio
<option value="News_and_Media.Advertising"> -&gt; Advertising
<option value="Recreation_and_Sport"> Recreation & Sport
<option value="Recreation_and_Sport.Accommodation"> -&gt; Accomodation
<option value="Recreation_and_Sport.Antiques"> -&gt; Antiques
<option value="Recreation_and_Sport.Gambling"> -&gt; Gambling
<option value="Recreation_and_Sport.Hobbies"> -&gt; Hobbies
<option value="Recreation_and_Sport.Olympic"> -&gt; Olympic
<option value="Recreation_and_Sport.Sports"> -&gt; Sports
<option value="Reference-City_Seek"> Reference, City Seek
<option value="Reference-City_Seek.Dictionaries"> -&gt; Dictionaries
<option value="Reference-City_Seek.Libraries"> -&gt; Libraries
<option value="Reference-City_Seek.Maps"> -&gt; Maps
<option value="Reference-City_Seek.Classifieds"> -&gt; Classifieds
<option value="Reference-City_Seek.Phone_Numbers"> -&gt; Phone Numbers
<option value="Reference-City_Seek.Email"> -&gt; Email
<option value="Science"> Science
<option value="Science.Astronomy"> -&gt; Astronomy
<option value="Science.Biology"> -&gt; Biology
<option value="Science.CS"> -&gt; CS
<option value="Science.Engineering"> -&gt; Engineering
<option value="Science.Fiction"> -&gt; Fiction
<option value="Science.Solar"> -&gt; Solar
<option value="Social_Science"> Social Science
<option value="Social_Science.Anthropology"> -&gt; Anthropology
<option value="Social_Science.Languages"> -&gt; Languages
<option value="Social_Science.Communications"> -&gt; Communications
<option value="Social_Science.Psychology"> -&gt; Psychology
<option value="Social_Science.Economics"> -&gt; Economics
<option value="Social_Science.Sociology"> -&gt; Sociology
<option value="Society_and_Culture"> Society & Culture
<option value="Society_and_Culture.Environment"> -&gt; Environment
<option value="Society_and_Culture.Fashion"> -&gt; Fashion
<option value="Society_and_Culture.People"> -&gt; People
<option value="Society_and_Culture.Religion"> -&gt; Religion
<option value="Society_and_Culture.Shopping"> -&gt; Shopping
<option value="Society_and_Culture.Sex_and_Love"> -&gt; Sex & Love
</select><BR>
Description (10 Words):<BR><input type=text NAME="comments" size=20><BR>
<input type=submit value="Submit">
<A HREF="http://www.aaa.com.au">Matilda</A>
</form>
</td></tr><tr><td align=center>
<form method="POST" action="http://www.pointguide.com/cgi/new/free.cgi" target=new17>
<select name="category" size=1>
<option selected>Select One Category</option>
<option value="10" selected>Music/Entertainment
<option value="11">Business/Finance
<option value="12">Computers/Internet
<option value="13">Education
<option value="14">Government/Politics
<option value="15">Health/Medicine
<option value="16">Living &amp; Leisure
<option value="17">News &amp; Reference
<option value="18">Science/Technology
<option value="19">Sports
<option value="20">Travel
</select><br>
<input type=hidden name="url" value="<% =REQUEST.FORM("URL") %>">
<input type=hidden name="title" value="<% =REQUEST.FORM("TITLE") %>">
<input type=hidden name="description" value="<% =REQUEST.FORM("description") %>">
<input type=hidden name="name" value="<% =REQUEST.FORM("NAME") %>">
<input type=hidden name="email" value="<% =REQUEST.FORM("EMAIL") %>">
<input type=submit name="add" value="Submit">
<A HREF="http://www.pointguide.com">Pointguide</A>
</form>
</td></tr><tr><td align=center> <FORM ACTION="http://www.jayde.com/cgi-bin/addurl.cgi" METHOD=POST target=new18>
<input type=hidden value=verify name=action>
<INPUT TYPE=hidden NAME="name" value="<% =REQUEST.FORM("NAME") %>">
<INPUT TYPE=hidden NAME="email" value="<% =REQUEST.FORM("EMAIL") %>">
<INPUT TYPE=hidden NAME="sname" value="<% =REQUEST.FORM("TITLE") %>">
<INPUT TYPE=hidden NAME="URL" VALUE="<% =REQUEST.FORM("URL") %>">
<input type=hidden NAME="desc" value="<% =REQUEST.FORM("description") %>">
Category:
<SELECT NAME=cat><OPTION> Personal
<OPTION> Law<OPTION> Social Sciences<OPTION> Art Links<OPTION> Bus General<OPTION> Internet<OPTION> Food Links<OPTION> Free Stuff<OPTION> Sports<OPTION> Software<OPTION> Bus Industry<OPTION> Reference<OPTION> Bus MLM<OPTION> Science and Tech<OPTION> HTML Support<OPTION> JavaScript<OPTION> Education<OPTION> Directories<OPTION> News Links<OPTION> Literature<OPTION> Computers<OPTION> Game Sites<OPTION> Marketing<OPTION> Music Links<OPTION> Job Sites<OPTION> Government<OPTION> Stores and Malls<OPTION> Travel<OPTION> EZines<OPTION> Bus Financial<OPTION> Gardening<OPTION> Canadian Links<OPTION> Bus Real Estate<OPTION> Miscellaneous<OPTION> Health<OPTION> Web Design<OPTION> International<OPTION> Religion<OPTION> Entertainment<OPTION> Non Profit
</SELECT><BR>
<input type=hidden name=list value=on>
<INPUT TYPE=submit VALUE="Submit">
<A HREF="http://www.jayde.com">Jayde</A>
</FORM>
</td></tr><tr><td align=center>
<form method=GET action="http://www.google.com/addurl" target=new19>
<input type=hidden name=q value="<% =REQUEST.FORM("url") %>">
<input type=hidden name=dq value="<% =REQUEST.FORM("description") %>">
<input type=submit value="Add URL">
<A HREF="http://www.google.com">Gooble</A>
</form>
</td></tr></table>
```


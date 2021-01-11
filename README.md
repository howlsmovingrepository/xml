# xml-mp3
Projects for Frank &lt;3

XML project for Frank Akaiwa Fall 2020, grade: 100%

3 parts: XML data file, XML file w/ internal DTD, external DTD - schema and edits on next project.



Rubric: 

For this project we are going to use information about music as a data source to build XML documents.  We will start with the Grammy Awards.  Since the project starts just after the awards, we will use the eight (8) nominees and winner for album of the year in the general category.  Please don’t confuse the album of the year with the record of the year, which is an individual song.  You will also add another five (5) of your favorite albums to this list.  You will end up with a total of thirteen (13) albums with no duplicates.  You may include albums from the same artist, but you must have a total of thirteen (13) albums.  Next you are going to place this information into an XML file and then create a DTD to validate that information. (Note:  You can find information on the Grammy Album of the Year nominees at http://www.grammy.com.)    
 
Part 1 – XML File
Artist, Album and Song (Track List) Information - Your XML file should be organized first by artist then by album and then by songs.  The information in your XML file will include information on each artist or group as well as the songs or tracks on the album. For the Grammy Album of the Year nominees you should include the following information from the Grammy site: the individual artists, the producers, engineers/mixers, songwriters, mastering engineer and record label. For the additional five (5) favorite albums you will not have to add the producers, engineers/mixers, and mastering engineer since this information can be difficult to find outside of the Grammy site. 

Each of your thirteen (13) albums will include information about the songs on the album and then a separate portion containing release information for that album.  Your XML document should contain the following information about the artists, albums, and their music; (please note, you do not need to use these names for your elements): artist, indication if the artist is a group or person, group member names (if appropriate), artist or group country, When the artist or group’s career began and ended (if appropriate), chosen album title, album category (choices are; “Grammy_Winner”, “Grammy_Nominee” or “Personal_Favorite”), all song titles for that album, song position (for each song in album), all song lengths and all song composers and writers (if available).  A great source for this information is at http://www.allmusic.com/.)

Album Release Information - Many albums have more than one release.  For the purpose of this project you are going to collect information on all releases of the albums mentioned above.  You must provide the album release date, record label, record label catalog number, bar code number (if available), country, and format information for every release of the thirteen (13) albums.  
 An excellent source to find much of the release information you will need is at http://musicbrainz.org/.  You may notice that some of the releases of the same album have slightly different song orders or bonus tracks.  In this case, use the track information provided on www.allmusic.com.  You should only provide the track list once.  Do not provide a track list for every release of an album.  
Album Cover Image - You will also add an album image to help you recognize the albums in your collection.  You must include a picture of each of the albums in your xml file.  We can’t place an image into an XML file, but we can reference the file name.  Download images for each of your albums.  Your images should be stored in a jpeg, jpg, or png file format. Add the image file names to your XML document as well as a citation of where you obtained each picture.  You can find these images on various music sites.  I have inserted an example of a link to an album image for Willy Porter’s Falling Forward album that I obtained from Amazon.
(http://images.amazon.com/images/P/B00000JZ2R.01.LZZZZZZZ.jpg ).  I suggest that you rename the file names into something more understandable.  If you are unable to find an image for a particular album, substitute an alternative image. (Note:  You must download the image file to your computer.  A link to an image online will not be accepted.)
You can set up your XML document any way you want; however, please include at least one attribute. This project will be much easier if you first outline your thoughts by constructing an XML hierarchy for the problem (as we did in in-class) and then create the XML document from this hierarchy (however, this is not required). Just make sure that your resulting XML document contains all of the above information and is well-formed. 
 
Please save your completed XML document as username_project1-1.xml.  
 
Part 2 – Internal DTD
Now that you have gotten your information organized create a DTD for the XML file that you created for part 1. This will be used to help ensure that the structure of the XML document remains valid. Create an internal DTD that will validate the XML document from part 1. Add the appropriate Document Type Declaration to your original part 1 file and name this new file username_project1-2.xml. Make sure your XML document is both well-formed and valid.
 
(Note: If you feel that you need to modify your Part 1 XML document to complete this project feel free to do so; however, include a few comments in your XML file explaining what you did and why you felt that it was necessary.)  You can use this format to include comments “<!--  Your comments go here -->”.

 
  
Part 3 – External DTD
After you complete Part 2, I want you to convert the internal DTD to an external DTD. Make the following changes to your original XML document and then create an external DTD that validates the new XML document.
 
Changes to the XML file:
 
1.	Create a required “sku” attribute for each Album and song. 
 
•	The Album SKUs will begin with K315F2020A, and then K315F2020B until each Album has been assigned a stock keeping unit. All Letters in the SKU must be capitalized.

•	The song SKUs will begin with K315F2020A001, and then K315F2020A002 until each song for the first Album has been assigned a SKU. The songs from the second Album will begin with K315F2020B001, and then K315F2020B002 until each song from each Album has a SKU. All Letters in the SKU must be capitalized.

•	(Note: I recommend sorting your songs in song order on the album before assigning sku’s.) 

2.	Create an “albumref” attribute to indicate which song is associated with which Album.

3.	Create a required “type” attribute for each Album and song. 

•	The attribute values will be either “album” or “song”. 
 
4.	Create the appropriate entries in the DTD for these changes. 

 
Name this file username_project1-3.dtd. Add the appropriate Data Type Declaration to your XML file. Save the XML file as username_project1-3.xml. Make sure your XML document is both well-formed and valid.
 
Place the username_project1-1.xml, username_project1-2.xml, username_project1-3.xml, username_project1-3.dtd and album image files in a compressed zip file named yourusername_project1.zip. Submit this file to the Project 1 assignment on the Canvas site any time prior to the due date.
 



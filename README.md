
   #                                                                                     CAPSTONE PROJECT
   ## Project Description
         
 This project is aimed to solve an imaginary problem or a hypothetical situation with the application of Foursquare API and other machine learning techniques. Foursquare API gives the location data and could be used to get details of different venues like ratings, location coordinates etc. Hence it can be used to cluster locations according to their venue categories, finding best suited locations for various business enterprices, housing and many more. In this project I take the opportunity to find a good location to start a small enterprise, a Bookstore.\n\nBooks have always had a very crucial part of development of mankind. They are even considered the best companions of ones life as they provide unconditional knowledge. Hence a bookstore or a library that provides such resources are also equally important for a town to bring up civilized and educated youth. As Neil Gaiman said _A town is not a town without a bookstore._
       
   ### Introduction/ Question to Solve
  In this project I have tried to find locations to open a bookstore in Warwickshire, a county in United Kingdom.\n\nIn order to do this, following information is required.
  * Towns in Warwickshire county
  *Location coordinates of these towns 
  * Accessibility of bookstores or libraries within a commutable distance
  * For towns without any bookstores or libraries, does the town have a big enough population to start a venture. 
  * Also the presence of schools or colleges in the vicinity so that the store could be useful for students and teachers.
      
      
   #### Target Audience
  *Entrepreneurs / High street bookstore chains who wish to open a bookstore in Warwickshire.
  
   #### Dataset needed for this project 
   * List of towns in Warwickshire 
   * The location coordinates of these towns 
   * Details regarding bookstores, discount stores and libraries 
   * Population data
   * School/College location data
        
   ### Data Extraction
   * Data is scrapped using 'beautiful soup' from the following sites:
   * _List of towns : https://worldpostalcode.com/united-kingdom/england/warwickshire
   * _Population data: https://www.ebayinuk.co.uk/warwickshire-towns-villages-population
   * Location coordinates of the towns were obtained using _OpenCage API.
   * Foursquare API was used to collect details of bookstores, libraries and schools in these towns
        
   ### Steps 
   
* Using location coordinates of towns in Warwickshire to extract the details of existing bookstores, discount stores and libraries using Foursquare API.
* Creating a segregated data-frame of towns without any bookstores or libraries in a radius of 5km from the location co-ordinates.
* Extraction of population data for the towns in segregated data frame 
* Search for location of schools or colleges using the Foursquare API. The towns with more population and schools nearby can be opted as the best option for opening a store.
* Towns with bookstores and libraries but are thickly populated are clustered using the K-means clustering to find towns that only have libraries which would be another smart option to open a discount store (Stores that sell second hand books) or a bookstore.


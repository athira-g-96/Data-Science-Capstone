{
    "cells": [
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "![](https://img.thedailybeast.com/image/upload/c_crop,d_placeholder_euli9k,h_675,w_1200,x_0,y_0/dpr_2.0/c_limit,w_740/fl_lossy,q_auto/v1493058170/articles/2011/10/12/america-s-greatest-independent-bookstores-and-why-they-should-survive/independent-bookstores-fountain-books_ocfbpl)"
        },
        {
            "cell_type": "markdown",
            "metadata": {
                "collapsed": true
            },
            "source": " #                                                                                     CAPSTONE PROJECT"
        },
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "## Project Description"
        },
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "This project is aimed to solve an imaginary problem or a hypothetical situation with the application of Foursquare API and other machine learning techniques. Foursquare API gives the location data and could be used to get details of different venues like ratings, location coordinates etc. Hence it can be used to cluster locations according to their venue categories, finding best suited locations for various business enterprices, housing and many more. In this project I take the opportunity to find a good location to start a small enterprise, a Bookstore.\n\nBooks have always had a very crucial part of development of mankind. They are even considered the best companions of ones life as they provide unconditional knowledge. Hence a bookstore or a library that provides such resources are also equally important for a town to bring up civilized and educated youth. As Neil Gaiman said \" A town is not a town without a bookstore\"."
        },
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "### Introduction/ Question to Solve"
        },
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "In this project I have tried to find locations to open a bookstore in Warwickshire, a county in United Kingdom.\n\nIn order to do this, following information is required.\n \n1) Towns in Warwickshire county\n\n2) Location coordinates of these towns \n\n3) Accessibility of bookstores or libraries within a commutable distance\n\n4) For towns without any bookstores or libraries, does the town have a big enough population to start a venture. Also the presence of schools or colleges in the vicinity so that the store could be useful for students and teachers.\n\n\n#### Target Audience\n Entrepreneurs / High street bookstore chains who wish to open a bookstore in Warwickshire."
        },
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "## Data"
        },
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "#### Dataset needed for this project\n\n1) List of towns in Warwickshire\n\n2) The location coordinates of these towns \n\n3) Details regarding bookstores, discount stores and libraries \n\n4) Population data\n\n5) School/College location data"
        },
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "### Data Extraction\n\nData is scrapped using 'beautiful soup' from the following sites:\n\n_List of towns : https://worldpostalcode.com/united-kingdom/england/warwickshire\n    \n_Population data:   https://www.ebayinuk.co.uk/warwickshire-towns-villages-population/\n \n\nLocation coordinates of the towns were obtained using _OpenCage API.\n\nFoursquare API was used to collect details of bookstores, libraries and schools in these towns\n"
        },
        {
            "cell_type": "markdown",
            "metadata": {},
            "source": "### Steps \n\nUsing location coordinates of towns in Warwickshire to extract the details of existing bookstores, discount stores and libraries using Foursquare API.\n\nCreating a segregated data-frame of towns without any bookstores or libraries in a radius of 5km from the location co-ordinates.\n\nExtraction of population data for the towns in segregated data frame \n\nSearch for location of schools or colleges using the Foursquare API. The towns with more population and schools nearby can be opted as the best option for opening a store.\n\nTowns with bookstores and libraries but are thickly populated are clustered using the K-means clustering to find towns that only have libraries which would be another smart option to open a discount store (Stores that sell second hand books) or a bookstore.\n"
        },
        {
            "cell_type": "code",
            "execution_count": null,
            "metadata": {},
            "outputs": [],
            "source": ""
        }
    ],
    "metadata": {
        "kernelspec": {
            "display_name": "Python 3.6",
            "language": "python",
            "name": "python3"
        },
        "language_info": {
            "codemirror_mode": {
                "name": "ipython",
                "version": 3
            },
            "file_extension": ".py",
            "mimetype": "text/x-python",
            "name": "python",
            "nbconvert_exporter": "python",
            "pygments_lexer": "ipython3",
            "version": "3.6.9"
        }
    },
    "nbformat": 4,
    "nbformat_minor": 1
}

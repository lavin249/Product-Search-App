# Product-Search-App

Page is tested on: 
	Microsoft Edge: Version 114.0.1823.79 (Official build) (64-bit).
	Google Chrome: Version 114.0.5735.199 (Official Build) (64-bit).
	Brave: Version 1.52.130 Chromium: 114.0.5735.198 (Official Build) (64-bit).

Steps to Run:
	Double Click on the index.html 
	
Tests Passed:
	Enter just one space. Page should throw alert stating 'Please Enter Only AlphaNumeric Characters'.
	Enter many spaces. Page should throw alert stating 'Please Enter Only AlphaNumeric Characters'.
	Enter space 23. Page should trim the space and display four results in resultSet that have "23" in it.
	Enter 23 space. Page should trim the space and display four results in resultSet that have "23" in it.
	Enter lavin in input. Page should display 'No Result Found'.
	Enter lavin in input. Page should display 'No Result Found'.
	Enter null in input. Page should display 'No Result Found'.
	Made sure that the ordering is based on ProductName ascending to descending.
	
Implementation:
	On Click of search button.
	Reset any previous result view.
	Reset all the variables.
	Get the data from search box
	Access the stored JSON object in the javascript. 
	Check if it's alphanumeric string.
	Get result set to be displayed by comparing the searcch string with each value in JSON object
	Sort it on basis of ProductName in ascending order.
	Display Result.
	
Improvements:
	Use persistence layer (relational database).
	Expose rest-api to get product information.
	Secure rest-api.
	Implement ajax call to fetch thee data from rest-api.
	Deploy on beanstalk.
	
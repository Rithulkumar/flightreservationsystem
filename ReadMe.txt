Plumbago Airlines : Online Seat Reservation System
=======================================================

Requirements:
Anypoint Studio 7.1.2
Mule 4
Mule runtime 4.1.3
RAML 1.0

Paste the flightrecords folder in d drive. 
Import the api into anypoint studio
Deploy and open the console to understand the api webservice given

Webservices :

1. plumbango-airlines.xml - main page containing api kit router
2. search-flights.xml - query parameters : from, to
	gives the list of flights that travels in both directions
3. seat-availability.xml - using flight id, we can get seat information on all classes
		FIRST, BUSINESS, ECONOMY (while confirming seat, pass class info as given)
		the payment is in progress in this state.
		modifies the seat availability in seat records simultaneously
4. payment-confirmation.xml - confirms the payment
5. global-config.xml - contains the global configurations and error handling flow for all

Files:
 1. flightrecords.csv contains the sample flight records
 2. confirmedseatrecords.csv will get updated with each confirmation
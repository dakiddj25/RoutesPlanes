# RoutesPlanes
Backend/API
Routes

Airports
GET /airports: Get all airports in NYC.
GET /Airports/:id: Get single airports. (Ex. LGA)
GET /researches/:id/Terminal: Get all Terminal for a specific airports. (Ex. LGA : Terminals:A, B, C)
POST /Airports: Add new airports. (Ex. Jones airport)
DELETE /Airports/:id: Delete single airports.

Airline
GET /Airline: Get all Airline.  (Ex. Jet Blue, American Airline)
GET /Airline/:id: Get single airline. (Ex. JetBlue)
POST /Airline: Add new airline.
DELETE /Airline/:id: Delete single airline.

Terminal
GET /Terminal: Get all Terminal. (Ex. LGA: Terminal A : JetBlue, Spirit, American)
POST /Terminal: Add new terminal.
DELETE /Terminal/:id: Delete single terminal.
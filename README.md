# RoutesPlanes
## Backend/API 

## Database Schema

### Tables and Columns

- **AIRPORT**
  - `id`: Integer, primary key.
  - `name`: String.
  - `location`: String.

- **AIRLINE**
  - `id`: Integer, primary key.
  - `name`: String.

- **TERMINAL**
  - `id`: Integer, primary key.
  - `airport_id`: Integer, foreign key referencing `id` column in Researchers table. Add "ON DELETE SET NULL".
  - `airline_id`: Integer, foreign key referencing `id` column in Species table. Add "ON DELETE CASCADE".


### Seed Data
- **AIRPORT**
  - JFK, Brooklny NY.
  - LGA, Queens NYC.
  - EWR, New Jersy NJ.
 
- **AIRLINE**
  - JetBlue
  - American Airline
  - Spirit
  - United
  - Southwest


- **Terminal**
  - LGA : A has JetBlue & American
  - LGA : B has Spirit
  - LGA : C has United
  - LGA : D has South West
  - JFK : 1 
  - JFK : 2
  - JFK : 3
  - JFK : 4
  - JFK : 5
  - EWR : 1
  - EWR : 2
  - EWR : 3
  - EWR : 4
  - EWR : 5



### Routes

**Airports**
- GET `/airports:` Get all airports in NYC.
- GET `/Airports/:id:` Get single airports. (Ex. LGA)
- GET `/researches/:id/Terminal:` Get all Terminal for a specific airports. (Ex. LGA : Terminals:A, B, C)
- POST `/Airports:` Add new airports. (Ex. Jones airport)
- DELETE `/Airports/:id:` Delete single airports.

**Airline**
- GET `/Airline:` Get all Airline.  (Ex. Jet Blue, American Airline)
- GET `/Airline/:id:` Get single airline. (Ex. JetBlue)
- POST `/Airline:` Add new airline.
- DELETE `/Airline/:id:` Delete single airline.

**Terminal**
- GET `/Terminal:` Get all Terminal. (Ex. LGA: Terminal A : JetBlue, Spirit, American)
- POST `/Terminal:` Add new terminal.
- DELETE `/Terminal/:id:` Delete single terminal.
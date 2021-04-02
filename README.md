# Texas HEB Covid-19 Vaccine Appointments
Automatically ping for Covid-19 vaccine appointments in Texas

## Usage

First you will have to clone the repository

``` bash
git clone https://github.com/joaquinrz/vaccine_appointments

cd vaccine_appointments
```

## Using Docker

### Build Docker Image
```bash
docker build -t hebvaccine ./
```

### Run your image
Examples:

 - `docker run hebvaccine -c "Austin" -c "San Antonio"` would search based on cities
 - `docker run hebvaccine -H "Round Rock, TX" -d 50` would look for appointments 50 miles from Round Rock
 - `docker run hebvaccine -H 78023 -d 30` would look for appointments 30 miles from zip code 78023

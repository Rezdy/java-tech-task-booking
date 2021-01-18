# Rezdy technical test in Java

## Background

- An imaginary company is operating a group tour of Sydney Opera House.
- The tour runs hourly from 9am to 5pm on each day.
- Right now, the company is taking the booking manually, which is not productive and error prone.
- You are going to create a software solution to address their issue.

## Requirements

- You need to implement an interface that has one method
  ```
  String book(String date, String startTime, int numberOfPeople);
  ```
- The customers can book a tour by giving a date, a start time (on the hour), and the number of people.
- A maximum of 10 people can be taken for each tour. First come, first served.
    E.g. a group of 3 booked a 09:00 tour, then another group of 8 will not be able to make the booking at 09:00.
- If the booking is successful, it will return a booking reference number.
- If the booking is not successful because there are no availability,
    or the selected startTime is out of the business hour,
    or the selected date is not a future date,
    a proper hint needs to be given.

## Assumptions

- The format of the input date is `yyyy-MM-dd`, e.g. `2021-01-15`, and the format of the input startTime is `HH:mm`, e.g. `09:00`.
- The input startTime is on the hour and in 24 hour format, e.g. `09:00`, `10:00`, `14:00`.
- No external data storage is required, and the booking information can be stored in memory.
- A concurrent booking scenario might occur if two customers try to book the same session at the same time.
  This concurrent booking scenario can be ignored for the purpose of the test, but you are welcomed to put some thought on it.

## Things we are interested in

- A buildable maven project (you can [fork the repository](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo)
  into your GitHub account and make the change)
- Readable code and clean structure
- Well tested solution

## Questions we may ask in the future

- To make the software solution more useful, what other methods or interfaces you can add?


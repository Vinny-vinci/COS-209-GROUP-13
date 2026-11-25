PRODUCT REQUIREMENTS DOCUMENT (PRD)

Project Title: Barbershop Booking and Workforce Optimisation System

Date: November 2026

---

1. Product Overview

The Barbershop Booking and Workforce Optimisation System is a web-based application designed to improve the way barbershops handle customer appointments and organise their workers.

The application will allow customers to view available services, check appointment slots, choose a preferred barber or allow the system to assign one automatically. Customers will also be able to manage their bookings without having to visit the shop or contact a barber directly.

For the barbershop, the system will provide a better way to organise individual work schedules and distribute appointments among available barbers.

The main purpose of the application is to reduce waiting times, prevent scheduling conflicts, make better use of available working hours and improve the overall operation of the barbershop.

2. Problem Statement

Several problems can affect the daily operations of a barbershop, particularly when appointments are not properly organised.

The problems identified by the team include:

2.1 Unequal Distribution of Workload

Some barbers may have several customers waiting while others have little or no work during the same period. This creates an imbalance in workload and affects productivity.

2.2 Loss of Customers

Customers who regularly experience poor organisation or long waiting times may decide to visit other barbershops.

2.3 Long Waiting Times

Without a proper booking arrangement, customers may arrive at the same time and have to wait for an available barber.

2.4 Poor Use of Working Hours

Some barbers may have fully occupied schedules while others have unused time slots. This affects how effectively the available workforce is used.

2.5 Reduced Revenue

Poor scheduling, unused working hours and the loss of customers can affect the amount of business the barbershop generates.

3. Existing Solution and Its Limitations

One approach to dealing with long waiting times and workload problems is to employ more barbers.

However, increasing the number of workers does not necessarily solve the problem of poor appointment scheduling. It may also increase operating expenses without ensuring that work is shared properly.

Another common approach is to take bookings through phone calls, WhatsApp messages or physical notebooks.

Although these methods can be useful, they make it difficult to keep track of all appointments, monitor individual barber availability and prevent scheduling conflicts.

A more organised booking system is therefore needed to make better use of the existing workforce.

4. Proposed Solution

The team proposes the development of a barbershop booking application that allows customers to schedule appointments based on the availability of services and barbers.

Customers will have two options when booking:

- Select a particular barber.
- Allow the system to assign any suitable available barber.

When automatic assignment is selected, the system will consider the barber's availability and existing workload before assigning the appointment.

The application will also provide individual schedules for barbers and allow customers to cancel or reschedule their appointments.

This will help the barbershop manage its appointments more effectively without depending on an increase in the number of workers.

5. Project Objectives

The objectives of the project are to:

1. Reduce the time customers spend waiting for services.
2. Improve the distribution of appointments among available barbers.
3. Prevent double bookings and scheduling conflicts.
4. Make better use of the barbers' available working hours.
5. Reduce customer loss caused by poor appointment management.
6. Make it easier for customers to book and manage appointments.
7. Improve the overall efficiency of barbershop operations.
8. Support an increase in customer satisfaction and business revenue.

6. Target Users

The application will have three main categories of users.

6.1 Customers

Customers will use the application to:

- Create an account and log in.
- View available services and their prices.
- Check available appointment dates and time slots.
- Select a preferred barber.
- Choose automatic barber assignment.
- Book appointments.
- View upcoming and previous appointments.
- Cancel or reschedule existing appointments.

6.2 Barbers

Barbers will use the application to:

- View their assigned appointments.
- Check their daily and weekly schedules.
- Manage their working availability.
- Mark specific days or periods as unavailable.
- View their assigned workload.

6.3 Administrator (Shop Owner)

The administrator will be responsible for managing the general operations of the application.

The administrator should be able to:

- Add, edit or remove barber accounts.
- Add and update available services.
- Set service prices and estimated durations.
- View appointments made through the application.
- View individual barber schedules.
- Monitor appointment distribution among barbers.

7. Functional Requirements

The application should provide the following features.

7.1 User Registration and Login

- Customers should be able to create accounts using their basic details.
- Registered users should be able to log in.
- The system should distinguish between customers, barbers and administrators.
- Users should only have access to features permitted for their roles.

7.2 Service Management

- The administrator should be able to add and update available services.
- Each service should have a name, price and estimated duration.
- Customers should be able to view the available services before making a booking.

7.3 Appointment Booking

- Customers should be able to select a service, date and available time slot.
- The system should display time slots based on barber availability and the estimated duration of the selected service.
- The system should prevent two appointments from being assigned to the same barber at overlapping times.
- Successful bookings should be recorded in the system.

7.4 Barber Selection and Automatic Assignment

Customers should have the option of selecting a specific barber or allowing the system to assign one.

When automatic assignment is selected, the system should:

1. Check which barbers are working during the requested period.
2. Identify barbers who can provide the selected service.
3. Check that they are available for the full duration of the appointment.
4. Compare the total booked working time of the available barbers for that day.
5. Assign the appointment to the suitable barber with the lowest total booked working time.
6. Where two or more barbers have the same workload, use the time since their last appointment to determine the assignment.

If no suitable barber is available, the customer should be informed that the selected time slot is unavailable.

7.5 Barber Schedule Management

- Each barber should have an individual work schedule.
- Schedules should include working days, starting and closing times, and breaks.
- Barbers should be able to mark themselves unavailable when necessary.
- The system should use these schedules when displaying available appointment slots.

7.6 Appointment Management

- Customers should be able to view their bookings.
- Customers should be able to cancel an appointment.
- Customers should be able to reschedule an appointment to another available time slot.
- The system should update the relevant barber's schedule after a cancellation or rescheduling.
- Cancelled appointments should no longer occupy the barber's available time.

8. Non-Functional Requirements

The following requirements describe how the application should operate.

8.1 Usability

The application should have a simple interface that customers and barbers can understand without difficulty.

8.2 Performance

The application should load available appointment slots and process booking requests within a reasonable time.

8.3 Security

User account information should be protected. Passwords should be securely hashed, and access to administrative features should be restricted to authorised users.

8.4 Reliability

The system should maintain accurate appointment records and prevent conflicting bookings.

8.5 Availability

Customers should be able to access the application to check and make bookings at any time, subject to system maintenance.

8.6 Consistency

Changes made to appointments should be reflected in the relevant customer and barber schedules.

9. Database Requirements

The application will require a database to store user information, barber schedules, services and appointment records.

The main data entities are expected to include:

Entity| Information stored
Users| User ID, name, phone number, password hash and role
Barbers| Barber ID, user ID, skills and availability status
Services| Service ID, name, price and duration
Barber Schedules| Schedule ID, barber ID, working days, start time and end time
Appointments| Appointment ID, customer ID, barber ID, service ID, date, start time, end time and status

The final database structure may be adjusted during development.

10. Project Scope

The first version of the application will focus on the main booking and scheduling functions.

10.1 Features Included in Version 1.0

- User registration and login.
- Customer, barber and administrator accounts.
- Service management.
- Viewing available services and time slots.
- Appointment booking.
- Preferred barber selection.
- Automatic barber assignment.
- Individual barber schedules.
- Appointment cancellation and rescheduling.
- Workload distribution.

10.2 Features Outside the Initial Scope

The following features may be considered for future versions:

- Online payment integration.
- Loyalty and reward programmes.
- Product and inventory management.
- Support for multiple barbershop branches.
- Advanced business analytics and reporting.
- SMS and WhatsApp appointment notifications.
- Customer ratings and reviews.

11. Acceptance Criteria

The application will be considered to meet its main requirements when:

1. Customers can successfully create accounts and log in.
2. Customers can view available services and appointment slots.
3. Customers can select their preferred barber.
4. Customers can choose automatic barber assignment.
5. Automatic assignment considers both availability and existing workload.
6. The system prevents overlapping appointments for the same barber.
7. Customers can cancel and reschedule appointments.
8. Changes to appointments are reflected in the relevant barber's schedule.
9. Barbers can view and manage their individual schedules.
10. Administrators can manage barbers, services and appointments.

12. Conclusion

The Barbershop Booking and Workforce Optimisation System is intended to address the problems associated with poorly organised appointments and unequal workload distribution in barbershops.

Rather than relying on employing more workers, the application will focus on making better use of the available barbers through organised scheduling and automatic appointment assignment.

By providing customers with a convenient way to book and manage appointments, the system aims to improve service delivery, reduce waiting times and help barbershops operate more efficiently.

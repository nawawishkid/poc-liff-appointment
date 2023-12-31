# PoC: Line LIFF for appointment

## Functional Requirements

1. Line users can book an appointment via the LIFF page
2. Appointment scheduling powered by ~~Cal.com (the open-source version)~~ Google Calendar (normal events, not the appointment scheduling since there's still no API support yet)

## User Journey

### Admin users

#### Initial setup

1. An admin user logs into the application's administration panel using their Google account
2. The application asks for permissions to access the admin user's Google Calendar information via OAuth 2.0 consent screen
3. The admin user allows the application to access their Google Calendar information
4. The application displays the integrated Google Calendar to let the user know which calendar they have given access to whenever they visit the administration panel

### End Users

1. A user visits the LIFF link
2. The user log into the LIFF app using their LINE account
3. The appointment scheduling page shows up as a calendar
4. The user books their preferred schedule and fills in the booking form
5. The user gets nofitification message via Line `n` minutes prior the booked time

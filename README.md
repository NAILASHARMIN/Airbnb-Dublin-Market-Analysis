# Airbnb-Dublin-Market-Analysis

This was a project where I worked on an Airbnb dataset. But unlike the typical property rating and review score prediction projects, in this one, I focused more on figuring out the host and guest relationship dynamics for a specific destination Dublin, Ireland. I tried to put up a storyboard in Tableau with the findings that would highlight key aspects from a managerial perspective to design a marketing campaign that may result in increased booking

- What guests are searching for in Dublin;
- Which inquiries hosts tend to accept;
- When is the most high-demand time for Dublin Airbnb; 
- The interaction dynamics between guests & hosts.

The goal of this challenge is to analyze, understand, visualize, and communicate the demand / supply in the market. For example you may want to look at the breakdown of start date day of the week, or number of nights, or room type that is searched for, and how many hosts accepted the reservation. In particular, we are interested in:

- what the gaps are between guest demand and host supply that the new city manager could plug to increase the number of bookings in Dublin,
- what other data would be useful to have to deepen the analysis and understanding.

There are 2 datasets: 

1. contacts dataset contains the following columns:

id_guest - Alphanumeric user_id of the guest making the inquiry
id_host - Alphanumeric user_id of the host of the listing to which the inquiry is made
id_listing - Alphanumeric identifier for the listing to which the inquiry is made
ts_contact_at - UTC timestamp of the moment the inquiry is made.
ts_reply_at - UTC timestamp of the moment the host replies to the inquiry, if so
ts_accepted_at - UTC timestamp of the moment the host accepts the inquiry, if so
ts_booking_at - UTC timestamp of the moment the booking is made, if so
ds_checkin - Date stamp of the check-in date of the inquiry
ds_checkout - Date stamp of the check-out date of the inquiry
n_guests - The number of guests the inquiry is for
n_messages - The total number of messages that were sent around this inquiry

2. searches dataset contains the following columns:

ds - Date of the search
id_user - Alphanumeric user_id
ds_checkin - Date stamp of the check-in date of the search
ds_checkout - Date stamp of the check-out date of the search
n_searches - Number of searches in the search set
n_nights - The number of nights the search was for
n_guests_min - The minimum number of guests selected in a search set
n_guests_max - The maximum number of guests selected in a search set
guest_country - The country the search was from
filter_price_min - The value of the lower bound of the price filter, if the user used it
filter_price_max - The value of the upper bound of the price filter, if the user used it
filter_room_types - The room types that the user filtered by, if the user used the room_types filter
filter_neighborhoods - The neighborhoods types that the user filtered by, if the user used the neighborhoods filter


My Approach was:
1. Clean and preprocess the 2 datasets
2. Use two specialized pandas package mitosheet & profiling for further exploratory analysis
3. Then use the procesed datasets for final visualization in Tableau

Find The Tableau Visual here: 
https://public.tableau.com/views/AirbnbDublinMarketAnalysis/Story1?:language=en-US&:display_count=n&:origin=viz_share_link

# Json-City-Similarities

Company XYZ is an Online Travel Agent, such as Expedia, Booking.com, etc.
They store their data in JSON files. Each row in the json shows all different cities which have
been searched for by a user within the same session (as well as some other info about the user).
That is, if I go to company XYZ site and look for hotels in NY and SF within the same session,
the corresponding JSON row will show my user id, some basic info about me and the two cities.
You are given the following tasks:

    1. There was a bug in the code and one country didn't get logged. It just shows up as an
       empty field (""). Can you guess which country was that? How?
    2. For each city, find the most likely city to be also searched for within the same session.
    3. Travel sites are browsed by two kinds of users. Users who are actually planning a trip and
       users who just dream about a vacation. The first ones have obviously a much higher
       purchasing intent. Users planning a trip often search for cities close to each other, while
       users who search for cities far away from each other are often just dreaming about a
       vacation. That is, a user searching for LA, SF and Las Vegas in the same session is much
       more likely to book a hotel than a user searching for NY, Paris, Kuala Lumpur (makes
       sense, right?). Based on this idea, come up with an algorithm that clusters sessions into
       two groups: high intent and low intent. Explain all assumptions you make along the way.


text source: A Collection of Take Home Data Science Challenges by Data Science Bootcamps

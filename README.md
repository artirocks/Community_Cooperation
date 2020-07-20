# Community collaboration in the context of COVID-19


### What's the problem?

In a very short period of time, COVID-19 has revealed the limits of the systems we take for granted. 
There is a growing interest in enabling communities to cooperate among themselves to solve problems, whether it be to advertise where supplies are held, offer assistance for collections, or other local services like volunteer deliveries.

In the COVID-19 crisis, we have already seen shortages of local food, medical equipment, and other supplies. In addition, the recommended (or required) self-isolation and social distancing measures can compound the problem by preventing people from easily getting to locations with the best stocks of supplies.

What is needed is a solution that empowers communities to easily connect and provide this information to each other.


## The idea

The goal is to provide a mobile application, along with server-side components, that serves as the basis for developers to build out a community cooperation application that addresses local needs for food, equipment, and resources.
It would allow both "Suppliers" (such as a store or a community member who has produce they can sell or distribute) to make people aware of what the have; and consumers ("Recipients") to locate where these supplies are, and, if necessary, guide them to the appropriate locations to pick them up.

Our solution addresses the problem of subdivision of Red, Green and Orange zone. Current subdivision of zone coloring is based on how many people are affected there. This has a loop hole that it cannot warn people before the spreading. Once a certain fraction of people get affected then only the color is designated or changed. This leads to people in green zone becoming careless and casual which in turn boosts covid19 spread.
Instead of this, people should be warned before the spreading actually takes place in that region. We propose a real time tracking of regions which will predict the region of being potentially hazardous to covid-19 based on various historical and present factors. This can warn people well in time so that they are not casual towards taking precautions in that area.We use predictive time series analysis model based on real time daily updates from trusted database such as https://www.covid19india.org/. We use a frame size of past 14 days updates (the phase of coronavirus blooming ) to predict the coloring of regions and it will change on real time basis. This will give the user a clear idea about the current and future scenario of there area. Features used are nearby region count of covid19, testing rate, recovery rate, death rate, Availability of doctors and beds, population density of region, active cases, migration rate of people, survival rate etc.

This feature can me incorporated with Community collaboration app so that demand and supply are done safely as well as it can serve as general purpose to ensure safety and secured life.
## How it works

A Supplier (who may be a regular resident, a small business, a voluntary organization, etc.) that has food, supplies, resources, or other essentials they can provide opens the mobile application and fill up a brief form that indicates what they have. This information is then stored in a database in the IBM Cloud.

A Recipient, who is in need of food, supplies, resources, or any such resources can open the mobile application and can use the chat interface to locate supplies near them. For instance, they might type "Where can I find bread?" or "Can someone collect my shopping for me?" The mobile application then accesses the database (after first understanding the question via Watson Assistant) and then displays a map showing locally where they can find what they are looking for.

Covid 19 Tracker to track and warn the people before the spreading in the community by analysing the real time increment in cases in the local region.

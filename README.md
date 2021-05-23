# **Covid\_bot V1**

- Covid\_bot V1 was solely made for educational and informative purposes.
- We are not intended to misguide the users through our service.
- All the data regarding COVID19 that we will be working on is from Government health bulletins and reputed news channels and blogs.

## **About :**

Covid\_bot V1 was a computer automated COVID informative service which updates the users with COVID updates directly through their whatsapp chat.

It is a non profit service

We expect
- No signup
- No fees
- No registration
- No standalone app or website running
- No special permission granted

Users will start receiving COVID updates every morning once they send their state name to the assigned whatsapp chat.

## **How it works:**

Assigned whatsapp account will be under automation using webdrivers(selenium)

The background python code will solely be responsible for processing the messages and responses in whatsapp chat.

### **wh.py :**

This code was responsible for responding to user&#39;s messages and accordingly

This code continuously checks for new messages and act according to them

### **graphs.py:**

This code was responsible for fetching the COVID19 related data from API, filter, process and plot graphs with the processed data.
Once all the data processing was done, this code temporarily shuts down wh.py execution.
Then it sends the plotted graphs and data to users according to their subscribed state.
Once all the users were updated, this code shuts down thereby waking up wh.py execution.

This cycle repeats every 24 hours

### **classes.py :**

This code provides the necessary defined classes and methods for wh.py and graphs.py in their execution

## **Privacy measures taken :**

- The only data that will be stored as subscription data was your phone number and subscribed state.
- To avoid threat prone to local databases on computers through LAN trespassers, we avoided use of database engines.
- The user&#39;s subscription data was stored in csv format with separate user privilege, so that the data is not prone to internet frauds and is completely bootstrapped.
- Once the user has unsubscribed from the service, all the users subscription data will be completely wiped off.
- The bot has no trackers to track your chat behaviour, it is made to act on a request model.

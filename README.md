# GateSec

## Classes:
* admin
* resident / user
* guest

# Implementation Options
- HTML5, CSS3

    - ### React Route
        * React by Facebook
        * Cordova
        * Node.JS
    
    - ### MEAN Stack
        * MongoDB - noSQL
        * AngularJS
        * ExpressJS
        * Node.JS

## Installing & Initializing System

### Admin configures basic settings
* length of time before entry expires
* number of guests allowed
    - per day / per month / per week (some time unit)
    - per household at any given period of time
        - [e.g] household can have up to 5 guests within the hour.
* maximum number of devices per household
    - *think number of key copies per house*
* amount of history stored
    - by time [month, year]
* number of times allowed to delete registered devices per __
    - [e.g.] Google Music implementation
* toggle for legacy implementation
    - [e.g.] if the community/organization is using their old system
* toggle for no guests allowed
    - optional; in case there's a reason for it.
* toggle to turn off scheduled entries
    - [e.g] gardeners, housekeepers

### Admin inputs *.csv* or manually inputs list of residents/users
* [label][email] ```string,string```
* Resident accounts are generated into the system
* Resdients are automatically emailed with PIN
    - PIN is a random, one-time use key to configure username / password.
    - Option to print temporary passes for access.

## Account Management (Admin)
* includes options to modify all settings above.
* edit resident settings
    - add new residents
    - remove residents
        - [e.g.] old residents moved out
    - update residents
        * add maximum number of devices on a house-to-house basis
            - [e.g.] if there is a household of 10
            - expiration date for maximum number of guests for that day/week/month
        * update email
    - include information of the resident
* print list of residents
    - ♯ of devices registered out of __
    - ♯ of guests registered out of __ per [configured unit of time]
    - guest log
    - label, email

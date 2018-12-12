FINN enables your IoT devices to perform seamless autonomous payments on your behalf. For more information, visit makethingsFINN.com.

# Requirements
This SDK works on Debian devices like Raspberry Pi or a regular Ubuntu.

# Getting Started
Visit our official documentation on docs.bankingofthings.io for a complete overview. The main steps are:

- Setting up your device (e.g. a Raspberry Pi)
- Installing the SDK
- Defining Actions on the portal
- Pairing the device with your phone
- Trigger actions on your device
- Check results in your dashboard
- Installation

# Cloning the repository
Clone the repository on your device, for example with ssh, and enter the folder:
git clone [BankingofThings/BoT-NodeJS-SDK](git@github.com:BankingofThings/BoT-NodeJS-SDK.git) 
cd BoT-NodeJS-SDK

Creating your environment
As for now, this SDK supports debian based environments. To setup your environment, run:
make environment-debian
For development you can use macOS with Xcode installed.

Installing dependencies
To install dependencies run:
make install

Configuration
On your first run, replace YOUR_MAKER_ID with the makerID from your FINN Account and run:
make server makerID=YOUR_MAKER_ID

Running the server
To run the server normally after you've configured it, simply run:
make server Using the SDK

Pairing your device
curl localhost:3001/pairing
Retrieving actions
curl localhost:3001/actions
Triggering actions
curl -d '{"actionID":"YOUR_ACTION_ID"}' -H "Content-Type: application/json"
http://localhost:3001/actions

# Contributing
All improvements to the FINN SDK are very welcome! Our software is open-source and we believe your input can help create a lively community and the best version of FINN. We’ve already implemented much of the feedback given to us by community members and will continue to do so. Join them by contributing to the SDK or by contributing to the documentation.

Running tests
At the moment we do not have high test-coverage. You're free to make a PR to add tests! To run the tests:
make test

# Community

Slack
Slack is our main feedback channel for the SDK and documentation. Direct feedback
Use the feedback button on the portal.

Meetups
We also organize meetups, e.g. demo or hands-on workshops. Keep an eye on our meetup group for any events coming up soon. Here you will be able to see the FINN software in action and meet the team.
[Meetup/Amsterdam-ING-Banking-of-Things](meetup.com/Amsterdam-ING-Banking-of-Things/).
 
# About FINN
After winning the ING Innovation Bootcamp in 2017, FINN is now part of the ING Accelerator Program. Our aim is to become the new Internet of Things (IoT) payment standard that enables service-led business models. FINN offers safe, autonomous transactions for smart devices.
We believe our software offers tremendous business opportunities. However, at heart, we are enthusiasts. Every member of the team has a passion for innovation. That’s why we love working on FINN
makethingsfinn.com

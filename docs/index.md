![POP Logo](img/pop-logo_320px.png "POP")

# Instructions

## Overview
In POP, programs are organized lists of outreaches where agents can follow an easy to use script when making an outreach to a contact. Once finished, the agent can record awareness, comments, statuses, and sentiment and then automatically retrieve the next contact to make an outreach to.

## Setup

### Configuration

1. To make adding contacts to a program easier, a list view and record action is available for Contacts.

### Assigning Permissions

1. Assign **POP Program Admin** to a user to be the administrator for all programs.
2. Assign **POP Program Owner** to any users that will be managing specific programs.
3. Assign **POP Program Agent** and **POP Program Translator** to any users that will be executing the progam.
4. Assign **POP App** to agents and translators if they are internal users and will need access to the app.

## Managing Programs

### Create a Program

Program owner creates programs and reads each field help text to understand various features.

### Create Default Script
 
Program owner should use Create Default Script button on Program and edit the script as desired. If you have multiple languages, clone an existing script, change the language and edit as desired.

###Add Contacts as Outreaches

Program owner adds contacts they wish to make outreaches to. Use the Test region, to add test contacts in order to train and on-board agents. Note that these contacts email address should not be real. Otherwise, an email, if that option is selected, will kick off.

###Share Program with Agents and Translators

Program owner shares the program with agents and translators by using the **Share** button.

### Activate and train on Program

When ready, program owner marks the program as active allowing agents to execute the program. Agents simply visit the program record page and follow the script.

That's how easy it is to run an outreach program!

## Advanced Features

1. Use the **Clone Unconnected Outreach** button to clone outreaches that did not connect with a contact (e.g. a voice mail was reached). With this, you can do a follow-up to try and reach contact.
2. Use the **Close Account on Unconnected** option if you want to close all outreaches if you **connect** with at least one contact at the Account.
3. By default, an email will be sent for outreach if the program hasn't excluded, the contact has an email address, and the contact has said they wish to receive an email. You can update the subject and body of email in the script. Use {{{First_Name}}} merge variable to make the email more personal.

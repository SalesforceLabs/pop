![POP Logo](img/pop-logo_320px.png "POP")

# Overview
POP allows you to organize a lists of contacts into a program where agents can then follow an easy to use script to make outreaches to every contact. A POP program can be run with many agents simulataneously making outreaches without inadvertantly trying to connect to the same contact. Before an outreach is finished, the agent can record useful reportable information such as awareness, comments, statuses, and sentiment. After an outreach is finished, the next outreach is automatically retrieved making it quick and easy to make your customers aware of your programs.

# Installation

## Latest Release                                                      

Current Release 0.1.0.12
                                                                         
Sandbox & Scratch Orgs:                                                   
https://test.salesforce.com/packaging/installPackage.apexp?p0=04t8Z000000lCjoQAE                                                                    

Production & Developer Edition Orgs:                                      
https://login.salesforce.com/packaging/installPackage.apexp?p0=04t8Z000000lCjoQAE    

# Instructions

## Setup

### Configuration

#### Make adding Contacts to Outreach Programs Easier

Included in this package are 2 buttons called **Add to Outreach Program**, one for Contact record page and one for Contact list views. Consider adding these buttons to make adding contacts to outreach programs easier. When adding the button, set the visibility to only show if the current user has the **Can_Add_to_Outreach_Program** custom permission. Additionally, consider adding **Program Outreaches** related list with fields such as name, status, closed date/time, awareness so users who submitted an outreach are aware of the status.

### Assign Permissions

1. Assign **POP Program Admin** to a user to be the administrator for all programs.
2. Assign **POP Program Owner** to any users that will be managing specific programs.
3. Assign **POP Program Agent** and **POP Program Translator** to any users that will be executing the progam.
4. Assign **POP Program Submitter** to any users that will be submitting contacts to outreach programs.
5. Assign **POP App** to agents and translators if they are internal users and will need access to the app.

## Manage Programs

### Create a Program

Program owners create programs. Programs have several configuration options.
- Allow Add to Outreach Program: Allow other user's the program is shared to add outreaches to a program (beta).
- Close Account on Connected: Close all outreaches if you **connect** with at least one contact at the Account.
- Exclude Send Email Script: By default, an email will be sent for outreach if the program hasn't excluded email, the contact has an email address, and the contact has said they wish to receive an email, and the script has content in email body and subject fields. You can update the subject and body of email in the script. Use {{{First_Name}}} merge variable to make the email more personal.

### Create a Default Script
 
Program owners can use the **Create Default Script** button on a Program and then edit the script as desired. If you have multiple languages, clone an existing script, change the language and edit as desired.

### Add Contacts to the Program as Outreaches

Program owners add the contacts they wish to make outreaches for. If the program is shared with users with the POP Program Submitter permission set and the contact layout has the **Add to Outreach** button added, those users can submit contacts on behalf of program owners.

Use the Test region to add contacts for training and on-boarding agents. Note, currently, that these contacts email address should not be real. Otherwise, an email, if that option is selected, will kick off.

### Share the Program with Agents and Translators

Program owners share the program with agents and translators by using the **Share** button. Read only access is all that is needed for agents to interact with the program. Program admin needs to ensure that these users should be assigned an appropriate permission set.

### Activate Program and On-Board Agents

When ready, program owners mark the program as active which allows agents to actually execute the program. Agents simply visit the program record page and follow the script.

*That's how easy it is to run an outreach program!*

## Considerations

1. By default, all outreaches will be set to English language and AMER region. If you would like to change this, create Flow based trigger that set new outreaches to values from your contact records.

## Advanced Features

1. Use the **Clone Unconnected Outreach** button to clone outreaches that did not connect with a contact (e.g. a voice mail was reached). With this, you can do a follow-up to try and reach contact.

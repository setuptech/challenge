


# SETUP TECH Mobile Developer Technical Challenge

### Business Requirement
As an user I want to be able to see a list of my mails, including mail attachment photo, title and date. I also want to be able to see the mail details on the details screen and full description when I click on the mails list item.

### API Clarification
### Get Mails

* Protocol `HTTP`
* Hostname `assessment.dev01.squaredbyte.com`
* Method `GET`
* Endpoint `/api/public-letter-list`
*  Query String Parameters
    - offset

      * Description: Starting index.
      * Data type: Integer.
    - limit

      *  Description: Number of mails requested
      *  Data type: Integer.

 * API Response example: HTTP code 200

          [
             {
            "id": 4,
            "title": "Title 1",
            "subject": "Subject of Title One",
            "destino": "Albufeira",
            "photo": [
                "http://assessment.dev01.squaredbyte.com/upload/5bffc01643fde.png"
            ],
            "document_number": 2,
            "deadline": "2018-11-28 16:27:00",
            "status": "Pending",
            "created_at": "2018-11-29 10:31:50",
            "event": "create",
            "destination": "Web Development",
            "destination_type": "Department",
            "perform_by": "admin admin",
            "letter_id": 4
        },
        {
            "id": 6,
            "title": "Title 1",
            "subject": "subject of test one",
            "destino": "Almada",
            "photo": [
                "http://assessment.dev01.squaredbyte.com/upload/5bffc0ca44c7b.png",
                "http://assessment.dev01.squaredbyte.com/upload/5bffc0ca560e9.png",
                "http://assessment.dev01.squaredbyte.com/upload/5bffc0ca66c06.png"
            ],
            "document_number": 1,
            "deadline": "2018-11-28 16:27:00",
            "status": "Pending",
            "created_at": "2018-11-29 10:34:50",
            "event": "create",
            "destination": "admin admin",
            "destination_type": "User",
            "perform_by": "admin admin",
            "letter_id": 6
        },
       ...
       ]
    

###  User Requirements
* Retrieve list of mails from the API
* Display list of mails.
* Show details when user select an item in the list.
* Show photo slider on details screen based on the provided attachment mail photos

### What we expect exactly?
Production ready solution at your utmost level.

### Technical Requirement
* Source code must be stored in a github/gitlab repository
* For public repos:

  - Avoid words `setuptech`,`mobile`,`mails` and `challenge` in your projects
  - Do not copy-paste any part of this file (task, API documentation, etc.)
  
* App should cache mails (Cached mails should be available in offline)
* Could fetch up to maximum 20 mails per API call
* You are free to use any libraries/Wrappers
* Storyboard or XIB is not allowed
* Create UI(Layout) using code only
* Layout must fit in all Devices(Universal)
* Must write in the latest Xcode version

### Wireframe
These UI/UX are for reference only, you can be creative with designs and UI/UX features. 

<table>
<tr border=0>
<td border=0><img src="https://user-images.githubusercontent.com/45398704/49221463-6a484300-f403-11e8-8518-50d234c8ccba.jpg" width="420px"  /></td>
<td border=0><img  src="https://user-images.githubusercontent.com/45398704/49221457-61f00800-f403-11e8-911b-f9af06f4ad1c.jpg" width="420px"/></td>
</tr>
</table>






### Any Questions? We love to get back soon with answers: techchallenge@setup.technology  

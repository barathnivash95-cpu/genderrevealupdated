# Gender Reveal Invitation - Google Form Connected

This version is connected to your Google Form.

## Connected form

Google Form action URL:

https://docs.google.com/forms/d/e/1FAIpQLSdZTY0rJIlz7nPAf2pHAbcJNnT05JV7Y8Oa0qnABLXpYsjldQ/formResponse

## Entry mapping

- Family / Guest Name: entry.1397653953
- Attendance: entry.679553306
- Number of persons attending: entry.695882065
- Vegetarian count: entry.985480686
- Non vegetarian count: entry.1225710060
- Any allergies: entry.1157302185
- Message for the parents-to-be: entry.610660446

## Upload to GitHub

Upload these extracted files to your GitHub repository root:

- index.html
- README.md
- .nojekyll
- assets folder

- invitation paragraph shortened and made more welcoming/funny
- parking paragraph replaced with: Parking available at the event hall.


## Title position update

- Moved "He or She? Come & See!" upward to the blank top area.
- Shifted the background couple image downward so the title does not hide the face.
- Kept the Google Form connection and latest wording.


## Title position update
- Moved He or She / Come & See down to the red-marked blank area.


## Cloud position update
- Moved kutti and kuttan slightly downward.

## Text line update
- Kept "Come & See!" on the same line, especially on mobile.


## Time and button update
- Time changed to 10:30 AM – 1:30 PM.
- Tap button changed from Tap to Open to Tap to Scroll.

## Not attending Google Form fix

For Not attending responses, the form now sends:
- Number attending: 0
- Vegetarian count: 0
- Non vegetarian count: 0
- Allergies: N/A
- Message: guest message, or N/A if blank

This helps Google Forms store the response even if some form questions are marked required.

## Reliable Not Attending fix

This version uses a real hidden form POST to Google Forms instead of fetch/no-cors.

For Not attending, it submits:
- Attendance: Not attending
- Number attending: 0
- Vegetarian count: 0
- Non vegetarian count: 0
- Allergies: N/A
- Message: entered message or N/A

Important:
In Google Forms, make sure Attendance option text is exactly:
- Attending
- Not attending

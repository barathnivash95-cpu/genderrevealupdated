# Gender Reveal Invitation - Google Form Ready Version

This version has Google Forms submission code added.

## What changed

- RSVP will submit directly to Google Forms after you connect your Google Form URL and entry IDs.
- You can connect the Google Form responses to Google Sheets.
- Until you replace the placeholders in `index.html`, the submit button will show a warning.

## Google Form questions to create

Create a Google Form with these questions:

1. Family / Guest Name
2. Attendance
3. Number of persons attending
4. Vegetarian count
5. Non vegetarian count
6. Any allergies
7. Message for the parents-to-be

## How to connect it

Open `index.html` and find this section:

```js
const GOOGLE_FORM_ACTION_URL = "PASTE_YOUR_GOOGLE_FORM_FORMRESPONSE_URL_HERE";

const GOOGLE_FORM_ENTRIES = {
  familyName: "entry.PASTE_FAMILY_NAME_ID",
  attendance: "entry.PASTE_ATTENDANCE_ID",
  personCount: "entry.PASTE_PERSON_COUNT_ID",
  vegCount: "entry.PASTE_VEG_COUNT_ID",
  nonVegCount: "entry.PASTE_NON_VEG_COUNT_ID",
  allergies: "entry.PASTE_ALLERGIES_ID",
  message: "entry.PASTE_MESSAGE_ID"
};
```

Replace each placeholder with the real Google Form values.

## How to get the formResponse URL

Your Google Form link normally looks like:

`https://docs.google.com/forms/d/e/YOUR_FORM_ID/viewform`

Change the last part from:

`viewform`

to:

`formResponse`

So it becomes:

`https://docs.google.com/forms/d/e/YOUR_FORM_ID/formResponse`

## How to get entry IDs

1. Open your Google Form.
2. Click the three dots menu.
3. Choose **Get pre-filled link**.
4. Fill sample text in every field.
5. Click **Get link** and copy the link.
6. The copied link will include values like:
   `entry.123456789=Sample`
7. Copy each `entry.xxxxx` value into the matching field in `index.html`.

## Upload to GitHub

Upload these extracted files to your GitHub repository root:

- `index.html`
- `README.md`
- `.nojekyll`
- `assets` folder

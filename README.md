# Parent Child Component Demonstration

This project is to demonstrate how to reuse a component on a record as well as a related record.
In this example, we will create a Lightning Web Component called "accountHighlights" which displays the fields and values that are displayed on the Account's Highlights panel.
We will also create a component called "contactAccountHighights" which administators can use to display the accountHighlights component on any related contact record as well.

## Account Highlights Component

This component will use lightning-record-form to display the compact layout for an Account

## Contact Account Highlights Component

This component will wrap around the accountHighlights component to render the account highlights for a given contact. This component uses the getRecord wire adapter to get the field values for the contact (specifically, the AccountID), then the component will pass that Id in as recordId for the nested accountHighlights component.



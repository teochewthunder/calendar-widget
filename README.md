# JS Datepicker

For each datepicker, there should be a `span` element which has styling set to `position:relative` and a `z-index` depending on which datepicker's controls should appear at the top. Each datepicker should also have an id. This id is used immediately within a `script` tag, via a call to `calendar.initialize()`.

All the Javascript is encapsulated within the `calendar` object. The idea here is that the JavaScript will then proceed to populate these `span` elements with controls.

These controls include:
- buttons for incrementing/decrementing month and year
- drop-down list for selecting month
- each displayed day is a button for selecting the date
- read-only text box for displaying selected date in a "pretty" format
- hidden text box to store the *actual* date value in the required format.

Each of these controls will have an id which is an expanded form of the parent `span` elment's id. This is to make them easy to reference when the parent `span` element is referenced.

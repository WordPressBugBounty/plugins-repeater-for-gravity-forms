=== Repeater Fields for Gravity Forms ===
Contributors: addonsorg
Tags: Gravity Forms, Gravity Forms fields, Repeater, Repeater form, Repeater field
Requires at least: 2.0
Tested up to: 7.1
Stable tag: 3.2.2
Requires PHP: 5.2
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

The Repeater Fields for Gravity Forms allow you to create one or more sets of fields that can be repeated.

== Description ==

[youtube https://www.youtube.com/watch?v=gaWE0IqjYsI]

**DEMO**: <https://demo.add-ons.org/demo-repeater-fields/>
**Document**: <https://add-ons.org/document-gravity-forms-repeater-fields/>
**Download Pro Version**: <https://add-ons.org/plugin/gravity-forms-repeater-fields/>

The Repeater Fields for Gravity Forms allow you to create one or more sets of fields that can be repeated.

Have you ever wanted to let your users submit multiple entries of the same field set as a single form on your WordPress site? If so, you’re in luck! This is a plugin to help you do it!

### Save and Continue Later Support
Fully compatible with Gravity Forms' built-in **Save and Continue Later** feature! When users save their unfinished submission and return via the save token link:
* **Preserves All Repeated Rows**: All added rows are automatically re-created in their exact order.
* **Restores Field Data**: Inputs including text, numbers, dates, checkboxes, radio buttons, and pricing choices are restored.
* **Retains Uploaded Files**: Attachments and files uploaded inside repeater rows are safely preserved across draft sessions.

== Features ==
- **Initial Rows & Field Mapping (Pro)**: Set custom default row counts or link repeater rows dynamically to a number/dropdown field (e.g., Number of Guests/Tickets).
- **Save and Continue Later Support**: Seamlessly saves and restores all repeated rows and input values when resuming draft submissions.
- **Pricing & Payment Fields (Pro)**: Calculate Product, Option, and Quantity inside Repeater rows with real-time Total calculation and payment gateway integration.
- **File Uploads Support**: Allow single or multiple file uploads inside repeated rows.
- **Minimum Rows**: Sets a limit on how many rows of data are required.
- **Maximum Rows**: Sets a limit on how many rows of data are allowed.
- **Button Label**: Customizable text shown on the ‘Add Row’ button.
- **Conditional Logic support**: Supports conditional logic inside and outside repeaters.
- **Date picker support**: Full date/time picker support inside repeated fields.
- **Entry and print preview support**: Easily view, export, and print repeated entries.
- **Drag and drop repeatable fields**: Simple and flexible form builder experience.

### Pricing & Payment Fields Support (Pro)
Easily create repeatable booking, ticket, quotation, or registration forms! With the Pro version, you can place Gravity Forms **Pricing Fields** (Product, Option, and Quantity) directly inside your repeaters:
* **Real-time Price Calculation**: The form's Total field updates dynamically in real time as customers add, remove, or modify repeated rows.
* **Supports All Product Types**: Single Product, Drop Down, Radio Buttons, User Defined Price, and Calculation products.
* **Option & Quantity Support**: Sub-options (Drop Down, Radio, Checkboxes) and item quantities are calculated per individual repeater row.
* **Payment Gateways Integration**: Seamlessly passes line items and totals to payment add-ons including Stripe, PayPal, Mollie, Square, and Authorize.net.
* **Detailed Order Summary**: View entry details with full itemized breakdown (Row 1, Row 2, etc.) for admin review, notifications, and customer emails.

### Dynamic Initial Rows Count & Field Mapping (Pro)
Control exactly how many rows appear when the form loads, or bind repeater row counts dynamically to another form field:
* **Custom Initial Rows Count**: Set any specific number of rows to display by default upon page load (e.g., start with 0, 1, 3, or more rows).
* **Smart Field Mapping**: Connect the repeater directly to another field in your form (such as a Number, Drop Down, or Quantity field) using its Field ID.
* **Instant Dynamic Row Generation**: When the user enters or selects a number (e.g., "Number of Attendees: 4"), the repeater automatically expands to create exactly 4 rows in real time.
* **Streamlined User Experience**: Optionally locks the row count and hides manual "+ Add Row" / delete buttons when mapped, preventing submission mismatches for ticket bookings, group registrations, and order forms.

== Pro Version ==
* Dynamic Initial Rows count & Field Mapping (Auto-generate rows based on user input)
* Pricing & Payment Fields support (Product, Option, Quantity, Total)
* Real-time Total price calculation on add/remove rows
* Payment gateways integration (Stripe, PayPal, Mollie, Square, etc.)
* Order summary breakdown per repeater row
* File Upload Support (Single & Multi-file)
* Conditional Logic support
* Unlimited minimum & maximum rows
* 30-day money-back guarantee
* 1-year support

== Installation ==
**Normal installation**

1. Download the repeater-for-gravity-forms.zip file to your computer.
2. Unzip the file.
3. Upload the `repeater-for-gravity-forms` directory to your `/wp-content/plugins/` directory.
4. Activate the plugin through the 'Plugins' menu in WordPress.
5. Document: https://add-ons.org/document-gravity-forms-repeater-fields/

== Frequently Asked Questions ==

= What is "Initial Rows Count" and how does "Field Mapping" work? =
**Initial Rows** allows you to choose how many rows are automatically displayed when the form loads. If you set it to 0, no rows show up until the user clicks "+ Add Row"; if set to 3, three rows appear immediately.

**Field Mapping with Initial Rows** allows you to enter the Field ID of another field in the form (such as a Number or Dropdown field asking "How many guests/tickets?"). When the user selects or enters a number (e.g., 4), the repeater automatically renders exactly 4 rows in real time without requiring the user to click "+ Add Row" four times.

= Does it work with Gravity Forms Save and Continue Later? =
Yes! The plugin fully integrates with Gravity Forms' "Save and Continue Later" feature. When users save their progress, all repeated rows and entered field values are saved to the draft. When they open the resume token link (`?gf_token=...`), the entire repeater structure, all field values, and uploaded files are automatically restored.

= Can I use Pricing, Product, and Option fields inside the repeater? =
Yes! With the Pro version, you can place Product, Quantity, and Option fields between Repeater Start and Repeater End. The form Total automatically updates as users add/remove rows or change values.

= Does it work with payment gateways like Stripe and PayPal? =
Yes, in the Pro version, line items from each repeater row are properly registered in Gravity Forms order info (`gform_product_info`), allowing Stripe, PayPal, and all Gravity Forms payment add-ons to charge the accurate order total.

= How do repeated products appear in Entry Details and Confirmation Emails? =
Each repeated row is itemized in the Order Summary table (e.g., "Ticket (Row 1)", "Ticket (Row 2)") along with chosen options, quantities, and subtotal.

== Screenshots ==

1. Frontend Working
2. Backend Field
3. Admin builder

== Changelog ==
= 3.2.1 =
- Added: Pricing Fields support in Repeater (Pro) - Dynamic calculation for Product, Option, Quantity fields and payment gateway integration.
- Added: Full support for Save and Continue Later - Automatically preserves and restores all repeated rows, entered field values, and files when resuming via draft token link. 

= 3.2.0 =
- Fixed: Radio field Required

= 3.1.1 =
- Fixed: Resolved '$element.datepicker is not a function' error by adding jquery-ui-datepicker dependency.
- Fixed: security issue

= 3.0.3 =
- Fixed: state_validation

= 3.0.1 =
- Fixed: Input Mask

= 3.0.0 =
- Fixed: PHP Fatal error:  Declaration of Superaddons_GFRepeater_Field::get_field_label

= 2.5.1 =
- Fixed: upload field on multi-step form

= 2.5.0 =
- Fixed: Phone field

= 2.4.5 =
- Fixed: conditional logic radio

= 2.4.4 =
- Added: Fixed Required upload field

= 2.4.2 =
- Added: Translate

= 2.4.0 =
- Fixed: Save datas

= 2.3.5 =
- Fixed: Required field


= 2.3.4 =
- Fixed: CSS Orbital Theme 
- Fixed: Date select type

= 2.3.2 =
- Fixed: for label

= 2.2.7 =
- Fixed: Checkbox label

= 2.2.6 =
- Fixed: Important

= 2.2.5 =
- Fixed: Compatible with Gravity Forms Chained Selects Add-On 

= 2.2.4 =
- Fixed: Multi Select field

= 2.2.3 =
- Fixed: https://wordpress.org/support/topic/possible-bugfix-fieldids-99-breaking-conditional-logic/

= 2.2.2 =
- Fixed: Upload multiple files

= 2.2 =
- Fixed: Conditional logic

= 2.1.6 =
- Fixed: set Initial Rows = 0

= 2.1.5 =
- Fixed: Conditional logic out repeater

= 2.1.4 =
- Fixed: Save Radio submit

= 2.1.3 =
- Fixed: Export entries

= 2.1.2 =
- Fixed: Maps with field

= 2.1.0 =
- Fixed: Uncaught ReferenceError: gform is not defined

= 2.0.9 =
- Fixed: Radio

= 2.0.8 =
- Fixed: Conditional logic with end repeater

= 2.0.7 =
- Fixed: Conditional logic 

= 2.0.6 =
- Fixed: Input Mask

= 2.0.5 =
- Fixed: shortcode end tags

= 2.0.4 =
- Fixed: Active the plugin

= 2.0.3 =
- Fixed: Big update

= 1.0 =
- Version 1.0 Initial Release
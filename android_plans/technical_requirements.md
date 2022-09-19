# RedBucketRealty: Android app Requirements

The requirements for the RedBucketRealty android app are:

- Create a base theme, and vary for light, and dark color themes. Document it.
- Add a font set to the theme. Document it.
- Create a logo.
- Create a splash screen that shows the logo for 2 seconds
- Create a login screen
  - Add fields for login details: email and password
  - Add a button for login
  - Add a button for reset password
  - Add a button for register account
  - Navigate to 2FA screen
- Create a signup screen
  - Add fields for signup: username, email, password
  - Add a button for signup
  - Add a button for login
  - Check password with PwnedPasswords service
  - Navigate to 2FA screen
- Create a 2FA screen page
  - Add a field for 2FA code
  - Add button to choose another 2FA method
  - Add a button to go back
  - Add a button to resend code
  - Display text to check 2FA method
  - Add button to verify code
    - Navigate to home page
- Create a choose 2FA page
  - Display list of 2FA options
  - Navigate to 2FA login screen with option
- Create a 2FA screen for signup
  - Display list of 2FA options
  - Navigate to 2FA registration screen for option
- Create a email 2FA screen for signup
  - Add a field for 2FA code
  - Add a button for verifying code
  - Add a button to navigate to 2FA screen for signup for choosing another method
- Create a TOTP 2FA screen for signup
  - Add a field for 2FA code
  - Display a QR code
  - Display a TOTP key
  - Add a button to copy TOTP key
  - Add a button for verifying code
  - Add a button to navigate to FA screen for signup for choosing another method
- Create a home page
  - Create a bottom navigation that lists the home page, cart page, orders page, and the profile page as fragments
  - Have a chip at the top to remind about KYC
  - Add a recommended products and services section that has recommended products and services in a horizontal list
    - Display a  heading like `Recommended` or `Picked for you` or something similar
    - Display product items in a horizontal list
    - Items should have a name, an image, and a favorite icon
    - Navigate to item on click
  - Add a new section that has new products and services in a horizontal list
    - Display a  heading like `New` or `Just released` or something similar
    - Display product items in a horizontal list
    - Items should have a name, an image, and a favorite icon
    - Navigate to item on click
  - Add a section for<!-- TODO: Add sections -->
- Create a cart page
  - Display product items added to cart
    - Display an image of the product item
    - Display the name of the product item
    - Display cost of the product item
    - Display amount of the product item
    - Display status of the rental agreement of the product item
    - Display a button to add to Buy Later list
    - Navigate to product items when clicking on the product image
    - Add button to add to favorites
    - Add button to remove product item from cart
    - Add button to increment or decrement amount of the product item
    - Add button to move to Buy Later list
    - Add button to sign rental agreement of the product item
  - Display a total cost amount added
  - Display icons of compliances needed to fulfill the orders
  - Add a button to navigate to KYC and Compliance page
  - Add a button to go to payment portal
    - Display list of compliances
      - Navigate to them on click
    - Display list of rental agreements
      - Navigate to them click
    - Go to payment portal only if:
      - All rental agreements are signed
      - All compliances are fulfilled
  - Display product items in the Buy Later list, if not empty
    - Display an image of the product item
    - Display the name of the product item
    - Display cost of the product item
    - Add button to move it to cart
    - Add button to remove it from the buy later list
- Create a favorites page
  - Display favorites lists
    - Display index number of the list
    - Display name of the list
    - Navigate to lists on click
  - Add button to create a new favorites list
  - Multi-select lists on long press
    - Display number of selected favorites lists
    - Display button to delete favorites lists
      - Display a dialog
        - Display confirmation text
        - Add button to delete
        - Add button to cancel
  - Display most recently added products to the favorites list.
    - Display name of the product item
    - Display an image of the product item
    - Display cost of the product item
    - Display which favorites list the product item is in
    - Navigate to product items on click
- Create a favorites list page
  - Display product items in the list
    - Display name of the product item
    - Display an image of the product item
    - Display cost of the product item
    - Navigate to product items on click
  - Display the name of the list
  - Add button to delete list
    - Display a dialog
      - Display confirmation text
      - Add button to delete
      - Add button to cancel
    - Navigate back to favorites page before deleting list
  - Add button to sort items in the list
    - Display dialog
      - Display ways to sort items
      - Perform sort on click
  - Multi-select product items on long press
    - Display number of selected product items
    - Display button to delete product items
      - Display a dialog
        - Display confirmation text
        - Add button to delete
        - Add button to cancel
    - Display button to move product items to another favorites list
      - Display a dialog
        - Display favorites lists
        - Add button to move
        - Add button to cancel
    - Display button to move product items to cart
- Create an orders page
  - Display latest ordered product items
    - Display name of the item
    - Display an image of the item
    - Display status of the item
    - Navigate to item on click
  - Add button to renew items
  - Display items similar to previous orders
    - Display name of the item
    - Display an image of the item
    - Display price of the item
    - Navigate to item on click
  - Add button to view invoice
    - Navigate to invoice page
  - Add button to export invoice
    - Navigate to export invoice page
- Create an invoice page
  - Display a GST compliant invoice, like the one displayed at [Cleartax](https://cleartax.in/s/gst-invoice)
  - Add button to export invoice
    - Navigate to export invoice page
- Create an export invoice page
  - Add button to export invoice as PDF file
  - Add button to export invoice via email
  - Add button to export invoice as an image
- Create a Residential Properties page
  - Display product items
    - Display the name of the residence
    - Display an image of the residence
    - Display rent price of the residence
    - Display number of people for the home
    - Display size of the home
    - Display location of the residence
    - Display icons for amenities
      - Furnished
      - High-speed internet
      - Close to public transport
      - Vibrant neighborhood
      - Accessible
      - Elevator
      - Pets allowed
    - Add button to add to favorites
    - Navigate to Residential Property page on click
  - Add dropdown to sort residences
    - Sort by rent price of the residence
    - Sort by number of people for the home
    - Sort by size of the home
  - Add button to filter residences
    - By location
      - Display locations in a dialog
      - Display chip of selected location
      - Filter by that location
    - By amenities
      - Display amenities in a dialog
      - Display chip of selected amenities
      - Filter by that amenity
- Create a Private Office Spaces page
  - Display product items
    - Display the name of the private office
    - Display the image of the private office
    - Display the location of the private office
    - Display the rent price of the private office
    - Display the number of people for the private office
    - Display the size of the private office
    - Display icons for amenities
      - Furnished
      - High-speed internet
      - Close to public transport
      - Vibrant neighborhood
      - Reception service available
      - Business services available
      - Air-conditioned building
      - Accessible
      - Elevator
    - Add button to add to favorites
    - Navigate to Private Office Space page on click
  - Add dropdown to sort private office spaces
    - Sort by rent price of the private office space
    - Sort by number of people for the private office space
    - Sort by size of the private office space
  - Add button to filter private office spaces
    - By location
      - Display locations in a dialog
      - Display chip of selected location
      - Filter by that location
    - By amenity
      - Display amenities in a dialog
      - Display chip of selected amenities
      - Filter by that amenity
- Create a Shared Co-Working Spaces page
  - Display product items
    - Display the name of the shared co-working space
    - Display the image of the shared co-working space
    - Display the location of the shared co-working space
    - Display the service price of the shared co-working space
    - Display icons for amenities
      - High-speed internet
      - Close to public transport
      - Vibrant neighborhood
      - Reception service available
      - Business services available
      - Air-conditioned building
      - Food and catering available
    - Add button to add to favorites
    - Navigate to Shared Co-Working Spaces page on click
  - Add dropdown to sort shared co-working spaces
    - Sort by rent price
  - Add button to filter shared co-working spaces
    - By location
      - Display locations in a dialog
      - Display chip of selected location
      - Filter by that location
    - By amenity
      - Display amenities in a dialog
      - Display chip of selected amenities
      - Filter by that amenity
- Create an Event Spaces page
  - Display product items
    - Display the name of the event space
    - Display an image of the event space
    - Display the location of the event space
    - Display the rent price of the event space
    - Display the number of people for the event space
    - Display the size of the event space
    - Display icons for amenities
      - High-speed internet
      - Close to public transport
      - Air-conditioned building
      - Food and catering available
      - Parking and valet services available
    - Add button to add to favorites
    - Navigate to Event Spaces page on click
  - Add dropdown to sort event spaces
    - Sort by rent price of the event space
    - Sort by number of people for the event space
    - Sort by size of the event space
  - Add button to filter event spaces
    - By location
      - Display locations in a dialog
      - Display chip of selected location
      - Filter by that location
    - By amenity
      - Display amenities in a dialog
      - Display chip of selected amenities
      - Filter by that amenity
- Create a Virtual Spaces page
  - Display product items
    - Display the name of the virtual space
    - Display an image of the virtual space
    - Display the location of the virtual space
    - Display the rent price of the virtual space
    - Display icons for amenities
      - Reception service available
      - Business services available
      - Mail-handling available
    - Add button to add to favorites
    - Navigate to Virtual Spaces page on click
  - Add dropdown to sort virtual spaces
    - Sort by rent price of the virtual space
    - Sort by number of people for the virtual space
    - Sort by size of the virtual space
  - Add button to filter virtual spaces
    - By location
      - Display locations in a dialog
      - Display chip of selected location
      - Filter by that location
    - By amenity
      - Display amenities in a dialog
      - Display chip of selected amenities
      - Filter by that amenity
- Create a Residential Property page
  - Display basic information about the residential property
    - Display the name of the residential property
    - Display location of the residential property
    - Display a cover image of the residential property
    - Display the price tag of the residential property
    - Display advantages of the residential property that sets it apart from the rest
    - Display icons and information about what amenities are available in the residential property
      - Furnished
      - High-speed internet
      - Close to public transport
      - Vibrant neighborhood
      - Accessible
      - Elevator
      - Pets allowed
    - Display other marketing copy if it exists
    - Display icons and information about compliances needed
    - Display information about who is renting out the property
    - Display a button that leads to other images of the residential property
  - Add button to navigate to a google maps listing of the property
    - Show a location using longitude and latitude in Google Maps
  - Add button to view the rental agreement of the property
    - Navigate to View Rental Agreement page
  - Add button to add to favorites
  - Add button to add to cart
- Create a Private Office Space page
  - Display basic information about the private office space
    - Display the name of the private office space
    - Display location of the private office space
    - Display a cover image of the private office space
    - Display the price tag of the private office space
    - Display icons and information about what amenities are available in the private office space
      - High-speed internet
      - Close to public transport
      - Vibrant neighborhood
      - Reception service available
      - Business services available
      - Air-conditioned building
      - Food and catering available
    - Display icons and information about services offered in the private office space
    - Display other marketing copy if it exists
    - Display icons and information about compliances needed
    - Display information about who is renting out the private office space
    - Display a button that leads to other images of the private office space
  - Add button to navigate to a google maps listing of the private office space
    - Show a location using longitude and latitude in Google Maps
  - Add button to view the rental agreement of the private office space
    - Navigate to View Rental Agreement page
  - Add button to add to favorites
  - Add button to add to cart
- Create a Shared Co-working Space page
  - Display basic information about the shared co-working space
    - Display the name of the shared co-working space
    - Display location of the shared co-working space
    - Display a cover image of the shared co-working space
    - Display the price tag of the shared co-working space
    - Display icons and information about what amenities are available in the shared co-working space
      - High-speed internet
      - Close to public transport
      - Vibrant neighborhood
      - Reception service available
      - Business services available
      - Air-conditioned building
      - Food and catering available
    - Display icons and information about services offered in the shared co-working space
    - Display other marketing copy if it exists
    - Display icons and information about compliances needed
    - Display information about who is renting out the shared co-working space
    - Display a button that leads to other images of the shared co-working space
  - Add button to navigate to a google maps listing of the shared co-working space
    - Show a location using longitude and latitude in Google Maps
  - Add button to view the rental agreement of the shared co-working space
    - Navigate to View Rental Agreement page
  - Add button to add to favorites
  - Add button to add to cart
- Create an Event Space page
  - Display basic information about the event space
    - Display the name of the event space
    - Display location of the event space
    - Display a cover image of the event space
    - Display the price tag of the event space
    - Display the people accommodation capacity of the event space
    - Display icons and information about what amenities are available in the event space
      - High-speed internet
      - Close to public transport
      - Air-conditioned building
      - Food and catering available
      - Parking and valet services available
    - Display other marketing copy if it exists
    - Display information about who is renting out the event space
    - Display a button that leads to other images of the event space
  - Add button to navigate to a google maps listing of the event space
    - Show a location using longitude and latitude in Google Maps
  - Add button to view the rental agreement of the event space
    - Navigate to View Rental Agreement page
  - Add button to add to favorites
  - Add button to add to cart
- Create a Virtual Space page
  - Display basic information about the virtual space
    - Display the name of the virtual space
    - Display location of the virtual space
    - Display a cover image of the virtual space
    - Display the price tag of the virtual space
    - Display icons and information about services offered in the virtual space
    - Display other marketing copy if it exists
    - Display icons and information about compliances needed
    - Display information about who is renting out the virtual space
    - Display a button that leads to other images of the virtual space
  - Add button to navigate to a google maps listing of the virtual space
    - Show a location using longitude and latitude in Google Maps
  - Add button to view the rental agreement of the virtual space
    - Navigate to View Rental Agreement page
  - Add button to add to favorites
  - Add button to add to cart
- Create a View Rental Agreement page
  - Display text of the rental agreement
  - Display product item of the rental agreement
    - Display name of the product item
    - Display type of the product item
    - Display an image of the product item
    - Display location of the product item
    - Navigate to item on click
  - Add a button to navigate to Sign Rental Agreement Page
- Create a Sign Rental Agreement page
  - Display product item of the rental agreement
    - Display name of the product item
    - Display type of the product item
    - Display an image of the product item
    - Display location of the product item
    - Navigate to item on click
  - Add a button to navigate to View Rental Agreement Page on click
  - Add a button to send email verification code
  - Add a field to receive verification code
  - Add button to verify code
- Create a profile page
  - Display user data
    - Display user email
    - Display username
    - Display profile image
    - Add button to edit user data
      - Navigate to get authorization page for editing user data
  - Add button to Compliance and KYC page
  - Add button to referral page
  - Add button to Contact Us page
  - Add button to Get Help page
  - Add button to Licenses and Attributions page
  - Add button to Policies page
  - Add button to Notifications page
- Create an Edit User Data page
  - Display current email
    - Add a field to edit email
      - Display message that a verification email will be sent afterwards
    - Display message about verifying email address
    - Add a button to save data
    - Add a field to enter verification code
    - Display success or failure message
  - Display current username
    - Add a field to edit username
    - Add a button to save data
    - Display success or failure message
  - Display profile image
    - Add a button to edit profile image
    - Display success or failure message
  - Add a field to enter new password
    - Add a button to save data
    - Check password with PwnedPasswords service
    - Display success or failure message
- Create a get authorization page
  - Add field to enter password
  - Add button to authenticate
    - Display success or failure message
    - Navigate to get authorization with 2FA page
- Create a verify authorization with 2FA page
  - Add a field for 2FA code
  - Add button to choose another 2FA method
    - Navigate to choose 2FA page
  - Add a button to go back
    - Navigate to get authorization page
  - Add a button to resend code
  - Display text to check 2FA method
  - Add button to verify code
    - Navigate to Edit User Data page
- Create a Compliance and KYC page
  - Display text about whether KYC is completed or not
  - Display text about why KYC details are necessary
  - Display text about data policy
  - Add link to Data Policy page
    - Navigate to datapolicy page
  - Add a field to choose whether KYC is for personal or business account
  - Add a button to move to complete personal or business KYC page
    - Navigate to personal or business KYC page
- Create a Personal KYC page
  - Display information about what information is needed and why
  - Add a field for name
  - Add a date picker for date of birth
  - Add a few fields for billing address
  - Add a field for phone number
  - Add a field to enter Aadhaar number
  - Display text about uploading Aadhaar image
  - Display empty Aadhaar image placeholder
  - Add a field to enter PAN number
  - Display text about uploading PAN image
  - Display empty PAN image placeholder
  - Add a button to save data
- Create a Business KYC page
  - Display information about what information is needed and why
  - Add a field for name of the entity
  - Add a field for mailing address of the entity
  - Add a few fields for billing address
  - Add a field for alternative email address for legal
  - Add a field to enter GST number
  - Display text about uploading GST certificate image
  - Display empty GST certificate image placeholder
  - Add a field to enter PAN number of the entity
  - Display text about uploading PAN image
  - Display empty PAN image placeholder
  - Add a button to save data
- Create a Referral page
  - Display referral code
  - Display how many times referral codes have been used
  - Display list of times when referral code was used
- Create a Contact Us page
  - Display contact email
  - Add a button to copy email address
  - Add a button to create an email
  - Display link to website
  - Add a button to copy link
  - Add functionality to make link clickable
  - Display mailing address of the company
  - Add button to copy mailing address
- Create a Get Help page
  - Display support email
  - Add a button to copy email address
  - Add a button to create an email with support subject
  - Add a button to display link to knowledge section on website
  - Add a button to copy link
  - Add functionality to make link clickable
  - Add button to move to in app chat support
- Create a Licenses and Attributions page
  - Display clickable list of attributions
    - Create attribution page for each attribution
    - Navigate to attribution page
  - Display clickable list of licenses
    - Create license page for each license
    - Navigate to license page
- Create a Policies page
  - Display text copy about data policy
  - Add a button to move to data policy page
  - Display text copy about privacy policy
  - Add a button to move to privacy policy page
  - Display text copy for terms of use
  - Add a button to move to terms of use page
- Create a terms of use page
  - Display terms of use
- Create a privacy policy page
  - Display privacy policy
- Create a data policy page
  - Display data policy
- Create a Notifications page
  - Display clickable list of notifications
    - Display text of the notification
    - Display icon for unseen notifications
    - Display number of unseen notifications
  - Add a button to page more notifications
- Send push notifications
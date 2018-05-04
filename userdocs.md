# Hopefully to land with 4.9.6 release

Some notes for now:
https://woocommerce.wordpress.com/2018/05/04/woocommerce-3-4-gdpr-features/


From @allendav: I think we need to describe how to use each of the four things we added on a separate page i.e.
   
* Privacy Policy Page is now a setting under wp-admin > Settings
    * Let's you designate or create a privacy policy page
* Privacy Policy Editing Helper
    *Gathers privacy policy declarations from plugins that support them into a copy and pasteable view above the page editor when editing the privacy policy page
    *Highlights when a plugin's declarations change (including date)
* Personal Data Export tool
    * Designed around GDPR Right of Access requests
    * Under wp-admin > Tools
    * Allows administrators to send a confirmation link to users to confirm their personal data export request
    * Allows administrators to download or directly email a personal data export to those users
    * Export is in the form of a ZIP file with an HTML report inside
    * Includes hooks for plugins to add their own contributions to the report
* Personal Data Erasure tool
    * Designed around GDPR Right to Erasure requests
    * Under wp-admin > Tools
    * Allows administrators to send a confirmation link to users to confirm their personal data erasure request
    * Allows administrators to run a personal data erasure for those users
    * Informs administrators of any personal data that was retained by a plugin
    * Allows administrators to optionally delete registered user accounts
    * Includes hooks for plugins to erase personal data they collected
    * Works with new anonymization functions in WordPress core to anonymize things like IP addresses instead of just erasing them        
        
* seems like we might need a fifth article to summarize all four and then that fifth article could appear on the codex Main_Page, e.g. under Learn How to Use WordPress or something

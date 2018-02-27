# Knowledge Base

## What is personal data (@webdevlaw)
The European data protection framework pertains to personal data. This is defined as “any information relating to an identified or identifiable natural person.” This can be one piece of information or multiple data points combined to create a record.
 
Beyond personal data there is also sensitive personal data, defined as information about a person’s
 
* Racial or ethnic origin
* Political opinions
* Religious or philosophical beliefs
* Trade union membership
* Health data
* Sex life or sexual orientation
* Past or spent criminal convictions
 
Sensitive personal data requires stricter protections than regular personal data, and the consequences for its leakage or misuse are greater.

GDPR expands the definition of personal data to include
 
* Genetic data
* Biometric data (such as facial recognition or fingerprint logins)
* Location data
* Pseudonymised data
* Online identifiers
 
The latter definition is important for developers. It includes things like IP addresses, mobile device IDs, browser fingerprints, RFID tags, MAC addresses, cookies, telemetry, user account IDs, and any other form of data which is identifiable to a natural person.
 
The European term “personal data” differs from the American term “personally identifiable information.” The latter pertains to a much more limited set of information than the European model. It also does not see information as contextual, whereas the European framework emphasises the risks inherent in data aggregation.
 
Personal data is used by data controllers and data processors. The data controller is a person or an entity, such as you or your organisation, which decides what data is collected, how it is used, and whom it is shared with. The data processor is any entity other than the data controller who processes the data on their behalf. As a developer, you may be a data controller, you may be a data processor, and you may be both.

## What Personal Data do we find in Core (To Be Updated!)
The following data has to be considered for anonymising, deleting, etc:
1. For Users

   * User Login
   * User Pass
   * User Nicename
   * User Display Name
   * User Email
   * User URL
   
1. For Comments

   * Author name
   * Author email
   * Author IP
   * Author URL
   * Author user agent
 
 What is NOT considered to be anonymised (so only the above parts are needed):
 * Posts/comments : Once a user is anynomised, the post/comment cannot be linked to the user anymore so should not be further anonymised.

## How do others allow users to download their own data
1. Facebook

   * https://www.facebook.com/settings
   * At the bottom click on 'Download a copy of your facebook data'
   * What is included?
      + Posts, photos and videos you've shared
      + Your messages and chat conversations
      + Info from the About section of your Profile
      + See full list on https://www.facebook.com/help/405183566203254
   * Check also facebook ads: https://www.facebook.com/ads/preferences/

2. Twitter

   * https://twitter.com/settings/your_twitter_data
   * Re-enter your password
   * Find the list of what data is kept
   * At the bottom 'Request your data' to get it by email
   
3. Google

   * https://takeout.google.com/settings/takeout

Requiring multiple types of authentication greatly increases security over traditional username-password paradigm.

## Types of multi-factor authentication

1. Knowledge - Something you know
2. Possession - Something you have
3. Identity - Something you are
4. Action - Something you can do
5. Location - Somewhere you are


## Multi-factor methods

### Knowledge-based
"Something you know"
- password
- PIN number
- username
- personal information (eg: "Where were you born? Mother's maiden name? Favorite high school teacher?")

### Biometric
"something you are"
- iris scan - infrared, surface level. quicker than retinal scan & less prone to inaccuracy due to disease 
- fingerprints
- voice scan
- vein scan
- retina scan 
- gait analysis

### Location
- User location, provided by GPS or device sensors 

### Push notifications
"something you have"
- enter a code given to the user by a push notification
- implies the user has possession the mobile device, and ability to open it

### Token / Keyfob
- "something you have" factor
- physical device providing a time-based numeric code
- this is a type of TOTP


### SMS code
- "something you have factor"
- technically  classified as "Out-of-band authentication"
- receive a one-time code by SMS

### HMAC 
- Hash-based message authentication code
- one-time password generator
- increments by counter
- used in authenticator apps or keyfob devices

### TOTP 
- Time-based one-time password
- one-time password generator 
- based on timestamp, expires after set period
- used in authenticator apps or keyfob devices


### Authenticator app
"something you have"
- software application
- generates a rotating time-based  or HMAC numeric code
- examples: Authy, Google Authenticator


### Actions
"something you can do"
- perform a puzzle or challenge (like CAPTCHA)
- match a signature


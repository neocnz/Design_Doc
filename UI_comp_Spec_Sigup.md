# UI Component [SignUp_PhoneNumberVerification] V1.0
### Usage
- Input phone number to create a new account on Select

### UI Elements
- **Actionbar**:
  - Title: Verify your phone number
  - Button: Back
  - Progress indication
- **ContryCodePicker**:
  - Label: +CountryCodeNumber
- **InputField**:
  - Hint: Your Phone Number
  - Input format error indication 
  - Input format correct indication
- **Link**:
  - Label: Terms & Service
- **NextButton**: 
  - Label: Send Confirmation Code
- **Keyboard**: 
  - Number Keyboard
- **ErrorDescription**: 
  - Detailed description

 
### Behaviors 
- **ContryCodePicker {Tap} :**
  - Bring up of the country code list
- **Keyboard_Number {Onload} :**
  - Auto popup
- **NextButton {Onload} :**
  - Display as inactive status (Sim-transparent)
- **NextButton {Tap} :**
  - Display as loading status
  - Finish loading land on next page
- **InputField {Input} :**
  - Conduct the validation check
  - If invalid input detected display the [Input format error indication], and popup the [ErrorDescription] on top of the keyboard
  - If the input is valid display the [Input format correct indication], and the [NextButton] dispaly as active status (Non-transparent)

### Mockups
![SignUp_PhoneNumberVerification](https://www.jianguoyun.com/c/tblv2/CPXHGRIg2N2tW3NteAYafHY2t73lRxhHT8PL99t2D8YbmNa6MwA/lILVfeAJd44/l)


# UI Component [SignUp_VerificationCodeInput] V1.0
### Usage
- Input verification code to verify the phone number

### UI Elements
- **Actionbar**:
  - Title: Enter your verification code
  - Button: Back
  - Progress indication
- **PageDescription**:
  - Text: A SMS verification code just sent to (entered phone number) you can tap back to change it if incorrect
- **InputField**:
  - Four digits input dashes
- **CooldownCounter**:
  - 60 seconds cooldown
- **ResendButton**: 
  - Label: Resend
- **CallButton**: 
  - Label: Call Me
- **NextButton**: 
  - Label: Continue
- **Keyboard**: 
  - Number Keyboard
- **ErrorDescription**: 
  - Detailed description

 
### Behaviors 
- **CooldownCounter {Onload} :**
  - 60 seconds cooldown
  - During cooldown the [Resend] and [Call] button are in inactive status (Sim-transparent)
  - When cooldown finishs the [Resend] and [Call] button are in active status (Non-transparent), and the cooldown counter disappears
- **Resendbutton {Tap} :**
  - Resend the verification code to the same phone number entered previously
  - The cooldown counter starts again from 60
- **Callbutton {Tap} :**
  - Send a voice verification code the same phone number entered previously
  - The cooldown counter starts again from 60 
- **InputField {Input} :**
  - Conduct the validation check
  - Popup the [ErrorDescription] on top of the keyboard
  - If the input is valid the [NextButton] dispaly as active status (Non-transparent)
- **NextButton {Onload} :**
  - Display as inactive status (Sim-transparent)
- **NextButton {Tap} :**
  - Display as loading status
  - Finish loading land on next page
  - If the input verification code is incorrect Popup the [ErrorDescription] on top of the keyboard

### Mockups
[SignUp_VerificationCodeInput](https://www.jianguoyun.com/p/DX6sfmoQpqzHBhiJ1jY)

# UI Component [SignUp_SetIDPassword] V1.0
### Usage
- Set an unique username
- Set a password

### UI Elements
- **Actionbar**:
  - Title: Set your user ID and password
  - Button: Back
  - Progress indication
- **PageDescription**:
  - Text: The SELECT ID is unique in the app and you can not change it after you set it
- **UserIDInputField**:
  - Hint: Your user ID
  - Input format error indication 
  - Input format correct indication
- **PasswordInputField**:
  - Hint: Password
  - Password visibility switch
  - Input format error indication 
  - Input format correct indication
- **NextButton**: 
  - Label: Continue
- **Keyboard**: 
  - Full Keyboard
- **ErrorDescription**: 
  - Detailed description

 
### Behaviors 
- **UserIDInputField {Input} :**
  - Conduct the validation check
  - 3 to 16 numbers or characters
  - If the input is invalid popup the [ErrorDescription] on top of the keyboard
  - If the input in [UserIDInputField] and [PasswordInputField] are valid the [NextButton] dispaly as active status (Non-transparent)
- **PasswordInputField {Input} :**
  - Conduct the validation check
  - 4 to 16 numbers or characters
  - If the input is invalid popup the [ErrorDescription] on top of the keyboard
  - If the input in [UserIDInputField] and [PasswordInputField] are valid the [NextButton] dispaly as active status (Non-transparent) 
- **NextButton {Onload} :**
  - Display as inactive status (Sim-transparent)
- **NextButton {Tap} :**
  - Display as loading status
  - Finish loading land on next page

### Mockups
[SignUp_SetIDPassword](https://www.jianguoyun.com/p/Da9Tcs0QpqzHBhia3TY)


# UI Component [SignUp_RequireAddressbook] V1.0
### Usage
- Give a suggestion to the user to upload the addressbook

### UI Elements
- **Actionbar**:
  - Progress indication
- **PageDescription**:
  - Title: Find Your Friends
  - Text: Need to access to your contacts book to help you find your friends and your info will never be used for other purposes
- **GraphicElements**:
  - Emoji icons to indicate that requiring addressbook upload
- **NextButton**: 
  - Label: Continue
- **SkipButton**: 
  - Label: Nan, I will stay alone

 
### Behaviors 
- **NextButton {Tap} :**
  - Display as loading status
  - Finish loading land on next page
  - Start uploading the addressbook
- **SkipButton {Tap} :**
  - Display as inactive appearance (Sim-transparent)
  - Finish loading land on next page
  - Not uploading the addressbook
  - Popup a dialog box to notice user that can enable addressbook access permission later in settings


### Mockups
[SignUp_RequireAddressbook](https://www.jianguoyun.com/p/Dbd5mgIQpqzHBhim3TY)

# UI Component [SignUp_SetProfile] V1.0
### Usage
- Set profile photo
- Set display username
- Set brithday
- Set gender
- Set email address
- Connect and use facebook profile details

### UI Elements
- **Actionbar**:
  - Title: Set your profile
  - Button: Back
  - Progress indication
- **AvatarPicker**:
- **UserNameInputField**:
  - Hint: Your username
  - Input format error indication 
  - Input format correct indication
- **BirthdayPicker**:
  - Default: 1st/Jan/1970
- **GenderPicker**:
  - Default: Male selected
- **EmailInputField**:
  - Hint: Your email address
  - Input format error indication 
  - Input format correct indication
- **FacebookButton**: 
  - Label: Use Facebook Details
- **NextButton**: 
  - Label: Done
- **Keyboard**: 
  - Full Keyboard
- **ErrorDescription**: 
  - Detailed description

 
### Behaviors 
- **AvatarPicker {Tap} :**
  - Bring up the image picker
- **UsernameInputField {Onload} :**
  - Default: UserID set previously
- **UsernameInputField {Input} :** 
  - Conduct the validation check
  - 1 to 16 any characters
  - If the input is invalid popup the [ErrorDescription] on top of the keyboard
  - If the input in [UsernameInputField] and [BirthdayPicker] and [GenderPicker] are valid the [NextButton] dispaly as active status (Non-transparent) 
- **BirthdayPicker {Tap}**:
  - Brings up the date picker
- **GenderPicker {Tap}**:
  - Display as selected status (Bold underline with a tick icon)
- **EmailInputField {Input}**:
  - Conduct the validation check
  - It is not a required field to proceed to next step
- **FacebookButton {Onload}**: 
  - If the user already connected with Facebook previously this button doesn't display
- **FacebookButton {Tap}**: 
  - Start connect Facebook process
  - Grab the user profile detials from Facebook an fill in to the corresponded user detials field on this page
- **Keyboard {Onload}**: 
  - The keyboard is folded (when the username field or email field is focused the keyboard popups)
- **NextButton {Onload} :**
  - Display as inactive status (Sim-transparent)
- **NextButton {Tap} :**
  - Display as loading status
  - Finish loading land on next page

### Mockups
[SignUp_SetProfile](https://www.jianguoyun.com/p/DZL6jhcQpqzHBhjz3TY)


# [SignUp_Flow] V1.0

### Flow Charts
[SignUp_Flow](https://www.jianguoyun.com/p/DTNZOXgQpqzHBhjd4DY)

[SignUp_Interruption](https://www.jianguoyun.com/p/DVMadPcQpqzHBhje4DY)

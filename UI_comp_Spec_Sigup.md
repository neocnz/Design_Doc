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
  - If the input is valid display the [Input format correct indication], and the [Next Button] dispaly as active status (Non-transparent)

### Mockups
[SignUp_PhoneNumberVerification](https://www.jianguoyun.com/p/DXDBymYQpqzHBhj81TY)


# UI Component [SignUp_VerificationCodeInput] V1.0
### Usage
- Input verification code to verify the phone number

### UI Elements
- **Actionbar**:
  - Title: Enter your verification code
  - Button: Back
  - Progress indication
- **PageDescription**:
  - Text: A SMS verification code just sent to 186 2273 7789 you can tap back to change it if incorrect
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
  - If the input is valid the [Next Button] dispaly as active status (Non-transparent)
- **NextButton {Onload} :**
  - Display as inactive status (Sim-transparent)
- **NextButton {Tap} :**
  - Display as loading status
  - Finish loading land on next page
  - If the input verification code is incorrect Popup the [ErrorDescription] on top of the keyboard

### Mockups
[SignUp_VerificationCodeInput](https://www.jianguoyun.com/p/DX6sfmoQpqzHBhiJ1jY)


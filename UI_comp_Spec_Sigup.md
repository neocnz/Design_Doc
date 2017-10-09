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



# UI Component [MFS] V1.0
### Usage
- Find and select friends faster according to the intention


### UI Elements
- **Actionbar**:
  - Title: Select
  - Button: Cancel
  - Button: Search contact
- **FriendPicker**:
  - GridViewList: 3 columns circle avatar with username beneath
- **SuggestionPickerBar**:
  - A single row of contacts circle avatar with username beneath
- **LocationFilterButton**:
- **ProfileFilterButton**:
- **PreviewBar**:

 
### Behaviors 
- **FriendPicker {Tap} :**
  - Select this friend
  - A selected indicator on the top right of the avatar
  - If there are associated friends popup the [SuggestionPickerBar]
- **SuggestionPickerBar {}:**
  - Tap an avatar select this friend and this avatar disappears
  - Tap the close button on the right end close the picker
  - Tap another friend on [FriendPicker] dismisses this current SuggestionPickerBar
- **LocationFilterButton {Tap} :** 
  - Open the [LocationFilter] page 
- **ProfileFilterButton {Tap} :** 
  - Open the [ProfileFilter] page 
- **PreviewBar {}**:
  - Display the avatars of the selected friends in an row
  - Tap the avatar on the PreviewBar to dis-select a friend
  - Tap the OK button on the right end of the PreviewBar to proceed to next step


# UI Component [MFS_LocationFilter] V1.0
### Usage
- Find friends from certain location


### UI Elements
- **Actionbar**:
  - Title: (Current Location)
  - BackButton: Select
  - SearchButton: Search a location
- **PrivacyStatement**:
  - Text: All locations are approximate
- **Map**:
  - A standard map layer
- **LocalFriendIndicator**: 
  - The number of friends in this location
  - Label: Contacts in the area
  - Button: OK

 
### Behaviors 
- **Map {Drag} :**
  - Move the map to different locations
  - The [PrivacyStatement] and [LocalFriendIndicator] become sim-transparent
  - The friends number on the [LocalFriendIndicator] updates according to how many friends in this location
- **Map {Pinch}:**
  - Pinch in: zoom out the map
  - Pinch out: zoom in the map
  - The [PrivacyStatement] and [LocalFriendIndicator] become sim-transparent
  - The friends number on the [LocalFriendIndicator] updates according to how many friends in this location
- **LocationSearch_OK {Tap} :** 
  - Proceed to next step


# UI Component [MFS_ProfileFilter] V1.0
### Usage
- Find friends from certain profile settings


### UI Elements
- **DialogWindow**:
- **GenderSelector**:
  - All: Select all genders
  - Male: Select male gender
  - Female: Select female gender
- **AgePicker**:
  - A two nobe slider
- **SetButton**: 
  - Label: Set
- **ResetButton**: 
  - Label: Reset

 
### Behaviors 
- **GenderSelector {Tap} :**
  - Select the tapped gender
  - The selected gender option is highlighted as selected status
  - The [All] gender is picked by default
- **AgePicker {Slide}:**
  - Left nobe to right set the minimum age
  - Right nobe to left set the maximun age
  - When tap on a nobe popup a number indicator
  - The default age rang is 16 - 25
- **Set {Tap} :** 
  - Start filtering with current condition
- **Reset {Tap} :** 
  - Clear current condition settings 

### Mockups
[MFS](https://drive.google.com/drive/folders/0ByrgX886wsYdN05PeXpiV245NHM?usp=sharing)

# UI Component [ImagePicker] V1.0
### Usage:
- Browse images on local device from different folders
- Search static images / gif moving images from Internet
- Pick images from the list and preivews of selected images
- Enlarge to view an image

### UI Elements
- **Actionbar**:
  - Button: Cancel
  - Button: Done
  - Dropdown: Image folders
- **Grid List View**: 
  - Three column grid list with square cells display from top down in an reversed chronological order
  - Button: Camera **(display on the first cell)**
  - Button: Web image search **(display on the second cell)**

### Behaviors 
- **Actionbar_Cancel {Tap}** : 
  - Dismiss image picker / go back to previous page
- **Actionbar_Done {Tap}** : 
  - Proceed the next step with picked images
  - At less one image been selected it appears as active status
- **Actionbar_ImageFolders {Tap}** : 
  - List of the image folders on the local device, select a folder will reload the grid cells with the images from the selected folder
  - On the dropdwon list, the folder names display on the left side and the number of the image in that folder displays on the right side of the list 
  - The selected folder name will be displayed on the dropdown button
- **GridListView_List {Scroll}** : 
  - Scroll only vertically 
- **GridListView_Cell {Tap}** : 
  - Tap to select the image in cell 
  - When selected has a sim-tranparent overlay with a number of the select sequence on it
  - When tap again the selected cell deselect the cell
  - The max number of the image can be picked in one go is 10
  - **[On Error]** when selecting an image exceeded the selection limit, popup a dialog box to notice the user
- **GridListView_Cell {LongPress}** : 
  - Enter the **[[ImageEnlargeView]](https://hackmd.io/BwFgZgRgTAjAnFAtDCBjArIkA2HiHoAmiqAzHBMHAKaEAMMA7NUA) (Altered)**
- **GridListView_Camera {Tap}** : 
  - Open the device camera
- **GridListView_WebImageSearch {Tap}** : 
  - Enter the **[[WebImageSearch]](https://hackmd.io/OwUwhsCMBMAsCcBaAJgYwKxkbAZugDImOuiIvMPtAMzrLrUBsj0QA===)** 

### Integrated Components:
- **[ImageEnlargeView] (Altered)** : 
  
  **Add UI Elements**
  - **Actionbar:**
    - Button: back
    - Checkbox: pick
  
  **Add Behavior**
  - **ImageLargeView_Actionbar_TickBox {Tap}** : 
    - Tap the CheckBox to select current image
    - When the selected images are more than 10 the TickBox will be appears as inactived status


### Wireframes:
[Image Picker Main](https://www.jianguoyun.com/p/DdiTSAoQpqzHBhiO-zU)

[Enlarge Image View](https://www.jianguoyun.com/p/DS350rwQpqzHBhiP-zU)

[Image Folders Dropdown](https://www.jianguoyun.com/p/DcpFivUQpqzHBhiQ-zU)

[Web Image Search](https://www.jianguoyun.com/p/DZdVuLUQpqzHBhiJ-zU)

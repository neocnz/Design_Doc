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
  - Tap to select the cell 
  - When selected has a sim-tranparent overlay with a number of the select sequence on it
  - When tap again the selected cell deselect the cell
  - The max number of the image can be picked in one go is 10
- **GridListView_Cell {LongPress}** : 
  - Enter the **[[ImageEnlargeView]](https://hackmd.io/BwFgZgRgTAjAnFAtDCBjArIkA2HiHoAmiqAzHBMHAKaEAMMA7NUA) (Altered)**
- **GridListView_Camera {Tap}** : 
  - Open the device camera
- **GridListView_WebImageSearch {Tap}** : 
  - Enter the **[[WebImageSearch]](https://hackmd.io/OwUwhsCMBMAsCcBaAJgYwKxkbAZugDImOuiIvMPtAMzrLrUBsj0QA===)** 

### Integrated Components:
- **[ImageEnlargeView] (Altered)** : 
  **Remove Behavior**
  - **ImageLargeView_ImageCounterIndicator (Highlight)** : 
    - the image counter indicator of the in view image will be highlight

  **Add Behavior**
  - **ImageLargeView_Actionbar_TickBox {Tap}** :
    - Tap the TickBox the select current image
    - When the selected images are more than 10 the TickBox will be appears as inactived status
    
### Wireframes:
**[Image Picker Main](https://share.weiyun.com/050a0fc50b878e7982152c7f430fc6d1)**

**[Enlarge Image View](https://share.weiyun.com/e5f7e9fa8d86f0eae170fd579a8ef487)**

**[Image Folders Dropdown](https://share.weiyun.com/fb13c4faf33a84eac999edfd3c33c9ed)**

**[Web Image Search](https://share.weiyun.com/de3eac61c20b03c85816aadb75b73abc)**

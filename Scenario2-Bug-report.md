# DICOM Images Not Displayed During Landmark Editing in Knee App

## Steps to Reproduce:

### 1. Import a Knee Case:
- Launch the Knee App.
- Navigate to the "Import Case" section.
- Select a knee case file that includes a pre-plan.
- Import the case.

### 2. Open the Imported Case:
- Locate the imported case in the case list.
- Click on the case to open it.

### 3. Navigate to Manage Case:
- Touch the "Manage Case" button.

### 4. Access the Plan Section:
- In the "Manage Case" interface, select the "Plan" section.

### 5. Access the Landmark Section:
- In the "Plan" section, select the "Landmark" section.

### 6. Verify Image Display:
- Check if DICOM images are displayed alongside segmented images in the "Landmark" section.

### 7. Attempt to Edit DMA Point:
- Select the DMA point and attempt to edit its position.

## Expected Results:

### DICOM and Segmented Images Display:
- All relevant images (DICOM and segmented) should be visible in the "Landmark" section, allowing the user to accurately position the DMA point.

### DMA Point Editing:
- The user should be able to see the DMA point on the DICOM images, adjust its location, and save the changes. The updated position should be reflected in the 2D images, 3D model, and pre-planning data.

## Actual Results:
- **Failure:** DICOM images do not appear in the "Landmark" section during the DMA point editing process. Only segmented images are displayed, making it difficult to accurately position the landmark.


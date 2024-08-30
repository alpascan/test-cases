
# Test Case: Knee App - Import and Manage Knee Case with Pre-Plan

## Step 1: Import Knee Case

**Objective:** Import a knee case with a pre-plan on the navigation station.

### Procedure:
1. Launch the Knee App.
2. Navigate to the "Import Case" section.
3. Select the knee case file that includes a pre-plan.
4. Import the case.

### Expected Result:
- The case is successfully imported into the Knee App.

### Pass/Fail:
- **Result:** Pass

---

## Step 2: Open Imported Case

**Objective:** Open the previously imported knee case.

### Procedure:
1. Locate the imported case in the case list.
2. Click on the case to open it.

### Expected Result:
- The imported case opens successfully in the Knee App.

### Pass/Fail:
- **Result:** Pass

---

## Step 3: Manage Case Navigation

**Objective:** Access the "Manage Case" functionality for the imported case.

### Procedure:
1. With the case open, touch the "Manage Case" button.

### Expected Result:
- The "Manage Case" interface is displayed.

### Pass/Fail:
- **Result:** Pass

---

## Step 4: Access Plan Section

**Objective:** Navigate to the "Plan" section within the case.

### Procedure:
1. In the "Manage Case" interface, select the "Plan" section.

### Expected Result:
- The "Plan" section is displayed, showing the existing pre-plan.

### Pass/Fail:
- **Result:** Pass

---

## Step 5: Access Landmark Section

**Objective:** Navigate to the "Landmark" section to view and edit landmarks.

### Procedure:
1. In the "Plan" section, select the "Landmark" section.

### Expected Result:
- The "Landmark" section is displayed, showing the current landmarks.

### Pass/Fail:
- **Result:** Pass

---

## Step 6: Verify DICOM and Segmented Image Display

**Objective:** Ensure that DICOM and segmented images are displayed correctly in the Landmark section.

### Procedure:
1. In the "Landmark" section, verify that both DICOM and segmented images are displayed.
2. Confirm that the DMA point is visible on the images.

### Expected Result:
- All associated images (DICOM and segmented) are displayed correctly in the Landmark section.

### Pass/Fail:
- **Result:** Fail
- **Comments:** DICOM images are not displayed.

---

## Step 7: Edit and Save DMA Point

**Objective:** Edit the DMA point location and save the changes.

### Procedure:
1. Select the DMA point in the Landmark section.
2. Manually adjust the location of the DMA point.
3. Save the changes.

### Expected Result:
- The DMA point is edited and saved successfully.
- The updated landmark is reflected on both 2D images and the 3D model.

### Pass/Fail:
- **Result:** Pass

---

## Step 8: Verify Plan Update with Edited Landmark

**Objective:** Ensure that the pre-plan is updated with the new DMA point position.

### Procedure:
1. Return to the "Plan" section after editing the DMA point.
2. Verify that the pre-plan reflects the new position of the DMA point.

### Expected Result:
- The existing pre-plan is updated with the new DMA point position.
- The 2D images, 3D model, and plan data all reflect the updated landmark.

### Pass/Fail:
- **Result:** Pass

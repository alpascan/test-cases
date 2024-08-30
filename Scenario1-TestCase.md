# Expanded Test Procedure for Knee App Soft Tissue Acquisition

## 1. Setup

### 1.1. Knee App Installation

- Verify app version and build number
- Check for any pending updates or patches

### 1.2. Test Environment Preparation

- Set up tracking cameras and ensure calibration
- Prepare all necessary instruments and markers

### 1.3. Test Subject/Model Preparation

- **If using a model:**
  - Ensure accurate simulation of different flexion angles
  - Verify capability to simulate various stresses

- **If using a test subject:**
  - Brief the subject on the procedure
  - Ensure subject comfort throughout testing

## 2. Workflow Testing

### 2.1. Flexion Test

#### a. Knee Positioning

- Test at 80°
- Test at 90°
- Test at 100°
- Test at 85° (mid-range)
- Test at 95° (mid-range)

#### b. Medial Stress Application

- Verify capture initiation
- Ensure continuous data recording during stress
- Check capture cessation upon stress release

#### c. Lateral Stress Application

- Repeat all steps from medial stress test

#### d. Data Storage Verification

- Check completeness of data structure
- Verify accuracy of timestamps

### 2.2. Extension Test

#### a. Knee Positioning

- Test at -20°
- Test at 0°
- Test at 15°
- Test at 30°
- Test at -10° (mid-range)
- Test at 22° (mid-range)

#### b. Medial Stress Application

- Verify capture initiation
- Ensure continuous data recording during stress
- Check capture cessation upon stress release

#### c. Lateral Stress Application

- Repeat all steps from medial stress test

#### d. Data Storage Verification

- Check completeness of data structure
- Verify accuracy of timestamps

## 3. UI Testing

### 3.1. Context Display

- Verify clear indication of flexion/extension state
- Ensure clear display of varus/valgus stress direction
- Test knee flexion angle display:
  - Verify accuracy within ±1° at various angles
  - Check real-time update frequency

- Test varus/valgus angle display in extension:
  - Verify accuracy within ±0.5° at various angles
  - Check real-time update frequency

### 3.2. Registration Notification

- **Test notification visibility:**
  - Verify prominent screen display
  - Check for audible alert

- **Test notification timing:**
  - Ensure immediate appearance after successful registration

- **Test notification dismissal:**
  - Verify user can acknowledge or dismiss

### 3.3. Repeat Registration

- Test repeat option visibility after each registration
- Verify proper overwrite of previous data
- Ensure correct storage of new data

## 4. Flexibility Testing

### 4.1. Tensioning Technique

#### a. Manual Knee Tensioning

- Test with light manual stress
- Test with moderate manual stress
- Test with firm manual stress
- Verify consistent capture across different users

#### b. Instrument-Assisted Knee Tensioning

- Test with various tensioning instruments
- Verify calibration process for each instrument
- Test capture at 10 lbs tension
- Test capture at 20 lbs tension
- Test capture at 30 lbs tension

### 4.2. Registration Stages

- **Test post-anatomy registration:**
  - Verify availability of soft tissue registration option
  - Test transition from anatomy to soft tissue registration

- **Test post-tibial resection:**
  - Ensure recognition of tibial resection
  - Verify any tracking or measurement adjustments

- **Test with trial implants:**
  - Verify recognition of trial implant placement
  - Check for appropriate measurement/calibration adjustments

- **Test with final implant:**
  - Verify recognition of final implant placement
  - Test final soft tissue balance evaluation

## 5. Wrong Acquisition Detection

### 5.1. Incorrect Stress Application

- **Test valgus stress when varus requested:**
  - Apply varying degrees of incorrect stress
  - Verify rejection threshold sensitivity

- **Test varus stress when valgus requested:**
  - Apply varying degrees of incorrect stress
  - Verify rejection threshold sensitivity

### 5.2. Out-of-Range Angle

- **Flexion test:**
  - Test at 79°
  - Test at 78°
  - Test at 101°
  - Test at 102°

- **Extension test:**
  - Test at -21°
  - Test at -22°
  - Test at 31°
  - Test at 32°

- Verify rejection and appropriate error messages for all out-of-range angles

### 5.3. Rejection Notification

- Verify clarity of rejection reason in notification
- Ensure clear guidance for correct action is provided
- Test ease of initiating repeat acquisition
- Verify that incorrect data is not stored

## 6. Edge Cases and Error Handling

### 6.1. Interrupted Capture

- Simulate brief tracking loss
- Test with longer duration tracking loss
- Simulate sudden patient movement during capture
- Test with various movement speeds and magnitudes

- **Verify error recovery:**
  - Check clarity of error messages
  - Test auto-recovery options
  - Test manual intervention procedures

### 6.2. Data Consistency

- Perform 10 consecutive captures for each test condition
- Analyze data for consistency and identify outliers
- Verify data integrity after app restart
- Check data accuracy after system sleep/wake cycles

### 6.3. Performance Under Load

- Perform 50 captures in quick succession
- Monitor for performance or accuracy degradation
- Run app continuously for 4 hours with regular captures
- Check for memory leaks or performance issues

## 7. Usability Testing

### 7.1. User Guidance

- **Test with novice users:**
  - Observe unaided navigation through workflow
  - Collect feedback on instructions and UI clarity

- **Test with experienced users:**
  - Time performance through workflow
  - Gather optimization suggestions

### 7.2. Visual Feedback

- Test in bright OR lighting conditions
- Check visibility in dimmed lighting
- Verify UI clarity for users with color vision deficiencies

## 8. Integration Testing

### 8.1. Data Flow

- Verify soft tissue data influence on implant positioning recommendations
- Check accuracy of soft tissue balance data in final reports
- Test data export in various formats (CSV, PDF)

### 8.2. Compatibility

- Test with all supported tracking systems
- Verify functionality with different display types
- Test integration with other TKA suite modules
- Verify compatibility across different OS versions

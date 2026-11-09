
# GIT 337 — Inclusive Form Flow Test Record

## Project
Mobile Auto Detailing Service Request

## Purpose
Test the usability, accessibility, validation, and responsive design of a fictional mobile auto detailing service request form.

The prototype uses HTML and CSS only. It does not collect or send real customer information.

## HTML and CSS Validation

- HTML: PASS — No errors or warnings.
- CSS: PASS — No errors found.
- HTML issue corrected: Removed the empty action attribute from the form.

Evidence:
- evidence/17-html-validation.png
- evidence/18-css-validation.png

## Form Validation Tests

| Test | Result | Evidence |
|---|---|---|
| Submit with required fields empty | PASS — Browser identifies missing information | 01-empty-submit.png |
| Enter malformed email | PASS — Browser requests a valid email format | 02-invalid-email.png |
| Leave service area unselected | PASS — Selection required | 03-required-service-area.png |
| Leave detailing service unselected | PASS — Radio selection required | 04-required-detailing-service.png |
| Leave vehicle type unselected | PASS — Selection required | 05-required-vehicle.png |
| Leave appointment date empty | PASS — Date required | 06-required-appointment-date.png |
| Complete form using fictional values | PASS — Native validation accepted entries | 07-valid-form.png |
| Leave optional fields empty | PASS — Optional fields do not block submission | 08-optional-fields.png |

## Fictional Test Information

- Email: student@example.com
- Service area: Baltimore County
- Detailing service: Full Detail
- Vehicle type: SUV
- Preferred date: November 16, 2026
- Preferred time: 10:22 AM
- Vehicle condition: Moderate cleaning
- Add-on: Clay Bar Treatment
- Parking: Driveway
- Instructions: Please clean the seats and floor mats.

All information was fictional and used for classroom testing.

## Keyboard and Focus Testing

- Keyboard focus indicator was visible.
- Radio buttons displayed a clear focus state.
- Required fields used native browser validation.

Evidence:
- evidence/09-keyboard-focus.png
- evidence/10-keyboard-radio-focus.png

## Responsive Layout Testing

| Viewport | Observation | Evidence |
|---|---|---|
| 320px | Visible form controls fit and text wrapped without overlap | 11-mobile-320-form.png |
| 320px | Submit area and static error example were inspected | 12-mobile-320-submit.png, 13-mobile-320-error.png |
| Tablet | Visible controls remained readable; confirm exact 768px width | 14-tablet-768.png |
| 1280px | Visible form controls fit without overlap | 15-desktop-1280.png |
| Enlarged browser zoom | Visible text, textarea, and submit button remained usable; exact 200% setting needs confirmation | 16-zoom-200.png |

## State and Recovery Evidence

- Default: Controls begin without entered information.
- Focus: A visible gold outline identifies keyboard focus.
- Required: Native HTML constraints prevent incomplete submission.
- Valid: Required fields accept correctly formatted entries.
- Invalid: Native browser messages explain missing or malformed entries.
- Disabled: A disabled example button is shown in F5.
- Static server-returned error: A fictional email error example includes an error summary, affected field, and correction instructions.

## Additional Verification Required

- Confirm the tablet test at exactly 768px.
- Confirm browser zoom was exactly 200%.
- Inspect accessible names and groups for email, select, radio, checkbox, and textarea controls.
- Confirm keyboard-only completion of the full form.

## Test Conclusion

HTML and CSS validation passed. The screenshots document native validation, focus visibility, and responsive behavior in the inspected sections. Remaining checks must be completed before final submission.

## Additional Test Results

- 240-character limit: PASS — Additional characters were blocked after reaching the maximum.
- Evidence: evidence/21-character-limit.png
- Keyboard-only navigation: PASS — Tab and Shift+Tab moved between fields.
- Radio buttons: PASS — Arrow keys changed selections.
- Checkboxes: PASS — Space selected and deselected options.
- Keyboard submission: PASS — The form was completed and submitted without a mouse.
- Evidence: evidence/09-10-keyboard-navigation.png
- Accessibility inspection: PASS — Email, radio buttons, checkboxes, textarea, and service area dropdown have meaningful accessible names and appropriate roles.
- Evidence: evidence/23-email-accessibility.png
- Evidence: evidence/24-radio-accessibility.png
- Evidence: evidence/25-checkbox-accessibility.png
- Evidence: evidence/26-textarea-accessibility.png
- Evidence: evidence/27-service-area-accessibility.png
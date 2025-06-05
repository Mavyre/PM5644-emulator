## Description

This project contains a web page that displays the PM5644 test pattern as a background image. The PM5644 is a classic television test pattern that was commonly used for calibrating and testing television equipment.

## Files

- **index.html**: The main HTML document that displays the PM5644 test pattern
- **PM5644.svg**: SVG version of the PM5644 test pattern used as background image

### URL Parameters

You can customize the display by adding URL parameters:

#### Top Bar Parameters

- **`tbar`**: Displays a single line of text in the top bar (large format)
  ```
  index.html?tbar=STATION%20ID
  ```

- **`tbar1`** and **`tbar2`**: Displays two lines of text in the top bar (small format)
  ```
  index.html?tbar1=LINE%201&tbar2=LINE%202
  ```

#### Bottom Bar Parameters

- **`bbar`**: Displays text in the bottom-right corner
  ```
  index.html?bbar=BOTTOM%20TEXT
  ```

- **`bbarfull`**: Displays text across the full bottom bar
  ```
  index.html?bbarfull=FULL%20WIDTH%20BOTTOM%20TEXT
  ```

### Special Values

Some parameters accept special values for dynamic content:

- **`TIME`**: Displays current time (HH:MM:SS format, updates every second)
  ```
  index.html?tbar=TIME
  ```

- **`DATE`**: Displays current date (DAY DD MON format, e.g., "WED 05 JUN")
  ```
  index.html?tbar1=TIME&tbar2=DATE
  ```

### Example Combinations

1. **Station identification with time:**
   ```
   index.html?tbar1=STATION%20XYZ&tbar2=TIME&bbar=TEST
   ```

2. **Full bottom bar with datetime:**
   ```
   index.html?tbar1=DATE&tbar2=TIME&bbarfull=TEST%20SIGNAL
   ```

3. **Custom text overlay:**
   ```
   index.html?tbar=TEST&bbar=CALIBRATE
   ```

## Technical Details

- The project uses pure HTML and CSS
- The SVG image is referenced as a background image in the CSS
- No additional dependencies or build steps required

This can be used as a file in a browser source in OBS studio.

## Browser Compatibility

This project should work in all modern web browsers that support:
- HTML5
- CSS3
- SVG images

## Development

To modify or extend this project:

1. Edit `index.html` to change the layout or styling
2. Replace `PM5644.svg` with a different test pattern if needed
3. Open the file in a browser to preview changes

No build process or server setup is required for development.
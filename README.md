# ND Filter & Exposure Calculator

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

A comprehensive web-based calculator for photographers working with neutral density (ND) filters. This tool helps you calculate the correct exposure settings when using ND filters, taking into account changes in aperture and ISO for perfect long exposure photography.

![Demo](assets/DEMO.gif)

## Features

###  ND Filter Calculator
- **Exposure Triangle Calculation**: Automatically calculates new shutter speed based on ND filter strength, aperture, and ISO changes
- **User-Friendly Inputs**: Accept shutter speeds in multiple formats (1/125, 2, 0.5)
- **ND Filter Range**: Support for ND filters from 0 to 20 stops (up to ND1M)
- **Real-Time Breakdown**: See exactly how each change (ND filter, aperture, ISO) contributes to total exposure compensation
- **Visual Feedback**: Brightness comparison and scale bar showing filter strength
- **Light Reduction Display**: Shows percentage of light blocked by the selected ND filter

###  Exposure Timer
- **Dual Mode**: Switch between countdown timer and stopwatch
- **Precision Timing**: Down to deciseconds (0.1s) accuracy
- **Quick Transfer**: One-click button to use calculated shutter speed
- **Audio & Haptic Feedback**: Optional sound alerts and vibration on completion
- **Custom Duration**: Set any exposure time manually

###  Bulb Mode Helper
- **Countdown**: 3-2-1 audio countdown before opening shutter
- **Millisecond Display**: Shows precise exposure time in milliseconds
- **Auto Alert**: Automatic alert when it's time to close the shutter
- **Audio Beeps**: Different tones for countdown and shutter close

###  Save & Load Presets
- **Custom Presets**: Save your favorite camera/lens combinations
- **Named Configurations**: Give each preset a descriptive name
- **Quick Load**: Instantly load saved settings
- **Persistent Storage**: Presets saved in browser localStorage
- **Reset Function**: One-click reset to default settings

## How It Works

The calculator uses the **Exposure Triangle** principle to maintain correct exposure:

Total Compensation = ND Filter Stops + Aperture Change + ISO Change

New Shutter Speed = Original Shutter × 2^(Total Compensation)

### Calculation Examples

**Example 1: Basic ND Filter**
- Original: 1/125s, f/5.6, ISO 100
- Add: ND64 (6 stops)
- Result: 0.5s (6 stops slower)

**Example 2: ND Filter + Aperture Change**
- Original: 1/125s, f/2.8, ISO 100
- Add: ND64 (6 stops) + change to f/11
- Result: 8s (6 + 4 = 10 stops total)

**Example 3: All Three Variables**
- Original: 1/125s, f/5.6, ISO 200
- Add: ND64 (6 stops) + f/16 + ISO 100
- Result: 8s (6 + 3 + 1 = 10 stops total)

## Usage

1. **Enter Current Settings**
   - Input your current shutter speed (supports formats like 1/125, 2, or 0.5)
   - Set your current aperture (f-stop)
   - Set your current ISO

2. **Add ND Filter & Adjust**
   - Select the ND filter strength (0-20 stops)
   - Optionally change aperture for desired depth of field
   - Optionally change ISO for desired noise level

3. **Get Results**
   - See the new required shutter speed
   - Review the compensation breakdown
   - Check light reduction percentage

4. **Use Timer (Optional)**
   - Click "Use Calculated Shutter Speed" to transfer the result to timer
   - Start the countdown or stopwatch
   - Use Bulb Mode Helper for long exposures with audio cues

5. **Save Your Setup (Optional)**
   - Name your current configuration
   - Click "Save Current" to store it
   - Load anytime with one click

## Technical Details

- **Pure HTML/CSS/JavaScript**: No dependencies, works offline
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Browser Compatibility**: Modern browsers (Chrome, Firefox, Safari, Edge)
- **Local Storage**: Presets saved locally in your browser
- **Dark Theme**: Eye-friendly interface for field use

## Photography Use Cases

- **Waterfalls**: ND1000 (10 stops) for silky smooth water
- **Sea Waves**: ND64 (6 stops) for dreamy ocean motion
- **Cloud Motion**: ND256 (8 stops) for dramatic sky streaks
- **Daytime Portraits**: ND8 (3 stops) for wide aperture in bright light
- **Cityscape**: ND16 (4 stops) for removing people from busy streets

## Installation

1. Clone this repository:git clone https://github.com/yourusername/ND-Filter-Exposure-Calculator.git
2. Open `index.html` in your web browser

That's it! No build process or installation required.

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Opera 76+

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## License

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

**You are free to:**
- Share — copy and redistribute the material
- Adapt — remix, transform, and build upon the material

**Under the following terms:**
- Attribution — You must give appropriate credit
- NonCommercial — You may not use the material for commercial purposes
- ShareAlike — If you remix, transform, or build upon the material, you must distribute your contributions under the same license

## Acknowledgments

Built for photographers who love long exposure photography and need precise exposure calculations in the field.

## Author

Created by mahmood MOHAMMED ALI

**Star ⭐ this repo if you find it useful!**

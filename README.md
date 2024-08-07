# DALL-E 2 Batch Downloader

This Tampermonkey script allows you to batch download your personal DALL-E 2 generated images from the OpenAI labs website. It includes features for resuming downloads, setting manual start points, and displaying image indices.

## Features

- Batch download DALL-E 2 images from your personal gallery
- Resume functionality to continue downloads from where you left off
- Manual index setting to start downloads from a specific image
- Display of image indices in the gallery for easy reference
- Configurable delay between downloads to avoid overwhelming the server

## Installation

1. Install the [Tampermonkey](https://www.tampermonkey.net/) browser extension for your browser.
2. Create a new script in Tampermonkey and paste the contents of `dalle-image-downloader.user.js` into it.
3. Save the script and ensure it's enabled in Tampermonkey.

## Usage

1. Navigate to your DALL-E 2 gallery page on the OpenAI labs website. Make sure to load all images on the page by scrolling all the way to the bottom.
2. You'll see new buttons and an input field in the top-right corner of the page:
   - **Start Download**: Begins downloading from the start of your gallery
   - **Stop Download**: Pauses the download process
   - **Resume Download**: Continues downloading from where you left off
   - **Reset Progress**: Clears saved progress
   - **Set Index** (with input field): Allows you to set a specific starting point
3. Each image in the gallery will now display its index number in the bottom-left corner.
4. Use the buttons to control the download process as needed.

## Important Browser Settings

To ensure smooth operation and avoid constant download prompts, you need to configure your browser settings. This is crucial for the script to work efficiently.

### Chrome

1. Go to Settings > Advanced > Downloads
2. Toggle ON "Ask where to save each file before downloading"
3. Set your preferred download location

### Firefox

1. Go to Options > General > Downloads
2. Check "Save files to" and choose your preferred download location
3. Uncheck "Always ask you where to save files"

### Edge

1. Go to Settings > Downloads
2. Toggle OFF "Ask me what to do with each download"
3. Set your preferred download location under "Save As" location

**Note**: Ensuring these settings are correctly configured is vital for the script to function without requiring manual intervention for each download.

## Customization

You can modify the following variables in the script to customize its behavior:

- `sleep(1000)`: Adjust the number to change the delay between downloads (in milliseconds)

## Troubleshooting

- If downloads aren't starting, check your browser's download settings as described above.
- Ensure you're logged into your OpenAI account and on the correct gallery page.
- If images aren't displaying indices, try refreshing the page.

## Disclaimer

This script is for personal use only. Ensure you comply with OpenAI's terms of service when using this script. The authors are not responsible for any misuse or violation of terms.


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Credits

The whole script and all text on this readme are written by Claude 3.5 Sonnet

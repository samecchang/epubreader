# ePub Reader

> **Read your favorite eBooks instantly with this powerful single-page ePub tool.**

## The Backstory
This project traces back to my time at **Microsoft Headquarters** just before the launch of **Windows 8**. I was tasked with writing sample applications to showcase the potential of building native-feeling apps using pure web technologies. 

One of my prototypes was an ePub reader. Although that specific project was never published at the time, I have rebuilt it here from the ground up. This modern version is a streamlined, single-page utility that brings that original vision to life—allowing anyone to read eBooks directly in their browser with no installation required.

## Features
*   **Zero Installation:** A standalone HTML file that works entirely in your browser.
*   **Smooth Navigation:** Includes a simple "page-flip" style transition for a more tactile reading experience.
*   **Customizable Viewing:** Easily adjust the font size to suit your reading preference.
*   **Privacy-Focused:** Your files are processed locally on your machine; nothing is ever uploaded to a server.

## How to Use
1.  **Open** the `ePubReader.html` file in any modern web browser.
2.  **Upload** your desired `.epub` file using the file picker.
3.  **Read** and enjoy! Use the on-screen buttons or arrow keys to turn pages.
4.  **Adjust** the text size using the controls in the header.

## Technical Details
This tool leverages the powerful [epub.js](https://github.com/futurepress/epub.js/) library for parsing and rendering, combined with [JSZip](https://stuk.github.io) to handle compressed ePub containers.

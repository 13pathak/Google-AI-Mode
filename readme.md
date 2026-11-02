# **Google AI Focused Window (Deprecating)**

A browser extension that opens Google's AI Search Mode in a dedicated popup window using a keyboard shortcut. The window closes when you switch to another browser window.

## **Features**

* **🚀 Keyboard Shortcut:** Press Ctrl+Shift+K (or Cmd+Shift+K on Mac) to open the search prompt. Change the shortcut at `chrome://extensions/shortcuts`.
* **✨ Focused Window:** Your search query opens in a clean, separate popup window, free from the clutter of a normal browser tab.  
* **🧠 Auto-Close:** The focused window closes when another browser window gains focus.  
* **🎨 Clean Layout:** Custom CSS adjusts the Google Search page for the smaller window.

## **Installation**

Since this is not on the Chrome Web Store, you can load it directly into your browser:

1. **Download:** Download this project's files, preferably as a ZIP, and unzip them to a folder on your computer.  
2. **Prepare the Icons:** Rename the included `icons` folder to `images` in your downloaded copy. The current `manifest.json` references `images/icon16.png`, `images/icon48.png`, and `images/icon128.png`.  
3. **Open Extensions:** Open your Chromium-based browser and visit its extensions page (`chrome://extensions` in Chrome or `edge://extensions` in Edge).  
4. **Enable Developer Mode:** In the top-right corner of the extensions page, toggle on "Developer mode".  
5. **Load the Extension:** Click the "Load unpacked" button that appears.  
6. **Select Folder:** In the file dialog, navigate to and select the folder where you unzipped the project files.  
7. **Done!** The "Google AI Focused Window" extension should now appear in your list of extensions and be ready to use.

## **How to Use**

1. On any webpage, press the keyboard shortcut: Ctrl+Shift+K (or Cmd+Shift+K on Mac).  
2. A small search box will appear. Type your question and press Enter.  
3. The Google AI Search results will open in a new, focused window.  
4. When you are finished, simply click back to your main browser window, and the focused window will automatically disappear.

## **File Structure**

* manifest.json: The core file that defines the extension's permissions, features, and file references.  
* background.js: The service worker that creates, updates, and closes the focused window.  
* popup.html / popup.css / popup.js: These files create the small initial search box that appears when you use the keyboard shortcut.  
* injector.css: Styles injected into the Google Search page to adjust the smaller window's layout.  
* icons/: Contains the extension icons. Rename this folder to `images` before loading the current manifest, as described above.

## **Contributing**

This was a personal project, but feel free to fork this repository, suggest improvements, or open an issue if you find any bugs!

# Custom Workflow: "把這張圖改成傳統"

Whenever the user says **"把這張圖改成傳統"** and provides an image or text:

### 1. Browser Setup
*   Open Google Gemini in the browser.
*   Locate and click the **"傳統玻璃生成"** Gem in the sidebar.
*   Switch the model to **"Pro"**.

### 2. Execution
*   Upload the user's provided image.
*   Paste the user's text prompt into the chatbox.
*   Click send and wait for completion.

### 3. File Management
*   Download the generated result.
*   Save the file to `/home/yorknty_natalie/clawd/Project/ImageTracker/Images/`.
*   Send the image back to the user on Telegram immediately.

### 4. Cloud Backup
*   Upload the image to Google Drive (folder: `image tracker`).

### 5. Tracker Hierarchy
*   **Case A (New Root)**: If the request is independent, add a new **root** entry to `Project/ImageTracker/tracker_data.js`.
*   **Case B (Extension)**: If the user **replies** to a previous image from the tracker, find that node by its ID and add the new image as a **child** of that node in `tracker_data.js`.

### 6. Deployment
*   Commit and push updated `tracker_data.js` to GitHub so the **Image Tracker** website reflects the change.

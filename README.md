# Mark all Canvas Announcements as Read

Easy way to automatically mark all course announcements on Canvas as read, instead of doing them manually one by one.

Users of Instructure's [Canvas LMS](https://www.instructure.com/canvas/) have [asked a lot](https://community.canvaslms.com/t5/Idea-Conversations/Marking-all-announcements-read/idi-p/351918) for the ability to quickly mark all course announcements as read. As of 24 Dec 2020, this capability still doesn't seem to be implemented in the web or mobile app GUIs, but is available through v1 of the Canvas REST API. This Python script facilitates this action.

## Configuration

You need a Canvas LMS token to run this script.

1. Log into the Canvas web app using your institution's domain (i.e., `https://umich.instructure.com`) and make a note of this `.instructure.com` URL.
2. Under **Account** > **Settings** > **Approved Integrations**, choose to generate a new access token. Take note of this token (a long string of letters, numbers, and symbols) because you can't see it again once you leave that screen.
3. Clone this repo to your local computer.
4. Change the `TOKEN` variable in the script to equal the generated access token from step 2.
5. Change the `MY_DOMAIN` variable in the script to match your institution's Canvas URL (e.g., `https://umich.instructure.com` for University of Michigan).

## Usage

Install the required packages using `pip install -r requirements.txt` and run the script using Python, 3.6 or higher.

Then just run the script directly. No command-line arguments are needed.

```
# On Linux/macOS/BSD
cd <repo folder>
python3 ./mark-canvas-announcements-as-read.py

# Or on Windows
cd <repo folder>
python ./mark-canvas-announcements-as-read.py
```

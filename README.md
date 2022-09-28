# WhatsApp Chat Analyser
Have you ever wondered whether your groupchat is dying? Or maybe someone in it talks way too much and you just want to prove it to them? Or perhaps, somebody uses a certain word way too often? Look no further.

This tool parses WhatsApp transcripts and generates pretty graphs using matplotlib and seaborn. The images are written to the out/ directory, and can be displayed together by opening html/index.html.

## Requirements
This tool was built using Python 3.10; unexpected behaviour may occur when using earlier versions. There are also a few external libraries. Thankfully, all can be installed using pip.

In the command line, type `pip install -r requirements.txt`

Alternatively, the required libraries can be installed individually
matplotlib: `pip install matplotlib`
numpy: `pip install numpy`
pandas: `pip install pandas`
seaborn: `pip install seaborn`

## Usage
### Setting up the WhatsApp data file
To use this tool, you'll first need a *WhatsApp data file*. This is a text file that can be generated by going into your WhatsApp app and navigating to the chat you want to analyse. Once you are there, press the three dots on the top right, press 'More', then press **Export chat**.

This will generate a .txt file filled with up to 40,000 messages from the selected chat. Give this file a simpler name then place it in the texts directory in this project.

Then, open the **CHANGEME.ini** file and change **textpath** to point to the path of the file. Change **gcname** to the name of your chat (this will be displayed in the figures' titles).

### Generating Graphs
There are a number of different graphs that can be generated. A brief description of each graph is shown in CHANGEME.ini. You can toggle whether these graphs will be generated by changing *false*'s to *true*'s and vice versa.

All graphs that are generated will be placed in the out/ directory. You can look at the individual graphs there.

Alternatively, a HTML file is present in html/ that presents all of the graphs on a single page. Simply open that page in a browser to view the images together.




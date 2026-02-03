Language Option:

[中文](README_SC.md) | English

---

# Wingmon - More Elegant Browsing Experience

![Wingmon](logo.png)

Wingmon is a browser sidebar extension designed to deeply integrate Large Language Models into the browsing experience.
Unlike other products, Wingmon is a complete Agent capable of accessing web pages and even operating the browser, rather than just a simple chat window.

---

## Why Wingmon

### AI No Longer Just Tells Users What To Do

Through unique technical solution, Wingmon continuously operates the browser **in a human-like manner**, including clicking buttons and links, opening and closing tabs, switching tabs, etc.
We placed our trust in LLMs, and our bet paid off. Relying solely on these basic capabilities, Wingmon has demonstrated excellent productivity in real-world tasks.

In a case study involving information research, Wingmon performed the following actions:
- Entered search terms into Google and initiated a search;
- Clicked on several credible search results;
- Summarized the search results and closed the tabs;
- Presented the data to the user in a visual format;

Demo Video:

![Capability Demo Video](show.mp4)

### Simple Scenarios

More often than not, we don't need AI to perform complex operations for us; we simply want to ask questions about the content on the page.
Thanks to its end-to-end framework design, Wingmon handles this perfectly as well.
Users simply click the "**Send with Page**" button, and the page content is presented directly to Wingmon, bypassing tool calls and minimizing potential misunderstandings.

---

## How We Connect Wingmon with Users

### Trust
#### Wingmon has no backend.
To empower the Agent sufficiently, permissions are necessary. Although we have minimized them as much as possible, this may still not be enough to reassure everyone.
Based on our philosophy of privacy protection:
- **Wingmon does not provide built-in models**
- **Wingmon has no server backend**
- **All usage records disappear after uninstallation**

Wingmon currently supports the Chat Completion API and Response API. You can use your trusted service providers or even local models.
When selecting a model, the reference standard we recommend is [Tau-2 Bench](https://arxiv.org/abs/2506.07982).

### Less is More
We are well aware that such products should not overly interrupt the user's browsing experience.
- Wingmon resides in the browser **sidebar**; you can open it with one click or let it recede completely into the background with one click.
- "Noisy" products are annoying. We are committed to leveraging powerful capabilities with minimal interface complexity, and facts have proven this to be feasible.

---

## Installation and Usage

Wingmon is a closed-source extension. We plan to launch it on the Chrome Web Store in the future.
It is currently in the public beta phase and requires manual installation.

### Installation Steps:
1. Download the zip file from the Release page and unzip it.
2. Open the Chrome or Edge browser.
3. Enter and visit `chrome://extensions/` or `edge://extensions/` in the address bar.
4. Turn on the **"Developer mode"** toggle on the page.
5. Click the **"Load unpacked"** button that appears.
6. Select the Wingmon folder.
7. Click the Wingmon icon on the browser toolbar to open the sidebar.
8. Upon first use, you will need to fill in the configuration.
9. Click save, and you can start chatting with Wingmon.

---

## Roadmap

### Coming Soon:
- Autonomous form filling.
- Display of Reasoning content.

### Under Evaluation:
- Autonomous page scrolling to browse information.
- A local server to expand capability boundaries.

---

## Appendix

### Contact
If you have questions or suggestions, please post an issue. If you are willing to participate in development or request a source code security review, please contact:

Email: damoy@tuta.io

### Limitations
We must clarify that not all models will perform satisfactorily after being integrated into Wingmon.

Before use, we strongly recommend that you understand the Agentic capability level of the model you are using.
Currently known potential issues:
- Web information gathering capability:

  Some models may autonomously use the search engine but fail to actively click on the results. This is largely because the search tools used during their training process returned results directly, causing the models to overfit on "search" operations.

# Purpose
I was sick of scrolling the the right all the time when ChatGTP was displaying code. I just wanted the chats to take up the entire width of the browser window so I created this extension which just overwrites a few lines of CSS to accomplish the goal.

# Implementation
This is the entire extension:

Remove the gap and force max-width.
```CSS
article > div > div {
	gap: 0px !important;
	max-width: 100% !important;
}

```

Remove the openAI logo beside each response to create more space.
```CSS
article > div > div * div.gizmo-bot-avatar {
	display: none !important;
}
```

## Install
Install from store and refresh your ChatGTP tab.
# Udemy Scale Workaround

## Problem Acknowledgement

After having an issue with udemy's scaling issue, I did some research and found a fix. I will explain everything here and show the process for how I was able to fix this issue.


## Solution Section

### Identifying the Issue / Troubleshooting

- Discovered that the website would not scale correctly for test sections
- Already tried clearing cookes / cache for website.
- Tried disableing / removing all extenstions on Chrome
- Ended up Finding some Things on Reddit about the specific issue

### The Specifics

According to [Reddit](https://www.reddit.com/r/Udemy/comments/1rvqs60/comment/oc7bt5f/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button). This is a common issue for some people using the Chrome broswer and I decided to follow their instructions.

![Reddit Post](https://github.com/CHarris-VR/udemy-scale-workaround/blob/main/pictures/redditpost.png)

### Div Specific Class Issue

The issue will be shown here related to the div known as "curriculum-item-view--scaled-height-limtiter"
![Devtool Picture](https://github.com/CHarris-VR/udemy-scale-workaround/blob/main/pictures/devtoolpicture.png)

Which I believe should be fixed within the websites own code so that thrid party extensions don't need to be utilized.


### Code Fix and Stylus Extnsion Utilization
![code fix](https://github.com/CHarris-VR/udemy-scale-workaround/blob/main/pictures/codefix.png)

If you would like to directly copy and utilize the code I have the code snippit for my specific scaled height limiter, yours may be different so ___make sure to check the last bit of text and numbers that may be attached after "limiter"___

```css
.curriculum-item-view--scaled-height-limiter--lEOjL {
    max-block-size: none !important;
    height: 70vh !important;
}
```

### How to set Up Fix for Google Chrome
- Make sure you are using Stylus extension for Google Chrome
- Make sure the code is pointing towards "URLs Starting With:" https://www.udemy"
- Add the code to the coding section
- Give it a memorable name and Save changes

All pages regarding udemy will be up to date with your fixes and changes. 

___NOTE___:  My height is different than what is recommended in the above reddit post that has the fix and the related issues, I like having a bit of the view height to show the underside tabs. so instead of making the scaled hieght 100% of the view I made it 70% aka the 70vh.



### Before / After
Last but not least just showing the original issue and the finished soultion. 
![Original Issue](https://github.com/CHarris-VR/udemy-scale-workaround/blob/main/pictures/originissue.png)


![Resolved Issue](https://github.com/CHarris-VR/udemy-scale-workaround/blob/main/pictures/resolvedissue.png)
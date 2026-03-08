# Cyber Neon for Uptime-Kuma (tested up to 2.2.0)

This theme comes in three variants, the standard 3-wide, now in darkmode also that is not very dense and a compacted 4-wide variant! Choose whatever flavor you like. If there are any issues or you want darkmode compact since that was me messing around please let me know.

## IMPORTANT
Since this removes the default icon and title text from view, set your desired site icon prior to applying it! then you can move forward to the next steps.

### ISSUES
1. Using a title will still display it to the right of the themed one if you are on an older version, you will need to inspect the title and replace the Vue data-v-xxxx with the correct ones in the below code which then goes at the end of the theme css. This also will apply if theme does not get updated for new releases fast enough.
```css
span[data-v-7d4a7f28][data-v-007873bc] {
    display: none !important;
}
```

### Usage
1. Select Dark as the page preference instead of automatic or light.
2. Copy your chosen variant into Uptime Kuma's custom CSS block.
3. Find the header line with ctrl+f or however and change the text between the brackets to whatever you want:

       content: "[ **YOUR DOMAIN // **CHANGE TO ANYTHING IN THIS SPACE ]" !important;

   If you selected darkmode (theme not page mode):

        content: "[ SUDOCAT.DEV // SYS_STATUS ]" !important;

Group titles are left-aligned by default, except for Darkmode. To center them, paste this at the end of the theme or view centered-titles.css (same thing):

```css
.title-section {
  display: flex !important;
  align-items: center !important;
  position: static !important;
}

[data-testid="group-name"] {
  position: absolute !important;
  left: 0 !important;
  right: 0 !important;
  text-align: center !important;
  pointer-events: none !important;
  z-index: 1 !important;
}

.title-section svg {
  position: relative !important;
  z-index: 2 !important;
  flex-shrink: 0 !important;
}
```
If you want a thematic format for your description, like I have set for mine here is that code and preview is below, change up the text of course.

```html
<div style="text-align:center;font-family:'JetBrains Mono',monospace;max-width:700px;margin:0 auto;padding:10px 0;">
<span style="font-family:'Orbitron',sans-serif;color:#00f0ff;font-size:1.1rem;letter-spacing:6px;text-shadow:0 0 10px #00f0ff;">
SUDOCAT // PUBLIC UPTIME DISCLOSURE
</span>
<br><br>
<span style="color:#aaa;font-size:0.85rem;letter-spacing:2px;line-height:2;">
This feed is provided as a courtesy.<br>
Infrastructure events are classified until resolved.<br>
</span>
<br>
<span style="color:#ff2a85;font-size:0.85rem;letter-spacing:2px;line-height:2;text-shadow:0 0 8px #ff2a85;">
Your patience is noted. Your frustration is irrelevant.<br>
All services will be restored in due course.
</span>
</div>
```



### Save and enjoy!

**Full-sized 3 wide**
[![Cyber Neon Demo](https://raw.githubusercontent.com/Sayamew/kuma-theme-cyber-neon/main/previews/cyber-neon-full.png)](https://youtu.be/x27mJT_q5PA)

**Compact 4 wide**
![Cyber Neon Compact](https://github.com/Sayamew/kuma-theme-cyber-neon/blob/main/previews/cyber-neon-compact.png?raw=true)

**Darkmode 3 wide**
![Cyber Neon Darkmode](https://github.com/Sayamew/kuma-theme-cyber-neon/blob/main/previews/cyber-darkmode.png?raw=true)

**Thematic description formatting?**
<img width="1300" height="570" alt="image" src="https://github.com/user-attachments/assets/8a9cb146-9b37-4f0b-9bcd-b4eeadb404fc" />




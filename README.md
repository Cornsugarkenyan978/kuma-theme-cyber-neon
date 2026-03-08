# Cyber Neon for Uptime-Kuma (tested up to 2.2.0)

This theme comes in two variants, the standard 3-wide that is not very dense and a compacted 4-wide variant! Choose whatever flavor you like. If there are any issues please let me know. If you want group titles centered read below.

## IMPORTANT
Since this removes the default icon and title text from view, set your desired site icon and title to what you want in navbar prior to applying it! then you can move forward to the next steps.

### Usage
1. Copy your chosen variant into Uptime Kuma's custom CSS block.
2. Find the header line with ctrl+f or however and change the text between the brackets to whatever you want:

       content: "[ **YOUR DOMAIN // **CHANGE TO ANYTHING IN THIS SPACE ]" !important;

Group titles are left-aligned by default. To center them, paste this at the end of the theme or view centered-titles.css (same thing):

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

### Save and enjoy!

**Full-sized 3 wide**
[![Cyber Neon Demo](https://raw.githubusercontent.com/Sayamew/kuma-theme-cyber-neon/main/cyber-neon-full.png)](https://youtu.be/x27mJT_q5PA)

**Compact 4 wide**
![Cyber Neon Compact](https://github.com/Sayamew/kuma-theme-cyber-neon/blob/main/cyber-neon-compact.png?raw=true)




## ineedaresume

Build great resumes with [ineedaresu.me](http://ineedaresu.me).

This repo was built as a way to capture the evolutions of my work experience.

Fork this repo and update your resume information accordingly in **resume.json**


## How to use

1) Update the **resume.json** with your own details
2) Open [ineedaresu.me](http://ineedaresu.me) preferably in an incognito window so as to start fresh
3) Copy the content of the **resume.json** into your clipboard
4) In the browser console, type the following
```javascript
let resumeJson = <paste your resume.json content here>;
for(key in resumeJson) {
  localStorage.setItem(key, JSON.stringify(resumeJson[key]));
}
```
5) Refresh the page.
6) Accept to load resume from localStorage. The site should load now with all your content.
6) Goto **Finish up** tab to preview your resume
7) Make any tweaks you want to and save a PDF copy.

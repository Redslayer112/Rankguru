# Rankguru
Rankguru GUI for retrieving Test List Data

## Installing :
### You can go to the release page install the latest version of your os

## Usage :
### After you install, :
#### First make a new json file called "auth.json" in the same folder where Rankguru.exe is . . .      -*IMPORTANT*

### To get Auth :
- Login to rankguru.com
- Open the category of your exams (Ex - All India level exams)
- Open Dev tools by clicking Ctrl + Shift + I *or* F12
- Go to console tab in dev tools
- Paste this :  
`const ca=document.cookie.split(";");for(let o=0;o<ca.length;o++){let n=ca[o];for(;" "===n.charAt(0);)n=n.substring(1);0===n.indexOf("token=")&&(t=n.substring("token=".length,n.length),console.log({Accept:"application/json, text/plain, */*",Authorization:t,accesscontroltoken:localStorage.accessControlToken}))}`  
- The console will return a object
- Right on the object and click on copy object
- Now you have the auth, open the auth.json file using a code editor or notepad
- Paste the auth
- Then save the file and close your editor


To get ans you need qpid (questionpaperid)
### To get QPID :
- Login to rankguru.com
- Open the category of your exams (Ex - All India level exams)
- Open Dev tools by clicking Ctrl + Shift + I
- Go to console tab in dev tools
- The last log in console is called TestListData, expand it or click on the arrow before it
- The number of exams you see in the website will be here(inside TestListData of this category of exams)
- The first exam is the same as 1st option inside TestListData (Ex - 1st exam = 0, 2nd Exam = 1)
- Open the exam which you want to find qpid or ans,
- Look for "questionpaperid" option
- copy the value of questionpaperid (the numbers and alphabets bext to questionpaperid)
- Now you have copied the questionpaperid, Open Rankguru app which you have donloaded from here, and paste it
- The app will return the ans of the qpid or the question paper

## If you are comfortable using CLI you can checkout: https://github.com/SwaminathShiju/rankguru

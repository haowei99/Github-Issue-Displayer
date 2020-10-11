# issue-explorer

A simple Vue.js web application that displays issues of a given repositary. 

Features Implmented:
- Smooth transistion from home page to issue page with animation
- Cover the case of an error fetching the results
  - Case 1: Invalid repo/Repo not found
  - Case 2: No issues in the repo
- Allow users to be able to share states via URLs to other users so that they can view results without searching!
- Slight change to design to make it look more modern (instead of X sign, I added a home button on the nav bar)
- Labels are truncated in case it is too long. Hovering over the labels will popup tooltip that has the full name of the label
- Add link to issues/pull request on each card so users can refer to the issue on Github easily

Logic for sorting issues:
- Issues that are closed take precedence over pull request (if case is closed and there's a pr for the repo, only the closed icon will show up in the card)
- Issues that are open and has an active pull request will have a pull request icon show up on the card
- Issues that are open and has no active pull request will not have any icon on the card (to indicate it is an open case)

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve

Use this command to run the project on localhost
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

### Appendix: Screenshots of the app
#### Laptop
![Home Desktop](/demo_pic/home_desktop.PNG)
![Issue Desktop](/demo_pic/issue_page_desktop.PNG)

#### Ipad
![Home Ipad](/demo_pic/home_ipadPro.PNG)
![Issue Ipad](/demo_pic/issue_page_ipadPro.PNG)

#### Iphone
![Home Iphone](/demo_pic/home_iphone.PNG)
![Issue Iphone](/demo_pic/issue_page_iphone.PNG)





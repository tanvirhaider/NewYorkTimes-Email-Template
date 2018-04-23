# NYT Email Template

### Step 1:  Install NodeJS and NPM (Node Package Manager)
https://nodejs.org/en/

### Step 2:  Clone the repo in your project directory
```bash
git clone git@github.com:tanvirhaider/NewYorkTimes-Email-Template.git
```

### Step 3:  CD into downloaded file
```bash
cd NewYorkTimes-Email-Template/
```

### Step 4:  Install Necessary Node Modules
```bash
npm install
```

### Step 5:  Run Build to see the preview
```bash
npm run build
```





## Build Commands

Run `npm start` to kick off the build process. A new browser tab will open with a server pointing to your project files.

Run `npm run build` to inline your CSS into your HTML along with the rest of the build process.

Run `npm run litmus` to build as above, then submit to litmus for testing. *AWS S3 Account details required (config.json)*

Run `npm run mail` to build as above, then send to specified email address for testing. *SMTP server details required (config.json)*

Run `npm run zip` to build as above, then zip HTML and images for easy deployment to email marketing services. 

### Speeding Up Your Build

If you create a lot of emails, your build can start to slow down, as each build rebuilds all of the emails in the
repository. A simple way to keep it fast is to archive emails you no longer need by moving the pages into `src/pages/archive`.
You can also move images that are no longer needed into `src/assets/img/archive`. The build will ignore pages and images that
are inside the archive folder.

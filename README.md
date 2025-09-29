# JAAW - JUST ANOTHER ANIME WEBSITE

JAAW is live on [RENDER](https://jaaw-official.onrender.com/) (desktop only, use an ad blocker 😅)

---

## FRONTEND
- React JS
- Tailwind CSS
- Axios

## BACKEND 
- FastAPI
- Node

---

## To Run Locally

### Available Scripts

In the project directory, you can run:

### `npm start`
Runs the app in the development mode.  
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.  
The page will reload if you make edits.  
You will also see any lint errors in the console.

### `npm test`
Launches the test runner in the interactive watch mode.  
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm build`
Builds the app for production to the `build` folder.  
It correctly bundles React in production mode and optimizes the build for the best performance.  
The build is minified and the filenames include the hashes.  
Your app is ready to be deployed!

### `npm eject`
**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

---

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).  
To learn React, check out the [React documentation](https://reactjs.org/).

- [Code Splitting](https://facebook.github.io/create-react-app/docs/code-splitting)  
- [Analyzing the Bundle Size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)  
- [Making a Progressive Web App](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)  
- [Advanced Configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)  
- [Troubleshooting Build Issues](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

---

## Deployment

### Deploying Frontend on Vercel

You can easily deploy the React frontend on **Vercel**:

1. Go to [Vercel](https://vercel.com/) and login/signup.
2. Click **New Project** → **Import Git Repository** → Select your GitHub repo.
3. Configure the project:
   - **Framework Preset:** Create React App
   - **Root Directory:** leave empty (unless your React app is in a subfolder)
   - **Build Command:** `npm run build`
   - **Output Directory:** `build`
4. Click **Deploy**. Vercel will build and host your React app automatically.
5. Your live site URL will be generated, e.g., `https://your-app.vercel.app`.

### Backend Deployment Options

Vercel does **not directly host FastAPI**. You can deploy your backend separately and connect it to the frontend:

1. **Render:** Easy hosting for FastAPI/Node apps. [Render](https://render.com/)
2. **Railway:** Another free hosting option. [Railway](https://railway.app/)
3. **Heroku:** Classic PaaS for backend apps. [Heroku](https://www.heroku.com/)
4. **Vercel Serverless Functions:** If using Node, you can move API endpoints into `/api` folder. More info: [Serverless Functions](https://vercel.com/docs/concepts/functions/serverless-functions)

**Important:** Update your frontend `.env` to point to the deployed backend URL instead of `localhost`.

---

## Deploy Frontend on Vercel

You can deploy this React frontend directly to Vercel by clicking the button below:

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/Hkmusic/bstation)

> **Note:** This will deploy **frontend only**. Backend (FastAPI/Node) should be deployed separately (Render/Railway/Heroku), and then update the frontend `.env` with your backend URL.
> 
### Notes

- Make sure your backend is deployed before setting the API URL in the frontend.  
- For static sites or frontend-only deployment, Vercel is enough.  
- For full stack, deploy backend on another platform and connect via API URL.

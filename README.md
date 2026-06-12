# RoadFix Telangana

Citizen pothole reporting and tracking system built with Streamlit.

## Features

- Citizen complaint submission with optional road image upload
- Public complaint tracking with status and district filters
- Worker dashboard for status updates and repaired-road photos
- Analytics for district-wise complaints and repair status

## Run locally

1. Create a virtual environment.
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Start the app:

   ```bash
   streamlit run app.py
   ```

## Deploy and get a site link

### Option 1: Streamlit Community Cloud

1. Push this `roadfixtelangana` folder to a GitHub repository.
2. Go to [share.streamlit.io](https://share.streamlit.io).
3. Click **New app**.
4. Select your GitHub repository.
5. Set the main file path to `app.py`.
6. Click **Deploy**.

Streamlit will give you a public URL like:

```text
https://your-app-name.streamlit.app
```

### Option 2: Render

1. Push this folder to GitHub.
2. Go to [render.com](https://render.com).
3. Create a new **Blueprint** or **Web Service** from your repository.
4. If using a Web Service manually, use:

   ```bash
   pip install -r requirements.txt
   ```

   as the build command, and:

   ```bash
   streamlit run app.py --server.port $PORT --server.address 0.0.0.0
   ```

   as the start command.

Render will give you a public URL like:

```text
https://roadfix-telangana.onrender.com
```

## Deployment note

The app uses SQLite and local file uploads. This is fine for a demo or hackathon deployment, but production hosting should use persistent storage such as PostgreSQL plus cloud file storage.

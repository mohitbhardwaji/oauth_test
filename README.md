# Supabase Google OAuth Test App

Small static web app to validate Google OAuth with Supabase.

## What it does

- Shows a **Sign in with Google** button.
- Redirects to Google login via Supabase Auth.
- After login, displays user details on screen.
- Allows sign out.

## Files

- `index.html` - full app (UI + Supabase auth logic).

## Supabase setup checklist

1. In Supabase dashboard, enable Google provider:
   - `Authentication -> Providers -> Google`.
   - Add Google OAuth Client ID and Secret.
2. Configure redirect URLs:
   - `Authentication -> URL Configuration`.
   - Add your local URL (for example: `http://localhost:5500` or `http://127.0.0.1:5500`) in both Site URL and Redirect URLs as needed.

## Run locally

Use any static server from this folder, for example:

```bash
python3 -m http.server 5500
```

Then open:

`http://localhost:5500`

## Validate OAuth

1. Click **Sign in with Google**.
2. Complete Google login.
3. Confirm user details JSON appears.
4. Click **Sign out** to verify logout.

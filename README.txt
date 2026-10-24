HAZRA BARI DUAL TEMPLE — STREAMLIT CLOUD DEPLOYMENT FIX

This package puts app.py and requirements.txt together at the repository root.
The runtime error says psycopg was not imported, even though app.py expects it.

DO NOT delete or reset your Neon database. This fix only addresses Python dependency deployment.

Apply to GitHub repository nilkanth-nilchandika-mandir, branch main:
1. Replace the root app.py with this app.py.
2. Put requirements.txt in the SAME root folder as app.py (not inside a subfolder).
3. Commit both files to branch main.
4. In Streamlit Community Cloud, open the app's Manage app menu and choose Reboot app.
5. Wait for dependency installation to finish, then reload the app.

If Streamlit Cloud is configured to use a different repository, branch, or app file path,
these files must be placed in the configured repository/branch root that contains app.py.
Keep the existing Streamlit Secrets / DATABASE_URL unchanged.

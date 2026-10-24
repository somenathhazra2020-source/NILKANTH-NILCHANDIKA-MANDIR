# Hazra Bari Virtual Dual Temple — Guest Entry Edition

This version keeps the existing Mandir pages and devotional features while changing the entry flow:

- No Sign In or Create Account screen.
- Welcome screen with an **Enter into the Mandir** button.
- Each entry credits **₹1,001 virtual credits**. Returning to Welcome and entering again adds another ₹1,001.
- Removes the visible History section/button, Festival/Theme Control section, and Achievement/Streak dashboard presentation.
- The existing daily deity theme colours remain part of the visual design; only the editable Festival/Theme Control section is removed.

## Deploy on Streamlit Community Cloud
1. Upload `app.py`, `requirements.txt`, and this README to a **new GitHub repository**.
2. Create a Streamlit Community Cloud app from that repository, selecting `app.py` as the main file.
3. In the Streamlit app's Secrets, configure `DATABASE_URL` with your PostgreSQL connection string. Keep credentials private; never commit secrets to GitHub.
4. If your original app also used Panchang or Supabase features, add those existing secret values through Streamlit Settings → Secrets, not into source files.

Virtual credits have no real-world cash value. Each anonymous browser session gets a temporary guest identity; the database stores that session's wallet and devotional activity under a generated guest ID. Clearing the browser session or opening a different session may create a different guest identity.

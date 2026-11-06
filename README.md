# ENJOY CLUB starter project

Included: public games/video listing, admin login and management for games/videos, Express + SQLite backend, basic Socket.IO four-player dice-room backend.

## Run locally
1. Install Node.js 20 or newer.
2. Run `npm install`.
3. Copy `.env.example` to `.env`.
4. Create a bcrypt hash: `node -e "console.log(require('bcryptjs').hashSync('Choose-A-Strong-Password', 12))"`
5. Put the hash in `ADMIN_PASSWORD_HASH`; set `ADMIN_USERNAME`.
6. Set `JWT_SECRET` to a random secret of at least 32 characters.
7. Run `npm start`.
8. Open `http://localhost:3000` and `/admin.html`.

Never publish `.env`, passwords, or secrets. Admin login will not work until the three environment variables are configured.

Limitations: Adsterra link management is not included. The Socket.IO backend exists, but the browser room interface is not implemented. This is a starter, not a production-ready site; it does not include 100 licensed playable games. Configure persistent storage/backups and security review before public launch.
